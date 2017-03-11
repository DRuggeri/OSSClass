# Community models
* Shared from least to greatest community "factor"
* For each one...
  * When is it right?
  * Challenges
  * Examples
* The models are all about *governance*
* What is governance (see definition)?
  * Formally put together in bylaws, but not always done so formally as we'll see
  * The set of rules around the project that determines who...
    * ... gets commit bit
    * ... is allowed to make decisions
    * ... settles disputes
    * ... sets community culture
    * ... "owns" the project and branding
    * ... determines the license
  * Depending on governance model, this may also include corporate governance rules
    * Regulatory/compliance
    * Legal/risk

# Models
* Dump and run
  * When code is produced and tossed somewhere...
    * Not actively developed
    * No intent to build a community around it
    * Not watched for issues/bugs
    * User/code feedback not welcome or ignored
    * More or less a dead project
  * When is it right?
    * Just get the code out there
    * Basic utility code
  * Challenges
    * If the code is great or useful, contributions don't make it back in
    * Without a driving "critical mass" of interested devs...
      * The code gets copied to several repos for individual intent
      * No "one" place exists for improvements
      * Feedback has nowhere to go
    * Impossible to create a community without a fork
    * Dead projects are bad juju!
  * Examples
    * gist postings
    * MOST GitHub/SourceForge/etc projects
* Lone wolf
  * A project maintained by one person
    * May or may not be actively developed
    * Feedback is welcomed in some way
    * Common on GitHub/SourceForge/etc
    * Generally not enough "critical mass" for a community
  * When is it right?
    * Project is small
    * Desire to BEGIN a community
    * Individual still wants to assert some sort of control
      * Project direction
      * Branding
  * Challenges
    * It's hard for one person to keep up if the project becomes popular
    * High risk of project dying if the individual...
      * gets busy with life
      * loses interest
      * walks away
      * does not foster a growing community
    * There may be no intent to create a community
    * Sometimes individuals have trouble letting go of control
  * Examples
    * TeX from history lecture
      * Branding note in license
* Open Source, closed governance
  * A living project still controlled by a single point
    * A step up from lone wolf
    * Often maintained by a single "entity"
    * Effort is made to SHOW that it isn't just "one person"
    * Often much higher community involvement
    * Common with companies who open their code
      * Still want to control direction
      * Want to focus on specific features
    * The "entity" may actually be...
      * A single person in a company, but shrouded by the company
      * A delivery team in a company
      * An entire department of a company
      * An entire company
  * When is it right?
    * Same as lone wolf, plus...
    * Project is the foundation for a bigger project
      * This isn't the service I provide, but is required by it
      * Other projects depend on this one
  * Challenges
    * Community direction is still "owned" by a central point
    * Some view this model as a less-than-open model
      * Idealism comes into play
      * But the code is open, and that IS good
    * The "entity" can take the project any direction
      * Whether the community likes it or not
      * A fork is an option, but forks still suck
    * The "entity" can be torn between their goals and the community
  * Examples
    * Netflix Open Source
      * Lots of tools/utilities that Netflix controls
      * The code isn't making them money, but it sure is driving their business
      * ACTIVE community participation (feedback is WELCOME)
* Paid membership/Invite only
  * The governing body is multiple entities, but access to the body is limited in some way
    * The "entity" that governs the project is composed of more than one...
      * Person
      * Company
      * *Commercial interest*
    * Creates a governance _community_ for the project
    * This makes it so no one "company/person" has final say
    * Splits ownership of the project to a collective
      * Reduces risk of one company failing and the project dying
      * Reduces the ability for a particular industry to dominate the project
    * Obtaining rights to the "governing board" is limited
      * Sometimes seats are paid for
      * Sometimes is done only by invite
        * Status in the industry
        * Commercial interest
        * *NOT* merit based - that is our next model
    * Often the governing body is a foundation
      * A "single" entity composed of many
      * More to come about foundations
  * When is it right?
    * To expand the governance of the project beyond a single commercial interest
      * Helps spread the load
      * More perspectives
    * When the project wants to show it is independent of one company
    * Further community growth
    * When you want to instill confidence in the project
  * Challenges
    * Growing governance group creates growing opinions
    * Managing the governing body becomes a task in addition to managing the code
      * Conflicting interests and objectives have to be resolved
      * Sometimes conflict can spill into code discussions
      * Charter and rules for how to gain membership is neccessary
    * Some view this as "pay to play"
      * ... and consider it less-than-open
    * Access to governing body is reserved for those who can afford it
  * Examples
    * Eclipse
    * OpenStack (note that individuals are also on board)
* All volunteers (open code AND governance)
  * Single governing body over the project that is open to anyone
    * Nearly identical to previous example
    * Except access to the board comes from project involvement
      * Meritocracy (see definition)
    * Often requires individuals, not companies, to participate
  * When is it right?
    * As above, plus showing complete independence of the project from corporations
  * Challenges
    * "Corporate shills"
      * Individuals or teams that participate only to serve corporate interests
      * Gives influence to a company when intended for individuals
    * Governing an open governance board is, itself, a large challenge
      * Often described as organized chaos
      * Those that DO, may not be the best at LEADING
    * Often made up entirely of volunteers
      * See risks about Lone Wolf and volunteerism
  * Examples
    * Apache Software Foundation
    * Software Freedom Conservancy
    
# Vocabulary
* **governance** - a set of rules applicable to a project that defines important aspects of how decisions are made in the project
* **bylaws** - a rule made by a company or society to control the actions of its members.
* **Meritocracy** - Philosophy holding that power should be vested in individuals almost exclusively based on ability and talent. In Open Source communities, this also includes contribution to the project.
