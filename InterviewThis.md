###Disclaimer

This is not a checklist, this is not a shopping list. If you send this entire list to an employer, they probably wont be calling you back. This list is intended to serve as a reference point for things to be aware of during your interview process. Not all of these questions will be relevant to every person or position, you should choose the ones that are relevant to you and what you are interviewing for.  It's ok for there to be questions on this list that you personally do not care about.

The questions on this list are not all appropriate for the initial interview, many could not even be answered by the HR person likely to conduct an initial interview. This list is intended to be a comprehensive collection of things a developer may want to know about a company before they accept an offer.

Use your discretion when choose what questions to ask and when to ask them.

#Interview This!

##Development Process

- What will be my day to day responsibilities?

- What source control do you use? Can you explain why you chose it?

- Are your repos hosted in-house or on a third-party service? GitHub?

- What is your workflow currently, with regards to developers pushing changes. Do you do pull requests, or does everyone just merge to a central repo?

- Are you using a ticket system or is it more play it by ear? 

- Do you have a code review process?

- Do you have established code style rules?
  - Tabs or spaces?
  - Allman or BSD braces?

- What are your development environments like?
  - Virtual Machines?  Local (VirtualBox) or Remote (ESXi)?
  - Does everyone have an identical development environment?
  - Are you using vagrant and/or puppet/chef?
  - How closely do the dev environments mirror your production environment?

- What is your release schedule like?

- Do you maintain separate release and dev branches? (git-flow?)

- Will I be provided with a new laptop?
  - Windows, Mac or Linux? Do I get a choice?
  - Am I allowed to install anything I want on that laptop?
  - Will it have an SSD?
  - How hard do I have to justify software purchases?

- Which comes first, bugs or features?

- Single product, or will I be regularly working on different projects?

- How frequently does your company start a new project?

- Will I communicate directly with clients on a regular basis, or does this typically happen through an intermediary?

- Do developers make estimates on deliverables, or are due dates normally decided upon ahead of time?

- What can I expect to see in terms of project specifications and/or mock-ups prior to beginning a new project?

- How do you track development time?
 
- How do you handle change requests?

- Do you have a SLA (Service Layer Agreement)?
  - Do you gaurentee any of the following? If so, how long?
    - Turn Around Time TAT?  
    - Average Speed to Answer (ASA)
    - Time Service Factor (TSF)
  - What is the escalation plan?  What are the consequences if the plan is not followed?
  - Do you have on call hours?
    - What is the on call schedule 



##Remote

- Will the company pay for home office equipment such as monitors or furniture?
  - If yes, will that equipment be considered company property?
  - Would I have to return it if/when I leave the company?

- Do you have a team chat setup such as IRC or Jabber? Do your developers actively use it, is it their primary communication channel?

- Do your developers use video chat software such as Skype or Google Hangouts?

- If a portion of the team works in-office, do you have a dedicated computer to be used for video chat with remote employees?

- Will I have to work over a VPN?
 
- How frequently will I be expected to visit the office?

- Will my visits be reimbursed?

- How flexible are my hours? Can I take time off during the day if needed and make up for it in the evenings?


##Codebase / Architecture

- How old is your codebase?

- Do you unit test?
  - What libraries do you use?
  - What is your testing methodology? (BDD, TDD, Spike & Stabilize, ...)
  - What is your current level of test coverage? Are you happy with it?

- Do you regularly correct technical debt?

- On a scale of 1 to 10, how much spaghetti code do you have?

- How well documented is your codebase?
  - Do you use automated documentation systems like PHPDoc or JSDoc?
  - Do you maintain a wiki?

- Pure CSS, or compiled middleware (LESS, SASS, etc)?

- What is your minimum supported version of IE?

- Does your codebase require a build process, and is it automated?

- Do you use MVC or similar code structuring?

- What is your primary backend language, including version?

- Do you host your product yourself (Local, CoLo, VPS) or is it running on a cloud platform such as AWS or Heroku?

- Do you use open source libraries, and are you aware of the licensing on those libraries?


##PHP

- Do you use a public framework or is it an in-house environment?
  - When you find a bug in a public framework, do you give it back to the commumnity?

- Do you use PHP driven html templates, or a third-party template engine such as Smarty or Twig?

- Do you use Composer?

- Which version of PHP are you using? 
  - What is the update plan for new PHP releases



##JavaScript

- jQuery, Prototype, Underscore, Zepto, Dojo, or other?

- Do you use a templating engine, such as Mustache or Handlebars?

- Coffeescript? (If yes, is it required?)

- Does your code follow Crockford code conventions?
  - Semicolons?
  - camelCase variables?

## System & Network Administration / IT Operations

- Do you use a configuration management tool? (Puppet, Chef, cfengine, Ansible)
  - Why was it choosen?
  - Is its use accepted throughout your IT staff?

- Are configurations version controlled?
 
- What is the process for granting a user access rights (RDP, SSH, etc.) to a system?

- Are there multiple access levels for different classes of user?

- Do developers have admin/root rights on systems?
  - If yes: Why?
 
- Do you have different staging environments for testing/development? (Like: DEV, QA, PreLIVE, LIVE)

- Are developers allowed to connect to systems outside of the development environment?

