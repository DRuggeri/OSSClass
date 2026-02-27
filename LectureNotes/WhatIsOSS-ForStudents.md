<!-- .slide: data-background="#3a424f" -->
# Introduction to Open Source Software
### _For students_

???
<!-- .element: class="center" -->Something
Some slide notes

----
## Who is this guy?

&nbsp;

Daniel Ruggeri
- Infrastructure guy that loves code and OSS
- Participates in many OSS communities
- Mentor, teacher, handyman... geek

&nbsp;

See LinkedIn if you care for more...
- daniel<span>@</span>bitnebula.com

----
## So many things, so little time

In this presentation
- What is Open Source Software (OSS)?
- Why does Open Source exist?
- History leading up to OSS
- Initial OSS Communities
- Tools
- Terminology
- Licenses

&nbsp;

##### _... what is most interesting to you?_

---
# What Is It?
##### _A program whose source code is publicly available and licensed for use and/or modification_

----
It's software, of course... and it's _everywhere_!
- The Internet
- Government
- Research
- Big data
- Your pocket

----
## Side notes
- There is contention with "free"
  - `Free != Libre != Open`

- Universally agreed: Having the code allows...
  - Inspection of how it works
  - Fixing bugs
  - Making derivatives
  - Enhancing the software

---
# Benefits
##### _Why would anyone GIVE AWAY good software?_

----
Open algorithms/code get more eyes
- So are often more secure
- This allows us to understand how the S/W works
- "No one of us is as smart as all of us"

----
Depending on flavor, may have a backing foundation
- Leveling the playing field
- Removing concern of single-company control
- Lets the community drive the software

----
Ideology around freedom
- Is certain tech a basic human right?
- Freedom as in _'murica_

----
Giving back
- Contributing to projects we get things from
- Moving technology forward

---
# Some History

##### 1970s - 1990s

----
### In The Beginning...
##### _(Well, the 70's, actually)_

- Hardware was the seller
- There were several architectures
- Software was specific to the hardware
- ... and was openly shared (to drive lock-in)

----
### And then...

- Hardware performance levelled off
- A few architectures won out
- Higher level languages came on the scene
- _Software_ now became a differentiator

----
### So someone said
> "We should totally charge people for this stuff instead of giving it away"

---
# Meanwhile...

Separate threads happening simultaneously gave birth to different OSS communities

----
## BSD

- At UCB, UNIX OS was originally "Open"
  - Began adding some utilities
  - Rewrote kernel to add virtual memory support

- The birth of _Berkely System Distribution_ in '78
  - Expanding and reimplementing UNIX
  - All proprietary code eventually replaced

Create a better OS that isn't encumbered by software licenses.

----
## TeX

- A typesetting system by Donald Knuth
  - Developed as his book was produced
  - Interested in digital typesetting

- Began work in '78
  - Interesting license
  - Free code, but protected name
  - Must pass a test to be called `TeX`

Just be true to the name.

----
## FSF

- Richard Stallman in AI lab at MIT (culture of sharing)
  - Co-workers hired by a proprietary s/w company
  - New h/w with proprietary OS came to the lab

- "This sucks", so around '83
  - Resigned and started _Free Software Foundation_
  - Created (with others) _GNU Public License_
  - Started the GNU project (free OS and utilities)

Injected politics into the conversation.

----
## X Windows

- An MIT project
  - Hardware and vendor independant graphics
  - Lots of attention from vendors

- Became a consortium
  - Formed in '88 from several vendors
  - Neat license: open core, but can be expanded

Level playing field to let vendors compete on differentiators.

----
## ASF

- Free NCSA HTTPd
  - Several folks ran websites with it
  - It was abandoned in '94

- "Oh no!"
  - Apache group formed in '93
  - Shared patches and enhancements
  - 8 developers created an ad-hoc community
  - Became _Apache Software Foundation_ in '99

Value the community. Remove vendor dependence.

---
# Tools of the Trade

When multiple people that are geographically dispersed work on the same code, tools are _required_ to make it all work

----
## Source Control

A time machine for the code
- The code isn't just on your machine
- Changes are made locally and sent to the server
- Mistakes can be reverted to a previous revision

Popular tools:
- Git
- Apache SVN (subversion)
- mercurial

----
## Build Systems

Automates the build
- ... and sometimes the gathering of dependencies
- A vital part of Continuous Integration
- Distills the steps to build the s/w into a "script"

Popular tools:
- Gradle
- Apache Maven
- Apache Ant

----
## Issue/Ticket Tracking

Tracks issues or tickets (of course)
- Allows users/project members to report bugs
- Facilitates collaboration/info sharing around issue
- Assign owners, share patches, etc

Popular tools:
- Bugzilla
- JIRA
- Trac

----
## Other Collaboration Tools

Various other tools exist for various purposes
- Realtime chat for takling and ChatOps
- Patch management for discussing code changes
- Message forums for ongoing conversations
- WIKI sites for easy documentation

Popular tools:
- Slack/HipChat/IRC
- GitHub/GitLab/BitBucket
- phpBB/FUDforum/Discourse
- MediaWiki/Confluence/MoinMoin

---
# Terminology

Let's get on the same page about terms first

----
## Free Software

> "Software that can be freely shared and modified, including in source code form"

- Coined by FSF
- "Free" ambiguity acceptable to emphasize FREEDOM

----
## Open Source

> "... goal at the time was largely to make such software a more palatable choice for corporations, by presenting it as a development methodology rather than as a political movement."

- Coined by OSI
- Means the same thing, but different

----
## Proprietary/Closed

Software that places restrictions on it's use
- Access to source code
- Redistribution of the software

Sometimes has uncommon restrictions
- Field/industry of use

----
## Copyleft

Licensing that requires derivitives or use of the software to also be Free and/or use the same license

- Often called "viral"
- This scares people that wear ties

----
## Permissive License

A license that does not restrict derivitives

- May be incorporated into proprietary works
- May be used without contributing back

---
# Licenses
##### _(The fun part!)_

----
## The license...
Determines rights

- How may I use it?
- May I view the code?
- May I modify the code?
- May I distribute modifications?
- Must my modifications also be open?

----
## A Sea of Licenses!

Nearly all say:
- Anyone can modify the code
- Anyone can redistribute in original/modified form
- Copyright holders provide no warranty

Differences:
- Compatibility with proprietary/other free licences
- Enforcement of attribution
- Trademark protection
- Patent protection

----
## A few of the most popular licences...

----
### MIT

Permissive license
- Developed at MIT (of course)
- Has several derivitives
- Software derivitives must...
  - Include a copy of the license
  - Provide attribution

----
### GPL

Copyleft license
- Created by FSF
- Has a few variants
  - AGPL - viral for nearly anything that touches it
  - LGPL - copyleft stops at binary linkage/including
- Derivitives must...
  - Be GPL licenced
  - Provide attribution
  - Provide code

----
### Apache 2

Permissive "business-friendly" license
- Created by ASF (of course)
- Similar to MIT, but...
  - Grants patent license
  - Declares contributions to be covered
- Derivities must...
  - Include a copy of the license
  - Provide attribution

----
### BSD
Permissive license
- Created at UCB
- Has a few variants
  - 2 clause - Pretty much the same as MIT
  - 3 clause - No endorsement by copyright holder
  - 4 clause - Advertisements must acknowledge copyright holder
- Most common is 3 clause

----
## Great source of license popularity
<small>
##### [https://www.blackducksoftware.com/top-open-source-licenses](https://www.blackducksoftware.com/top-open-source-licenses)
</small>

---
## End
