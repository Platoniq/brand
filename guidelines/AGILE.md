
Here are three simple truths about ~~software development~~ life:

🌑 You can’t gather all the requirements up front.

🌓  The requirements you do gather will change.

🌝 There is always more to do than time and money will allow.


# How to be agile

## Kick-off meeting

Its goals are:

- 👀 An overview of the project and the goals
- 👪 Who will be working on the project
- 📄 Determining the point person for client sign-off
- 🏗️ Creating the project backlog
- ⛏️ Determining which features to work on
- 🌐 Getting on the same page


## Create the Project Backlog

Behind every project is a project backlog. The project backlog is a list of all the product features generally defined by “user stories”. User stories define everything potential users want to do on the site. They are defined for each of the user groups on the site and are structured like:

> AS A _type of user_ 💁
>
> I WANT TO _do this thing_ 🔧
>
> SO THAT I CAN _accomplish this goal_ 🏆

### 💁 **Role** - The user should be an actual human who interacts with the system.
  - Be as specific as possible
  - The development team is NOT a user
  - _The role represents the person, system, subsystem or any entity who will interact with the system to achieve a goal. They will gain values by interacting with the system._

### 🔧 **Action** - The behavior of the system should be written as an action.
  - Usually unique for each User Story
  - The "system" is implied and does not get written in the story
  - Active voice, not passive voice ("I can be notified")
  - _Represents a user's expectation that can be accomplished through interacting with the system._

### 🏆 **Benefits** - The benefit should be a real-world result that is non-functional or external to the system. 
- Many stories may share the same benefit statement.
- The benefit may be for other users or customers, not just for the user in the story.
- _Represents the value behind the interaction with the system._

### User Story Examples:

> A)
>
> As a **customer**,
>
> I want **shopping cart feature**
>
> so that **I can easily purchase items online**.

> B)
>
> As an **manager**
>
> I want to **generate a report**
>
> so that **I can understand which departments need more resources**.

> C)
>
> As a **customer**
>
> I want to **receive an SMS when the item is arrived**
>
> so that **I can go pick it up right away**


**It's important that the backlog is always accessible and easy to track (We use Github issues and projects to accomplish this).**

One of the best ways to create the initial project backlog is to write all of the user stories on post it notes during the kick-off meeting.

### Detailing User Stories with the 3 C's (Card, Conversation and Confirmation)

#### Card
- Represents 2-3 sentences used to describe the intent of the story that can be considered as an invitation to conversation
- Summarizes intent and represents a more detailed requirement, whose details remain to be determined
- The written text must address the "who (role)", "what (action)" and "why (benefits)" of the story.

#### Conversation

- Represents a discussion between the target users, team, product owner, and other stakeholders, which is necessary to determine the more detailed behavior required to implement the intent
- Represents a "promise for a conversation" about the intent
- The conversation is where the real value of the story lies and the written Card should be adjusted to reflect the current shared understanding of this conversation.
- This conversation is mostly verbal but most often supported by documentation and ideally automated tests of various sorts (e.g. Acceptance Tests).

## Rank user stories

After the user stories have been dreamed up, they are ranked in order of priority. Part of this ranking is also grouping stories together. Some stories will naturally lend themselves to being built with others, which will expedite the process. 

The project backlog is always fluid and never locked in. The project lead will be in charge of reprioritizing the backlog between sprints. And if new features are dreamed up or requested by users, they are encouraged to be added to the backlog. The one exception to the fluid backlog is during a sprint. While the sprint is in session, it is important to not add features. That keeps the team focused and makes sure that the project can be properly tracked.


## Estimate the user stories

Features are rated on a 1️⃣, 2️⃣ or 3️⃣ point scale. More precise estimation is more challenging and ends up less accurate. It is easy to compare things relatively on a scale of 3. And if something is particularly challenging that you don’t think it fits within the “3️⃣ point” bucket, it should be broken down into smaller features that can each fit into the respective buckets 🪣🪣🪣. 

It’s also important to determine the sprint velocity of the team working on the project. That is how many “points” the team can complete per sprint. This velocity is averaged over time. And in typical average time value- the more sprints you do, the estimates and velocity become more and more accurate. That is to say that in some sprints you may not hit your goal number and other sprints you may exceed it. Over the course of a standard project, this averages out. 


## Sprints => How to adapt this to the way we work?

📅 Agile projects are broken down into small, consistent time intervals. These intervals are referred to as sprints. They can be as short as a few days and generally are no longer than 3 - 4 weeks. During a sprint there is a dedicated team that includes designers, developers and business people working together.



## Sources 🔎

- https://pragprog.com/titles/jtrap/the-agile-samurai
- https://www.visual-paradigm.com/guide/agile-software-development/what-is-user-story/
- http://agilehandbook.com/agile-handbook.pdf