- Do you have a Change Management process? (ITIL, etc.)
 
- How do you organize system administration, application development, application deployment and application operating so they fit together?
 
- Is there a wiki for server documentation/howtos/best practises?
 
- Do you use the same OS distribution on all your servers, or is each server configured for specific needs?
  - Why did you choose your OS? What were the requirements?

- Are development systems and services standarized, or do developers choose their own environments?

- Do tools need to be approved before use, or may I use whatever I want?

- How frequently do you replace server hardware?
 
- Do I have to replace hardware parts myself or is there a dedicated team / external contractor?

- What software / services do you use to load balance?

- Are your applications architectured for horizontal or vertical scaling?

- What is the average uptime of your servers?
  - Do you consider uptime to be a good indicator for system reliability?

- How do you test fault tolerance? Do you have some kind of "[Chaos Monkey](http://techblog.netflix.com/2012/07/chaos-monkey-released-into-wild.html)"?

- Is there a process for self-build packages (.deb/.rpm/.msi) to be put on some internal repository when an official repository can't provide a package/bugfix?
 
- How do you manage IP addresses and DNS records on your network?

- Do you have plans for (switching to) IPv6?

- Do you categorize your networks? (database server network, frontend network, middleware network?) or is everything mixed together in various networks?

- Are DEV/QA/PreLIVE/LIVE systems all in one big network, or is each on a separate network? Are they firewalled so a DEV system can't DoS a LIVE system?

- What is the process for managing rules on internal/external firewalls?

## Monitoring / On-call duty

- Do you use any monitoring software? (Nagios, Icinga, Zabbix, etc.)

- How does it inform staff of error conditions? (Email, SMS, big monitors in each teams room, etc.)

- Is there a permanent on-call duty for each IT team?

- Is there a permanent "control center" that keeps track of events and informs the responsible on-call duty?

- Is there an escalation process if someone cannot be reached?

- Do the developers also have an on-call duty?

- Does time working on incidents/problems afterhours, when on on-call duty, count as overtime?

- Are employees expected to be doing afterhours work while waiting on-call?


##Developer Coordination

- How many developers do you currently have?

- How large are your teams?

- How frequently do team members find themselves in meetings?

- Do your developers pair program on a regular basis?

- Do you have a methodology for project management (Agile, scrum, etc?)

- Do your developers use screen sharing or collaborative coding tools?

- Are teams seated together?

- Do teams have isolated areas from the rest of the staff / other teams?

##Culture

- What would my role at the company be? Where would I be working within the organization?

-	Why are you hiring for this position?

-	What is the rhythm to the work around here? Is there a time of year that it's all hands on deck and we're pulling all-nighters, or is it pretty consistent throughout the year? How about during the week / month? Is it pretty evenly spread throughout the week / month, or are there crunch days?

- What made you (the interviewer) choose to join this company?
  - What do you enjoy the most about working here?

-	Who are the heroes at your company? What characteristics do the people who are most celebrated have in common with each other?

- Is there a company reward system for employee accomplishments?

-	What type of people are successful here? What type of people are not?

- Am I allowed to take my work home with me?

- Am I expected to take my work home with me?

- What are the expectations with regards to hours worked, deadlines, and overtime?

- How much vacation time do you provide?  How much lead time is expected on vacation requests?

- Open office, personal offices or cubicles?

- Is there a dress code?

- What relationship does your dev department have with your sales department? Who sets the deadlines?

- Does the company provide snacks and/or drinks?

- What are your expectations for how many productive hours a developer will have per day?

##Company

- What's the biggest change your group has gone through in the last year? Does your group feel like the recession is over and things are getting better, or are things still pretty bleak?

-	If I get the job, how do I earn a "gold star" on my performance review? What are the key accomplishments you'd like to see in this role over the next year?

-	About which competitor are you most worried?

-	How does sales / operations / technology / marketing / finance work around here? (I.e., groups other than the one you're looking to work in.)

-	What's one thing that's key to this company's success that somebody from outside the company wouldn't know about?

-	How did you get your start in this industry? Why do you stay?

-	What are your group's best and worst working relationships with other groups in the company?

-	What keeps you up at night? What's your biggest worry these days?

-	What's the timeline for making a decision on this position? When should I get back in touch with you?

-	If we have a very successful 2015, what would that look like? What will have have happened over the next 12 months? How does this position help achieve that?

-	What's your (or my future boss') leadership style?

-	How does the company / my future boss do performance reviews? How do I make the most of the performance review process to ensure that I'm doing the best I can for the company?

-	What information is shared with the employees (revenues, costs, operating metrics)? Is this an open-book shop, or do you play it closer to the vest? How is information shared? How do I get access to the information I need to be successful in this job?

- How many non-developer staff members does the company have?

- Who is your healthcare provider?

- What percentage of insurance does your company pay?

- Is your company currently profitable?

- Does your company release open source code?

- What is your company policy with regards to me releasing open source code (personal projects)? If there is an approval process, how lengthy is it?

- What is your company policy with regards to side projects? Am I allowed to work on my own sites?

- Do I own the code I make in my own time on my own hardware?

- Will the company pay for training programs / certifications / conferences? What is the approval process like?





