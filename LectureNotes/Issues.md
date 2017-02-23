# Issue/Bug Tracking

* Not just "bugs"
* All kinds of stuff gets tracked in a tool like this
  * Bugs
  * Feature requests
  * Major project milestones
  * Unsolicited code contributions
  * Documentation requests
* Each item is referred to as _something_
  * Bug
  * Issue
  * Ticket
  * "JIRA"
* We will use "issue"
* A tracker provides...
  * A way to normalize reports from users
    * What version of the code?
    * How severe is the problem?
    * Is it reproducible?
  * A way to formalize an issue's lifecycle
  * Alerting to tell...
    * devs that a user opened an issue
    * the reporter that information has been added
    * watchers that something has changed on the issue
  * Reporting
    * What issues are waiting?
    * What issues are new?
    * What issues do I own?
    * ...etc
  * Filtering or moderating
* Lifecycle stages of an issue
  * Open
    * Info has just been added
    * The data has not been verified
    * The issue may not even be a good issue
  * Open/Working
    * Comments are made on the issue
    * Additional information is added or requested
    * Some discussion occurs here
    * *Warning*: be ready to refer to the development list for better conversation
  * Waiting
    * Details have been requested
    * No one can continue working the issue until the info is provided
    * Sometimes only the person reporting a bug has the environment to reproduce the problem
  * Assigned
    * Someone claims ownership of the issue
    * Generally this means the person can _reproduce_ the issue
    * Diagnosis and analysis is under way
  * Resolved
    * Sometimes called "patch ready"
    * Code is available
    * Hopefully the reporter can use it to test
    * Others examine the code
    * Further discussion may happen on list
  * Scheduled
    * Some future release is targeted to resolve it
    * Code should be in the repo when this target hits
  * Closed
    * Can be closed for many reasons
    * The code fixes/does what was reported and has been added to repo
    * The issue was invalid
      * Sat in waiting too long
      * Not a bug, but misuse of the software
      * This change will never be made by design
    * The issue was a duplicate
    * No one can reproduce the problem
* Note about states
  * Not all trackers use all of these states
  * Some trackers use other states
  * As usual, the project uses the tool how it best suits the needs of the project