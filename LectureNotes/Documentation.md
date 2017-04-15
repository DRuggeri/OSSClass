# Must have documentation

* If you want your community to grow, people have to be able to...
  * ... find your project
  * ... use your project
  * ... build your project
  * ... contribute to your project
* Documentation is critical!
  * There is never enough
  * It is never good enough
  * It is never fun to make
* Anecdote about documentation...
  * Inversely useful
  * Those that KNOW the stuff, don't need it
    * ...but need to write it
    * Doco is difficult to write from a newbie's viewpoint
    * Things you "just know" can be hard to document
  * Generally, coders do not like writing doco
    * It is laborious
    * It is drudgery
    * It's painful to write down the stuff you already know

* Files that must exist in your source tree
  * README
    * **SUPER IMPORTANT**
    * All of the immediately important things about the project
      * What is this stuff (the files inside)
      * How do I build this software?
        * Required [dependencies](Dependencies.md)
        * What build software is used (may mean I have to download something else)
        * Environment or command line variables
        * Sometimes this can be pretty involved, so lives in its own file called BUILDING
      * How do I use the software?
        * Required [dependencies](Dependencies.md) for runtime
        * Basic overview
        * Should be a pointer to the full documentation
    * Cool trick: In github, make a README.md file
      * This becomes the landing page of your project
      * Most hosting tools work this way as well
  * CHANGELOG
    * Informs users what noteworthy changes have occurred
    * High level notes
    * A quick glance to know if the new version is worth grabbing
      * It fixes a bug
      * It adds a feature
      * It improves performance
  * LICENSE
    * The exact text of your [license](Licenses.md)
    * Lets the user know what they are getting into
    * Informs people inclined to contribute what model this project has
      * Some users or developers look for certain licenses
  * CONTRIBUTING
    * This is an overview of how to give back to the project
    * What work is expected before a contribution should be made
      * Examples:
        * Software compiles
        * Passes test cases
        * CLA or attribution made
        * Pull request or patch file generated
        * Ticket opened in tracker
        * Discussed on dev list
    * How the contributor should expect to interact
      * Discussion of the contribution
      * Actual submission of the bits
    * How the community is expected to respond
    * Sometimes succinct enough to go in README

* Other documentation
  * WIKI
    * Stands for "What I Know Is"
    * Open place where documentation can quickly be thrown together
    * Most wikis provide lightweight editing facilities
    * Very easy to get going
    * Beware
      * These often fall out of date
      * These often fail badly at decent organization
      * Wikis get spammed by bots sometimes
  * Website
    * You know what a website is
    * This should be the "core" of your documentation
      * Readily accessible
      * Thoughtfully organized
      * Separate sections for various concerns
    * Its job:
      * What IS this project?
        * This is your brochure
        * Home page must be GREAT
        * What problem does the project solve?
        * Why should I even care?
      * How do I USE the project?
        * Someone is interested, get them hooked...
        * Provide a quick introduction
          * HOWTO
          * Overview of getting started
          * If it is complex, break it down a bit (diagrams help)
        * Provide deeper documentation
          * Command line options
          * Configuration options
          * Environment stuff
          * API
      * History or About page
      * Contributing page
    * Developer documentation
      * You want to grow your dev community, so focus there, too
      * What immediately important things are there for a potential developer to know
        * How to get set up to modify the project
          * Is an IDE needed?
          * Are there certain tips and tricks?
      * Common questions asked by folks hacking on the project
