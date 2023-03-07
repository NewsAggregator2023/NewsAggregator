# Management Process and Principles
## Principles
Due to being a medium sized project team, we need to keep the documentation and management of the project reasonably light to ensure we can deliver valuable outcomes. 
Using automation and templates where possible, we can reduce the work overhead of documentation. We are also focused on operating as a high performing team, and will implement processes which prioritise team wellbeing and support. 

# Project Management Process
The team will be utilising a mix of Scrum, XP and Kanban to assist the development process and maintain a high-performing team. 

## Kanban:
Kanban focuses on representing a project visually by decomposing the project into individual tasks. These tasks are listed on a Kanban board (with swimlanes indicating the completion status of a given task). Kanban promotes incremental development by visually showing individual tasks as part of the larger project and allowing the team to prioritize which tasks they will currently focus on. Each task’s completion status shows the progress of a task and if any actions are needed. The statuses used in this project are listed as part of Scrum.

## Scrum:
The team is utilising Scrum as the main inspiration for our management process. We see particular value in the __iterative, collaborative, value-driven prioritisation and adaptable principles__ of Scrum. We will use __sprint planning, weekly standups, product demos and retrospective meetings__ to focus on the planning, business as usual, celebration of work and reflection. 

We will be using estimation tools like __planning poker__ to schedule and allocate tasks based on anticipated effort. This estimation will also act as the basis for __project reporting__. We will use __user stories__ to encapsulate the requirements of an outcome our client has defined to be valuable. Multiple user stories will be allocated to a particular project increment/release/milestone (a sprint). A __sprint cycle will be around 3 weeks__, most finishing after each audit. User story maps are used to plan over multiple sprints, where the user stories that are to be completed in the current sprint are moved from the product backlog to the sprint backlog (to-do lists). 

Scrum traditionally includes various statuses to show the progress of individual tasks. We will use:
+ __New issues__: User stories that haven’t been adequately discussed, including effort estimation and acceptance criteria or tasks.
+ __Icebox__: User stories or tasks that are delayed based on low importance or are needing to be reevaluated at regular intervals. This will include risks 
+ __Product backlog__: User stories that have been accepted and sufficiently documented
+ __Sprint Backlog__: User stories that have been scheduled for the current sprint.
+ __In Progress__: User stories that are currently being developed, including testing and docs
+ __Review&Q/A__: User stories that have been completed and need approval from the push master regarding sufficient testing, commenting and quality standards and the client regarding value.
+ __Done__: User stories that have passed all approvals and acceptance criteria
+ __Closed__: User stories which are no longer needing to be tracked, such as ones that have been completed in previous sprints or are no longer needed.

In addition to completion statuses, we will have labels for identifying what the task refers to (some labels are derived from extreme programming concepts). 
These will include:
+ __Documentation__: Any form of documentation
+ __Enhancement__: A new feature proposed by the client
+ __Bug__: A defect in the code or any issue with an output (e.g valid/complete documents)
+ __Testing__: Indicating a test is needed
+ __Question__: A question or clarification directed to be answered over a longer duration
+ __Refactor__: Indicating code is being modified to improve quality
+ __Help Wanted__: Request help for a task
+ __Management__: Any management process, including any process improvements or feedback to action
+ __Risk__: A potential risk for the project

## eXtreme Programming:
Extreme programming is a “__lightweight__” agile methodology that focuses on “taking agile to the extreme”. It is defined by the principles of __simplicity, rapid feedback, quality, collective understanding, iterative development and good work conditions__. It achieves this by __pair programming, test-driven development, constant refactoring and addressing technical debt and on-site customers__. 

As our client is easily accessible we can easily integrate the practice of an on-site customer through __regular communication and developing rapport__. This will enable us to easily adapt to his feedback on a regular basis. We will be utilising __test-driven development__ to the best of our ability with the knowledge that the abstract, black box systems we will be using may impede this. 

We will be utilising __pair programming__ to share __code understanding and promote collaboration__. Each goal will be allocated to __two__ individuals to complete a given task. Once a specific task is complete, the team will reorganise pairs so that one member of each pair remains on a goal until completion (an expert) and the other continues on to another goal (support). This will __promote learning, collaboration and code ownership__. 

XP is not time-boxed like Scrum, so for the purposes of our team, __each week will focus on XP to ease management__. __Pairs will be defined on a weekly basis__ and will focus on one or more components of a particular goal. XP avoids heavy documentation, and we will largely restrict code documentation to informative comments to increase velocity.

# Issue Management:
The emphasis of our processes is on integrating management and development into one platform, which will assist team communication by relating to specific issues. We are using GitHub as our code hosting platform, as it is free to use, has good version control, pipelines, markup capability and support for issue tracking. 

To integrate our management process into the development processes available through GitHub, we are using ZenHub. __ZenHub is a free GitHub addon that appears as an additional tab within a repo__. It has a reasonably clean interface and allows us to achieve all the functionality listed in our project management processes. In particular, it has __superior usability compared to GitHubs more basic projects tab__ and offers additional features including __advanced reporting, planning poker, and advanced issue filters__. These features should make it easier to manage our project, particularly with our project management process. 

### __To use ZenHub, you need to create an account and install the ZenHub chrome extension__. The extension is available at:
https://chrome.google.com/webstore/detail/zenhub-for-github/ogcgkffhplmphkaahpmffcafajaocjbd 

# Risk Management Process:
We will manage risks by __treating them as tasks that need regular attention__ and are hence part of the kanban board to be __reevaluated__ at the beginning of each (3-week) sprint (though unless it becomes an issue, won’t need further effort). This will ensure risks are receiving proper attention. The process is as follows:

1. A risk is discovered
2. A risk task is created under the risks epic
   + Short description
   + Assignee
   + Link to 3.
3. A markdown file is generated addressing that risk
   + Description
   + Relevant stakeholders (and impact)
   + Assignee
   + Trigger (what causes it to become a problem)
   + Symptom/cause
   + Possible Actions
   + Approaches from the hierarchy of control (elimination, substitution, isolation, process)
   + Implications/ new risks
   + Log of decisions (decision, date, who was responsible, monitoring needed)
4. Risk is treated as a task (following general scrum statuses)
5. Once completed, is moved to the icebox if it may need more attention or done if fully resolved

# Change Management Process:
To enable our team to grow and improve our processes, we are using a central location to record feedback and reflection we receive. We will record any feedback that is deemed to __address some aspect of our project in a meaningful way__. Similarly to risks, the process will add management issues to our backlog to ensure they are being actioned. This system will also encompass the decision log by identifying the need for the decision as a reflection. The process is as follows:

1. Feedback received
2. A management task is created under the management epic
   + Short description
   + Who provided it
   + Assignees
   + Link to 3.
3. A markdown file is generated addressing the feedback/reflection
   + Description
   + Who provided it
   + Relevant stakeholders (and impact)
   + Assignees
   + Possible Actions
   + Benefits/detriments
   + Risks created
   + Log of decisions about feedback (decision, date, who was responsible, monitoring needed)
4. Actioning is treated as a task (following general scrum statuses)
5. Once completed, is moved to the done status if fully resolved
# Version control/CI/automated testing:
We plan to utilise test suites to promote code quality and the use of a “push master” role to quality-check that all commits meet our standards. While we plan to improve our performance using pipelines and workflows, this will be determined as we get a better understanding of the project and areas we can improve by incorporating automation and pipelines. 

For VC standards, we will require code pushes to have informative commits about the user story they address, what was completed and any follow-ups needed (e.g potential bugs). This standard is not required for simple document changes.
