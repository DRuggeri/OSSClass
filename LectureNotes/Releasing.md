
## Releases
* Note #1... just be consistent with g
* Snapshot of code at a specific time
  * Tags help here
  * "Set" of features/ fixes
* A specific version of the software
  * Old bugs have been fixed
  * New bugs added
  * New features added
  * New options added
  * Incompatible changes
* Is a file name followed by version number
  * usually a dash
  * Capitalize or don't... doesn't matter, just be consistent
* Example:
  * foo-1.5.8
  * Foo-1.5.8RC1

## Version numbering
* Represent a contract with your users
  * Must be consistent between releases
  * Easily identifies..
    * Ordering of releases
    * Compatibility information/nature of changes
* Always increases
* Are groups of digits
  * Not decimal points
* Sometimes add a qualifier
  * Alpha
  * Beta
  * Release Candidate
* (Qualifiers follow the version number they will represent)
  * 1.4.0 alpha will become 1.4.0 eventually
* Rules vary by project... But MUST BE CONSISTENT within that project
* Major.Minor.Micro common "rules"
  * Major version is a compatibility boundary
  * Minor version is backwards compatible
  * Micro is forward and backward compatible
* Version compatibility
  * Backward compatibility
    * Allows new versions to talk/use older clients/servers/data
    * When paired with equally new clients/servers/data, may enable new features
    * "Works the way it always has"
  * Forward compatibility
    * Changing between micro up or down should not add or remove functionality
    * Downgrading from 4.1.6 to 4.1.5 should only restore bugs, not lose features
  * Compatibility domain
    * Defines what a Maj.Min.Mic will not break
    * Depends on what your project does
    * Examples:
      * Data formats read or written
      * Messages exchanged over network
      * Application Programming Interface (How other SW calls your code)
        * Function names
        * Parameters for functions
        * Function return data
      * Application Binary Interface (ABI - how compiled code binds to your library)
        * Expectations of memory locations of members within structures
        * Forces new stuff to end of structures
  * Prereleases (alpha/beta) usually get a pass on this
* Adding to Maj.Min.Mic
  * Sometimes adds a patch number after micro
  * Sometimes odd Maj or Min means "in development" and compatibility rules are off

## Releasing
* Open Source usually releases source code
  * Sometimes binaries
  * Sometimes binaries in addition to source
* Code set contained as an archive
  * Non-windows:
    * Source: compressed tar archive
      * gzip or bz2 compression
    * Binary:
      * Native package
      * DSO
      * "Installer"
  * Windows
    * Source: zip
    * Binary:
      * Installer
      * DSO/DLL
      * zip
  * Expected to extract into a directory of the same name as the archive

### Steps
* These are general guidelines and exact procedures vary by project
* Identify release process
  * Release manager
    * Person responsible for identifying and incorporating changes into release
    * Should "own" the release
    * Ensure compatibility domains are followed
    * Has final say
  * Voting
    * Similar as above, but responsibility is shared
    * Changes receive votes
      * Typically three +1 votes needed
      * Sometimes voting rights restricted to certain people
    * Usually a -1 is a veto for that change
* Incorporate changes into release branch
  * Perform votes or identify changes
  * Apply patches or pull requests
  * Tag branch for release
* Package up the release
  * Create change info (CHANGES file)
    * Noteworthy changes in this release
    * Significant bugs fixed
    * Features added
    * Any visible change in behavior
    * Compatibility changes
  * Create archive
  * Distribute archive to project for final testing...
    * On different OS platforms
    * On different architectures
    * With different config options
    * Via the test suite
* Finalize the release
  * Hold vote to proceed with release
  * Sign packages with digital signature (s)
  * Add new version to issue tracker
  * Publish packages to mirrors/distribution points
    * Ensure mirrors are synchronized before proceeding
  * Publish digital signature file(s)
  * Announce
    * On lists
    * On web page
    * On forums