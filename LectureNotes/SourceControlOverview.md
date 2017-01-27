# Source Code Management

* What is it?
  * Exactly as it says - manages all the important files
    * Code
    * Documentation
    * Web pages
  * Gives one place to get all the good stuff
    * Can share the location of the repo
    * Know where the latest and greatest version can be found
* "Management" of code?
  * Tracks metadata
  * Creates a "time machine"
    * Any change, ever, can be put back or obtained
  * Allows for experimentation in "sandbox" areas
  * Creates an audit log
    * Who changed what, when and why
    * Helps with attribution
  * Ensures only those allowed can change the code
  * Can help join changes from multiple people on the same file
  * Facilitates code review
  * Release management
    * A topic for another day
* Dangers of what you've only been told about so far
  * What if you lose your local data from accidental deletion or giant lizard attack?
  * It is hard to share the code
    * Sending files around... Who has the latest version?
    * Do I have everyone's changes?
    * Who even made this change?
    * How can we both work on the files at the same time?
  * Multiple people working on one file set can step on toes


## Important version control concepts
* The master server is the canonical place for the code
  * With git, every local copy and fork is a complete copy of the original repository
    * Including all previous commits since ever
    * And is now its own repository
      * You can commit/modify locally and offline
    * This allows for recovery of the repository if the central repository dies
* Version Control all the things
  * Except dynamically created (generated) content
* Most version control systems have a browseable UI
  * Helpful for quickly navigating the code or linking directly to files
  * Easy way to view history
  * Also have "sticky" links for commits and diffs
* Can also "watch" a repository
  * Notify when changes happen
  * Typically provide an email containing the diff
    * Most projects do this with their dev or vcs mailing list
* Useful log messages
  * Make an overview of what and why you changed things
  * Do not just say what you did
  * Sucks: Modify input.c to rename counter variable
  * Does not suck: Rename variable 'ctr' to 'i' in input.c to avoid confusion with 'cntr' variable
* Use a consistent nomenclature for revisions
  * Example: r9926
  * Allows semi-smart scraping to auto generate links
* The commit bit
  * Should ONLY be given to trusted people
    * These are the committers
  * Is earned over time by people that...
    * Demonstrate proficiency
    * Have been involved as a user/contributor
    * Know the project culture
    * Engenders your project's values
  * Typically extended via the following process (which should be documented publicly):
    * An existing committer nominates the person on a private list
    * A discussion is held
    * The matter is put to a vote by the other committers
    * If successful, the person is offered commit access
  * Often grants the ability to vote in some way, too
* Do not overdo authz
  * Keep a "permissions flat" repo
  * Ensure everyone understands the areas they should and should not change
  * Example: With docs and code in the same repo, a person given commit access who works on docs should know not to commit to the code

## Typical workflow - git
Fork the repository in the web UI

Obtain a local copy of the forked repository
```
git clone https://github.com/DRuggeri/OSSClass/OSSClass.git
```

Make the modifications you would like to make
```
vi syllabus.md
```

Add the modified files to the change set
```
git add syllabus.md
```

Commit the changes to the local repository
```
git commit -m "Update syllabus to push back assignment due date"
```

Send the local changes to the remote fork
```
git push
```

Open a pull request in the UI from your repository to the original repository

## Typical workflow - svn
Check out the code from the master server (note the below does not work on github because git!=svn
```
svn co https://github.com/DRuggeri/OSSClass/OSSClass.git
```

Make the modifications you would like to make
```
vi syllabus.md
```

Add the modified files to the change set
```
svn add syllabus.md
```

Commit the changes to the master repository
```
svn commit -m "Update syllabus to push back assignment due date"
```


## Vocabulary
* **Repository** - a hierarchical structure of files containing the objects under version control in addition to metadata about the history of the repository
* **Fork** - a copy of a repository managed separately from the project's formal repository. This may be an individual's personal working repository before submitting changes or a whole new community spinning off from the project.
* **Commit** - to make a change to a repository. With svn a commit is also a push.
* **Push** - (git) to send the local repository's changes to a remote repository
* **Log message** - an overview of why the change was made in a commit
* **Update/Pull** - to synchronize changes from a remote server to the working set/local repository
* **Checkout** - obtaining a copy of the repository at a specific version number (usually the latest commit)
* **Clone** - (git) obtaining a copy of the repository at the latest commit
* **Working copy** - the isolated, local set of files from the repository
* **Revision** - a specific version of a file or directory
* **Changeset** - a series of changes to one or more files or directories grouped together for a commit
* **Diff/patch** - a textual representation of the differences between two or more files/directories
* **Tag** - a label for a collection of files at a specific revision
* **Branch** - an isolated copy of the code inside the formal repository. Functions almost like a fork, but is still part of the repository
* **Trunk** - typical name for the development branch from which all branches came
* **Merge** - moving/propagating a change from one branch to another. Also: the automatic combination by the version control system of two different changes to the same file
* **Pull request** - (git) a request to incorporate (pull) the changes from one branch or repository to another. Often is a merge of commits from a fork or branch into mainline
* **Conflict** - a situation in which two changes are made to the same file by different developers that cannot be automatically merged by the version control system. Typically the second push/commit must be modified to eliminate the conflict
* **Lock** - to enforce the ability for only one developer to be able to write to specific files/directories in the repository
* **Stash** - to temporarily store modifications in a working set such that the working set can be restored to the previous revision and restored to the stashed version later
* **Log** - the list of revision identifiers with the time/date/author and log message of each revision
* **Revert** - to restore a repository to a previous revision. Note that this is another commit and does not erase the previous commit(s)
