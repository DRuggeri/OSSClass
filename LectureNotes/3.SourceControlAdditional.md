# Additional version control topics

## Bewarethe word "fork"
* Can be an overloaded term
* In git speak, it means copying the repository to a separate location
  * Usually a good thing
    * ... since it's the start of a potential contribution
    * ... or nothing at all
  * Either way "Give me a repository just like this one"
* In community speak, it is a much more serio problem
  * The community has come to a disagreement
    * Usually a major disagreement
    * Fundamental problem
  * There is no way forward
  * Neither side will cave
  * The community itself is forked
    * Only solution is to split into two projects
    * Now directly competing with eachother
      * ... for users
      * ... for developers
      * ... aganst proprietary software, too
  * The code base now lives in two places
    * Actively maintained by separate devs
    * Potentially very different project cultures
  * Sometimes projects continue separately
  * Sometimes one or the other folds
  * Sometimes both collapse completely
    * Likely outcome for smaller projects

## Branches
* A total copy of a set of version controlled files/directories
* At the time the branch happens, both are exactly the same
  * Contents
  * History
* Reason to branch: Release branch
  * Users need a stable release version - the code must be stabilized
  * ... but developers want to work on stuff
    * New features
    * Unrelated stuff for the release
  * Solution 1 - freeze work
    * No new features or changes beyond what is intended for the release
    * Everyone focused on getting the release out
    * Common in commercial development
    * Fastest turnaround time to get the release out the door
    * Dangerous for OSS projects
      * Stops devs from working on what they want to work on (unless it's the release)
      * That much control is not guaranteed to a project leader anyway
  * Solution 2 - branch development from stable
    * Requires a bit more care and work for getting changes from development to a stable branch
    * Allows developers to work on trunk
      * New features
      * Incompatible changes
    * The stable branch is less "loose"
      * Isolates active work from things ready for release
      * Requires a more deliberate act to get code into this branch
      * Most projects have a process for this
* Reason to branch: features
  * Sometimes a feature requires a lot of changes
  * ... and collaborators
    * Once you've used SCM right, it's hard to go back to non-collaborative development
  * A branch can be created from an existing branch (stable or trunk) to work on just that feature
    * Allows people to commit and change the branch
    * Allows for experimentation
  * As work is done, it is isolated from the original branch
  * When work is done, the branch can be...
    * merged into the branch it came from
    * deleted since it was just an experiment

## Tags
* An exact snapshot of every file/directory in the repo at a specific time
* Somewhat similar to a branch (point in time copy) except it cannot be modified
* Useful for releases
  * Identifies the exact contents that went into the release
  * Years later, can still obtain the files as they were when the release was done
* Also useful any time a snapshot is desirable
  * Before a rearchitecture
  * Interesting point in the project's history
