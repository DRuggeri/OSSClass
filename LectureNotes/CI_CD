
## CI
* Compiling software was great... but was dangerous
  * What if my computer is compromised?
  * What if I am a malicious coder?
  * What if I don't want to do all that work?
  * What if I made a mistake during the process?
  * What if all that takes me too long?
  * What if I'm checking in a huuuuge amount of code?
* Analysis result: humans suck!
* Enter Continuous Integration!
  * Check code in early and often
  * A build plan is created
  * The plan identifies the steps required to build
  * Also identifies failure points
    * A failure at any point should stop the process
    * Acts as safety nets
  * Tests and whatnot are also defined
  * An automated safety net
    * Input is the code
    * Output is either...
      * A failure alert
      * Successfully built software
    * That's it... no other weird in-between states
* Typical CI steps
  * Triggered by some action
    * Typically a change in the repo
  * Obtains the source tree
    * Puts it in a "cleanroom" area
    * A known starting state
  * Performs static analysis
    * "Reading" the code to identify problems before it is built
    * No "work" is done with the code - it is just read
    * Some examples
      * Bad formatting or style
      * Syntax errors
      * Obvious bugs
        * Unused variables
        * Unreachable code
        * Using uninitialized variables (* not perfect *)
      * Potential security issues
    * Depending on the analysis, you may choose to pass or fail
  * Compiles/builds the software
    * Syntax errors should be caught here if not caught by static analysis
    * Compiler warnings can become a source of stoppage
  * Executes unit and local tests
    * Run test against small components
    * Example: the function "add" should return 4 when given the parameters 2 and 2
  * Packages and bundles the software
    * This is the "artifact"
    * It **shall not** change from environment to environment!
  * Puts it somewhere accessible
    * A binary artifact repository
      * Similar to source code repository/object store
      * Holds immutable (unchangeable) objects
      * Each artifact has a unique URL
  * Keeps the feedback loop tight
    * Failure at any point should notify
    * Success at the end should notify
    * You know as soon as possible when somethign isn't right
      * Colloquially referred to as "shifting left"
      
## Continuous Delivery
* An extension of Continuous Integration
* A whole discipline in and of itself
* A series of practices to...
  * Shorten feedback loop for the customer
  * Ensure software is always in a releasable state
  * Make releases less scary
* The interesting part (to me, at least)
  * Means further automation of the deployment
  * Picks up where CI leaves off
  * Automates the promotion of code all the way to production
* Steps added on to CI
  * Before the code is committed, developer tests locally
    * Further "shifting left"
    * Run as much unit and integration test as possible
    * Find issues before even checking in
  * Code gets checked in and CI kicks off
  * The artifact gets "promoted" to the next environment
    * Testing appropriate for that environment occurs
    * New environments may offer new testing opportunities. Some examples...
      * Development environment may "stub out" services
      * Test environment integrates with those services
        * Verify that integration here
        * Just like CI, a failure should stop the process
      * Staging environment should be like production
        * Do performance and load testing here
        * Perform security scanning and penetration testing
        * Manual testing, too
    * Eventually the code is deployed in production
      * With minimal human intervention
      * With a high degree of confidence the code works
      * As a much smaller unit of work

## Vocabulary
* *Continuous Integration* - a development practice that requires developers to integrate code into a shared repository several times a day. Each check-in is then verified by an automated build, allowing teams to detect problems early.
* *Code promotion* - The act of moving the package/artifact along the delivery lifecycle to the next environment. Example: after successful integration of the code in the development environment, it can be *promoted* to the testing environment

## See also
* https://www.thoughtworks.com/continuous-integration
* https://continuousdelivery.com/
