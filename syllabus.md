# Seminar in Information Systems - Open Source Software Development

## Course Overview
This course is intended to familiarize students with the concepts of Open Source software development. Specific areas of focus are:
* History of Open Source
* Communities and governance
* Technologies used
  * Source control
  * Communications tools
  * Bug trackers
* Legal aspects (licensing/foundations)

Additionally, students should expect to be challenged in areas of personal development related to the business environment such as giving presentations, writing position papers and analyzing failures.

### Administrativia
Toan Pham - tpham0630@gmail.com
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
Communicating well is crtically important in the world outside of the classroom and, similar to giving presentations, is a muscle that must be exercised regularly.
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

### Project
In an effort to simulate real Open Source software development, we will embark upon a team-based project (with team sizes being dictated by the number of enrolled students).

### Extra Credit
Through the course of the semester, students will have opportunities to earn extra credit.
Opportunities will be shared as they come along.

Visit the ISPC events for extra credit opportunities:
http://mis.umsl.edu/Whats%20New/index.html

### Breakdown
Homework  
Presentation  
Paper 1  
Paper 2  
Participation  
Project  

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
* Chapter 1 discussion
* **Homework**: Read Bruce Perens' [Open Source definition essay](http://www.oreilly.com/openbook/opensources/book/perens.html)
  * Stop at "Analysis of the Open Source Definition"
* *Consider starting the Version Control chapter (below)*
* *Consider starting the Source Control for Pointy Hairs Paper*

### Tues Jan 24
* Discuss Open Source definition essay
* Presentation about giving presentations: Dr. Rottman
* SDLC overview/refresher
* Source Control - overview
  * Who gets the commit bit?
  * Communications
* **Homework**: Read [Chapter 3 - Version Control](http://producingoss.com/en/vc.html) section
* *Remember the Source Control for Pointy Hairs paper*

### Thurs Jan 26
* Discuss Version Control learnings
* Source Control - applied
  * Lab: Creating and using repositories
* *Remember the Source Control for Pointy Hairs paper*

### Tues Jan 31
* Source Control - Additional concepts
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
* Building software
  * Local builds
  * Local tools
* Build systems
  * Overview
    * What are they/Why do I care?
    * Declaration of build steps
  * CI
  * CD

### Thurs Feb 9
* Managing dependencies
  * What is a dependency?
  * Why use a library?
  * Automated dependency management

### Tues Feb 14
* Communities and their importance
* Community models (part 1)
  * Open Source, closed governance
  * Lone wolf
  * Dump and run

### Thurs Feb 16
* Community models (part 2)
  * All volunteers
  * Paid membership
  * Invite only
* Growth of open communities (non-code related)
  * Wikipedia/Creative Commons
  * Open Education
  * Open Government

### Tues Feb 21
* Lab - Show how Open Source software can be changed
  * Download
  * Modify
  * Build
* **Homework**: Read Chapter 5 - (Economics of Open Source)[http://producingoss.com/en/money.html#economics-of-open-source] and (Types of Corporate Involvement)[http://producingoss.com/en/types-of-corporate-involvement.html]

### Thurs Feb 23
* Guest Speaker: [Brian Lock](https://www.linkedin.com/in/brian-lock-9390491), Pivotal - How we as a company make money with Open Source
* **Homework**: Read (Chapter 3 - Bug Tracker)[http://producingoss.com/en/bug-tracker.html]

### Tues Feb 28
* Discuss bug tracking chapter learnings
* Issue Tracking - overview
* Bugs vs issues

### Thurs Mar 2
* Issue Tracking - applied
  * Lab: Create an issue
* **Homework**: Create your own issue
  * If this issue is for our class, resolve it with a pull request
  * If this issue is in a real project, extra points if you resolve it!

### Tues Mar 7
* Open time - questions/review for midterm
* Go around the room
  * What issue did you report?

### Thurs Mar 9
Mid term examination

(Mar 13 - mid semester)

### Tues Mar 14
* Licenses!!!
  * Questions that must be asked of every license
    * What are the terms, are they compatible with planned use?
* The "big"  licenses (source)[https://www.blackducksoftware.com/resources/data/top-20-open-source-licenses]
  * MIT
  * GPL 2/3
  * Apache 2
  * BSD
* **Homework**: Read (Chapter 3 - Mailing Lists/Message Forums)[http://producingoss.com/en/message-forums.html]

### Thurs Mar 16
* Discuss communications tools learnings
* Communications tools
  * Mailing lists
  * IRC
  * Forums

### Tues Mar 21
* Paper 2 (The Best Open Source License is...) is due

### Thurs Mar 23
* Guest Speaker: [Chris Kampmeier](https://www.linkedin.com/in/ckampmeier), Mastercard - What is Innersourcing and why we want it

### Tues Mar 28 (spring break)
### Thurs Mar 30 (spring break)

### Tues Apr 4
* Foundations
  * Their role (some examples)
  * US Non-for-profit types
* **Homework**: Read (Chapter 2 - Documentation)[http://producingoss.com/en/getting-started.html#documentation]

### Thurs Apr 6
* Development best practices - Documentation
  * MUST have files: README, CHANGELOG, LICENSE
  * Wiki, FAQ, Website
  * Developer guidelines
  * Translation

### Tues Apr 11
* The importance of credibility in the community
* A path to getting engaged
  * User
  * Contributor
  * Committer
  * Voter

### Thurs Apr 13
* Guest Speaker: [Rich Bowen](https://www.linkedin.com/in/rcbowen), Apache Software Foundation - The Apache Way

### Tues Apr 18
* Software delivery methodologies
  * Waterfall
  * AGILE

### Thurs Apr 20

### Tues Apr 25

### Thurs Apr 27

### Tues May 2

### Thurs May 4
* "Guest Speaker": [Daniel Ruggeri](https://www.linkedin.com/in/danielruggeri), business guy - How to not suck at business

(May 6 - end of classes)

May 9 (finals)

May 11 (finals)

(May 13 - semester close)


## Thanks and Attributions
This class has been shaped through input from many folks, but a few notable contributions are deserved:
* [Seokchan (Channy) Yun's open-source-class](https://code.google.com/archive/p/open-source-class/)
* [The Apache Software Foundation community development project](http://community.apache.org/) - ([mailing list archive](https://lists.apache.org/list.html?dev@community.apache.org))
