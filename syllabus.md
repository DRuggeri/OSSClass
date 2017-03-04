# Seminar in Information Systems - Open Source Software Development

## Course Overview
This course is intended to familiarize students with the concepts of Open Source software development and modern development practices. Specific areas of focus are:
* History of Open Source
* Communities and governance
* Technologies used
  * Source control
  * Communications tools
  * Issue trackers
* Legal aspects (licensing/foundations)

Additionally, students should expect to be challenged in areas of personal development related to the business environment such as giving presentations, writing position papers and analyzing failures.

### Administrativia
Daniel Ruggeri - druggeri primary.net  
Tues/Thus 5:30pm - 6:45pm, 104 ESH  
INFSYS 3898 (Undergrad)  
INFSYS 6891 (Graduate)  

#### Textbook
Open Source Software ~ *Karl Fogel*  
ISBN: 0596007590, ISBN-13: 978-0596007591  
Download free at [http://producingoss.com/](http://producingoss.com/)

## Assignments and Grading
In full transparency, the assignments dished out as well as how they are graded is shared in this section

### Homework
Homework assignments will be passed out from time to time involving reading, researching or taking some action. These assignments should be completed by the next class

### Presentation
Each student will be required to give a short presentation about a topic.

The reason for this requirement is two-fold:
* To ensure a certain level of mastery of the topic such that it can be explained well
* To ensure a certain level of mastery *in giving a presentation*

This is so each student gets experience in exercising their "marketing" muscle which is not only required in the world of business, but also the world of Open Source.
While presentations will be graded on content, a significant portion of the grade will also come from organization of the content, aestetics of any materials presented as well as the ability to adhere to guiding principals for good presentations.

### Papers
Communicating well is critically important in the world outside of the classroom and, similar to giving presentations, is a muscle that must be exercised regularly.
Students will be tasked with writing short papers in the form of:
* **Position papers** in which an opinion and supporting facts (persuasive in nature) should be presented. These documents will be graded on grammar, composition and coherence to the assignment and argument since opinions vary.
* **Summary documents** which should be written in a form suitable for a manager to understand the landscape or overview of a concept they are not familiar with. In addition to the points earned in position papers, these documents will also be graded on accuracy of their factual contents and the simplification of complex topics.

#### Source Control for Pointy Hairs
Exactly 1 physical page  
I am a manager that has worked in manufacturing all of my career but have recently moved to become the manager of a software development team.
I hear people mention "source control" and things like "commit", "branch", "tag" and such but I don't know what any of these things are.
Provide me a one-pager that explains what source control is and gives a few key terms/definitions.

#### The Best Open Source License Is...
At least 2 physical pages  
The legal environment of business and software development is complex.
It's even harder when trying to open a code base because there are so many FOSS licenses to choose from.
What is the best Open Source license out there and why?
Use the first paragraph to make assumptions about why I want to open my code and the remainder of the document to define your choice and explain it.

### Participation
The world of Open Source is driven by community so it is important that the community within our classroom is full of individuals willing to contribute to the success of the whole class.
Therefore, participation during discussions and presentations as well as within code and the project will be measured over the course of the semester and will contribute to a significant portion of the grade.

### Extra Credit
Through the course of the semester, students will have opportunities to earn extra credit.
Opportunities will be shared as they come along.
* Contribute fixes to this course's content
* Contribute fixes to a real Open Source project
* Attend [ISPC events](http://mis.umsl.edu/Whats%20New/index.html)

### Breakdown
* Homework	10
* Class Participation	10
* Paper: Source Control for Pointy hairs	20
* Paper: The best Open Source Licence is...	20
* Midterm	40
* Final	40
* Presentation: Topics Assigned 20
* Presentation: About My Favorite Project	20
* Total	180


## Schedule
This is the planned schedule of events for the course. Since topics may run longer or come up short, expect some minor alterations. It's also important to note that *when you see **discussion** come up in the schedule, you should **expect the instructor to ask questions** that will verify your understanding/homework* as well as to cover some of the topics in depth.

### Tues Jan 17
* Get to know eachother
* Cover syllabus
  * Discuss presentations
  * Discuss project
* **Homework**: Read chapter 1 of book
* **Homework**: Create a github.com account - email me the username

### Thurs Jan 19
* Chapter 1 discussion - [lecture notes](LectureNotes/IntroAndHistory.md)
* **Homework**: Read Bruce Perens' [Open Source definition essay](http://www.oreilly.com/openbook/opensources/book/perens.html)
  * Stop at "Analysis of the Open Source Definition"
* *Consider starting the Version Control chapter (below)*
* *Consider starting the Source Control for Pointy Hairs Paper*

### Tues Jan 24
* Discuss Open Source definition essay
* Presentation about giving presentations: Dr. Rottman
* Source Control - overview
  * Who gets the commit bit?
  * Communications
* **Homework**: Read [Chapter 3 - Version Control](http://producingoss.com/en/vc.html) section
* *Remember the Source Control for Pointy Hairs paper*

### Thurs Jan 26
* Discuss Version Control learnings - [lecture notes](LectureNotes/SourceControlOverview.md)
* Source Control - applied
  * Lab: Creating and using repositories
* *Remember the Source Control for Pointy Hairs paper*

### Tues Jan 31
* Source Control - Additional concepts - [lecture notes](LectureNotes/SourceControlAdditional.md)
  * Beware of "fork" term
  * Branching
  * Tags
* Source Control - applied
  * Lab: Pull requests and patches
* **Homework**: Source Control for Pointy Hairs paper

### Thurs Feb 2
* Paper 1 (Source Control for Pointy Hairs) is due
* Application environments (dev, stage, prod)
* Guest Speaker: [Tom Manor](https://www.linkedin.com/in/thomas-manor-7aa2b110), RedHat - Why I trust Open Source software in my production environment

### Tues Feb 7
* Source Control - applied
  * Another lab to wrap up concepts
* **Homework**: Read [Chapter 7 - Packaging](http://producingoss.com/en/packaging.html#packaging-build-install) "Compilation and Installation" and "Binary packages" subsections

### Thurs Feb 9
* Building software - [lecture notes](LectureNotes/Building.md)
  * Local builds
  * Local tools

### Tues Feb 14
* Managing dependencies - [lecture notes](LectureNotes/Dependencies.md)
  * What is a dependency?
  * Why use a library?
  * Automated dependency management

### Thurs Feb 16
* Lab - Show how Open Source software can be changed
  * Download
  * Modify
  * Build

### Tues Feb 21
* Build systems - [lecture notes](LectureNotes/CI_CD.md)
  * Overview
    * What are they/Why do I care?
    * Declaration of build steps
  * Continuous Integration (CI)
  * Continuous Delivery/Deployment (CD)
* **Homework**: Read Chapter 5 - [Economics of Open Source](http://producingoss.com/en/money.html#economics-of-open-source) and [Types of Corporate Involvement](http://producingoss.com/en/types-of-corporate-involvement.html)

### Thurs Feb 23
* Guest Speaker: [Brian Lock](https://www.linkedin.com/in/brian-lock-9390491), Pivotal - How we as a company make money with Open Source
* **Homework**: Read [Chapter 3 - Bug Tracker](http://producingoss.com/en/bug-tracker.html)

### Tues Feb 28
* Discuss bug tracking chapter learnings - [lecture notes](LectureNotes/Issues.md)
* Issue Tracking - overview
* Bugs vs issues

### Thurs Mar 2
* Issue Tracking - applied
  * Lab: Create an issue
* **Homework**: Create your own issue
  * If this issue is for our class, resolve it with a pull request
  * If this issue is in a real project, extra points if you resolve it!

### Tues Mar 7
* Go around the room
  * What issue did you report?
* Open time - questions/review for midterm

### Thurs Mar 9
Mid term examination

(Mar 13 - mid semester)

### Tues Mar 14
* Communities and their importance - [lecture notes](LectureNotes/Communities.md)
* Community models (part 1) - [lecture notes](LectureNotes/CommunityModels.md)
  * Open Source, closed governance
  * Lone wolf
  * Dump and run

### Thurs Mar 16
* Community models (part 2) - [lecture notes](LectureNotes/CommunityModels.md)
  * All volunteers
  * Paid membership
  * Invite only
* Growth of open communities (non-code related)
  * Wikipedia/Creative Commons
  * Open Education
  * Open Government
  * Open Street Maps

### Tues Mar 21
* Licenses!!! - [lecture notes](LectureNotes/Licenses.md)
  * Questions that must be asked of every license
    * What are the terms, are they compatible with planned use?
* The "big" licenses [source](https://www.blackducksoftware.com/resources/data/top-20-open-source-licenses)
  * MIT
  * GPL 2/3
  * Apache 2
  * BSD

### Thurs Mar 23
* Guest Speaker: [Chris Kampmeier](https://www.linkedin.com/in/ckampmeier), Mastercard - What is Innersourcing and why we want it
* **Homework**: Read [Chapter 3 - Mailing Lists/Message Forums](http://producingoss.com/en/message-forums.html)

### Tues Mar 28 (spring break)
### Thurs Mar 30 (spring break)

### Tues Apr 4
* Discuss communications tools learnings - [lecture notes](LectureNotes/CommunicationsTools.md)
* Communications tools
  * Mailing lists
  * IRC
  * Forums
* Paper 2 (The Best Open Source License is...) is due

### Thurs Apr 6
* Foundations - [lecture notes](LectureNotes/Foundations.md)
  * Their role (some examples)
  * US Non-for-profit types

### Tues Apr 11
* The importance of credibility in the community
* A path to getting engaged
  * User
  * Contributor
  * Committer
  * Voter

### Thurs Apr 13
* Guest Speaker: [Rich Bowen](https://www.linkedin.com/in/rcbowen), Apache Software Foundation - The Apache Way
* **Homework**: Read [Chapter 2 - Documentation](http://producingoss.com/en/getting-started.html#documentation)

### Tues Apr 18
* Development best practices - [lecture notes](LectureNotes/Documentation.md)
* Documentation
  * MUST have files: README, CHANGELOG, LICENSE
  * Wiki, FAQ, Website
  * Developer guidelines
  * Translation

### Thurs Apr 20
* Software delivery methodologies - [lecture notes](LectureNotes/SDLCMethodologoies.md)
  * Waterfall
  * AGILE

### Tues Apr 25

### Thurs Apr 27
* Releasing software - [lecture notes](LectureNotes/Releasing.md)
* Versioning
* Release procedures

### Tues May 2

### Thurs May 4
* "Guest Speaker": [Daniel Ruggeri](https://www.linkedin.com/in/danielruggeri), business guy - How to not suck at business

(May 6 - end of classes)

May 9 (finals)

May 11 (finals)

(May 13 - semester close)


## Thanks and Attributions
This class has been shaped through input from many folks, but a few notable attributions are deserved:
* [Seokchan (Channy) Yun's open-source-class](https://code.google.com/archive/p/open-source-class/)
* [The Apache Software Foundation community development project](http://community.apache.org/) - ([mailing list archive](https://lists.apache.org/list.html?dev@community.apache.org))
* [Karl Fogel](http://www.red-bean.com/kfogel/)'s work on the [Producing Open Source Software](http://producingoss.com/) book
