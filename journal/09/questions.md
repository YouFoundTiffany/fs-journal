# Working in a Professional Environment
01. What is Inheritance?

> Inheritance is the process by which one object can be based on another. This lets the objects to share each other’s properties.


02. What is the `Singleton` design pattern?

> he singleton pattern is one of the simplest design patterns. Sometimes we need to have only one instance of our class for example a single DB connection shared by multiple objects as creating a separate DB connection for every object may be costly. Similarly, there can be a single configuration manager or error manager in an application that handles all problems instead of creating multiple managers. The singleton pattern is a design pattern that restricts the instantiation of a class to one object. Let’s see various design options for implementing such a class. If you have a good handle on static class variables and access modifiers this should not be a difficult task.

03. What is the `Observer` design pattern?

> enables one-to-many data binding between elements. This one-way data binding can be event driven. With this pattern, you can build reusable code that solves for your specific needs.

04. What is the `Strategy` design pattern?

> This pattern enables an object to choose from multiple algorithms and behaviors at runtime, rather than statically choosing a single one.

05. What is the `Factory` design pattern?

> The factory pattern wraps a constructor for different types of objects and returns instances of the objects via a simple API. It makes it easy to create different objects by exposing a simple API that return the specified object type.

06. What is test driven development?

> Test-driven development (TDD) is a software development process relying on software requirements being converted to test cases before software is fully developed, and tracking all software development by repeatedly testing the software against all test cases. This is as opposed to software being developed first and test cases created later.

07. In Scrum/Agile what is the DoD?

> Definition of done (DoD) is crucial to a highly functioning scrum team. The following are characteristics that you should look for in your team’s definition of done. Verifying that your team’s DoD meets these criteria will ensure that you are delivering features that are truly done, not only in terms of functionality but in terms of quality as well.

Definition of Done is a Checklist of Valuable Activities Required to Produce Software
Definition of done is a simple list of activities (writing code, coding comments, unit testing, integration testing, release notes, design documents, etc.) that add verifiable/demonstrable value to the product. Focusing on value-added steps allows the team to focus on what must be completed in order to build software while eliminating wasteful activities that only complicate software development efforts.

Definition of Done is the Primary Reporting Mechanism for Team Members
Reporting in its simplest form is the ability to say, “This feature is done.” After all, a feature or product backlog item is either done or it is not done. DoD is a simple artifact that adds clarity to the “feature is done” statement.  Using the definition of done as a reference for this conversation a team member can effectively update other team members and the product owner.

Definition of Done is Informed by Reality
Scrum asks that teams deliver “increments of value” at the end of every sprint. In reality, many teams are still working towards an increment of value.  Such teams may have a different DoD at various levels:

Definition of done for a feature (story or product backlog item)
Definition of done for a sprint (collection of features developed within a sprint)
Definition of done for a releasable increment
There are various factors that influence whether a given activity belongs in the DoD for a feature, a sprint or a release. Ultimately, the decision rests on the answer to the following three questions:

Can we do this activity for each feature? If not, then
Can we do this activity for each sprint? If not, then
We have to do this activity for our release!
Certified Scrum Trainer Chris Sterling recommends that for activities that cannot be included for a sprint/feature, teams should, “Discuss all of the obstacles which stop them from delivering this each iteration/sprint.”

Common root causes for impediments include:

Team does not have the skillset to incorporate activities into the definition of done for a sprint or for a feature.
Team does not have the right set of tools. (Example: continuous integration environment, automated build, servers etc.)
Team members are executing their sprint in mini-waterfalls.

* Aha! Here’s an opportunity to be more cross-functional and share responsibilities across functional silos.
Definition of Done is Not Static
The DoD changes over time. Organizational support and the team’s ability to remove impediments may enable the inclusion of additional activities into the DoD for features or sprints.

Definition of Done is an Auditable Checklist
Features/stories are broken down into tasks both during sprint planning and also within a sprint. The DoD is used to validate whether all major tasks are accounted for (hours remaining). Also, after a feature or sprint is done, DoD is used as a checklist to verify whether all necessary value-added activities were completed.

It is important to note that the generic nature of the definition of done has some limitations. Not all value-added activities will be applicable to each feature since the definition of done is intended to be a comprehensive checklist. The team has to consciously decide the applicability of value-added activities on a feature-by-feature basis. For example, following user experience guidelines for a feature that provides integration point (eg. web service) to another system is not applicable to that particular feature; however, for other features within the system that do interface with a human being, those user experience guidelines must be followed.

Summary
The definition of done is orthogonal to user acceptance criteria (functional acceptance) for a feature. It is a comprehensive checklist of necessary, value-added activities that assert the quality of a feature and not the functionality of that feature. Definition of done is informed by reality where it captures activities that can be realistically committed by the team to be completed at each level (feature, sprint, release).

08. Give two examples of a user story:

> When I want to log in to the Geo-STache web app I would like to be able to search for other users that comment on my Created STaches and interact with them, see what they have created, what other comments they have made and what other Staches they found.

"As a user, I should be able to see all of the snacks images and prices upon page load."

09. During which ceremony is your Sprint Backlog created?

> refinement meeting

10. In which of these ceremonies are Tasks assigned to you?

> In scrum, a developer is not assigned a task, they volunteer.
