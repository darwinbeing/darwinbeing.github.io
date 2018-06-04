---
layout: post
title:  "User Story Guidelines"
permalink: /user-story-guidelines
date:   2018-05-17 00:00:00
author: André Maré
images:
  - assets/images/blog-header/business-man-3-2.jpg
excerpt:
  The goal of user stories is not only to document the requirements, but to deliver working software used by customers in production. User Stories provide a mechanism to document the discussion between the customer and developers w.r.t functionality of the software.

categories: Guidelines
tags: [software engineering, guidelines, user stories]
---


The goal of user stories is not only to document the requirements, but to deliver working software used by customers in production. User Stories provide a mechanism to document the discussion between the customer and developers w.r.t functionality of the software.

##### Definition
"User Stories represent customer requirements in a card, leading to conversations and confirmation." ~ Ron Jeffries

##### Template
The following are well known templates used in defining user stories and acceptance criteria.

<strong>Value Statement:</strong> As a (user role), I want to (activity), so that (business value)

<strong>Acceptance Criteria:</strong> Given (context), when (action performed), then (observable consequences)

##### General Guidelines
The following are some general guidelines to consider when writing user stories:
<ul>
 	<li>User Stories have three aspects: Card, Conversation and Confirmation (Ron Jeffries 2001)</li>
 	<li>User Stories should represent functionality that is of value to users or system owners.</li>
 	<li>User Stories should describe a single feature.</li>
 	<li>User Stories should have a note section where conversations are documented about the user story detail.</li>
 	<li>User Stories should have an estimation (cost) in story points which indicates size and complexity.</li>
 	<li>User Stories should be prioritised according to its value to the customer.</li>
</ul>

##### Attributes of good User Stories (I.N.V.E.S.T)
Mike Cohn specifies six fundamental attributes of a good user story in his book User Stories Applied. These are:

<strong>Independant (I)</strong>
<ul>
 	<li>User Stories should be free of dependencies on other user stories.</li>
 	<li>User Stories should be self-contained.</li>
 	<li>User Stories should be completed and released in any order.</li>
 	<li>User Stories should be combined or split in different ways when dependencies occur.</li>
</ul>
<strong>Negotiable (N)</strong>
<ul>
 	<li>User Stories should not be contractual obligations as they are negotiable.</li>
 	<li>User Stories should be a collaborative negotiation between customers, developers and testers.</li>
</ul>
<strong>Valuable (V)</strong>
<ul>
 	<li>User Stories should be of value to the user or owner of the software.</li>
 	<li>User Stories should not be only of value to developers.</li>
 	<li>User Stories should clearly define the benefit to customers/users to assist in prioritization.</li>
 	<li>User Stories should be written by customers to ensure it is valuable to customers/users.</li>
</ul>
<strong>Estimatable (E)</strong>
<ul>
 	<li>User Stories should be estimated in terms of story points.</li>
 	<li>User Stories should be clearly understood before it is estimated by development teams.</li>
 	<li>User Stories should contain enough detail before it is estimated by development teams.</li>
 	<li>User Stories may not be estimatable when development teams lack domain knowledge.</li>
 	<li>User Stories may not be estimatable when development teams lack technical knowledge.</li>
 	<li>User Stories may not be estimatable when the user story is too big.</li>
</ul>
<strong>Small (S)</strong>
<ul>
 	<li>User Stories should be as small as possible while still providing user value.</li>
 	<li>User Stories should be able to fit into one iteration.</li>
 	<li>User Stories that are to big will be difficult to understand and estimate.</li>
</ul>
<strong>Testable (T)</strong>
<ul>
 	<li>User Stories should be verified by tests to prove they are implemented correctly.</li>
 	<li>User Stories should contain the story acceptance criteria to guide testing.</li>
 	<li>User Stories should be easily unit tested. (Technical Implementation)</li>
 	<li>User Stories should be easily acceptance tested. (Behavioural)</li>
 	<li>User Stories should be tested in an automated manner where possible.</li>
</ul>

##### Story Point Planning
<ul>
 	<li>Fibonacci ( 0, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89, ?, Pass )</li>
 	<li>Modified Fibonacci ( 0, ½, 1, 2, 3, 5, 8, 13, 20, 40, 100, ?, Pass )</li>
 	<li>T-shirts ( xxs, xs, s, m, l, xl, xxl, ?, Pass )</li>
 	<li>Powers of 2 ( 0, 1, 2, 4, 8, 16, 32, 64, ?, Pass )</li>
</ul>

##### Definition of Done (DoD)
There are numerous criteria a team can use to define their Definition of Done. This ensures that teams deliver features that are completed in terms of functionality and quality. Definition of Done is an auditable checklist. The following is a set of possible criteria and activities for a DoD:
<ul>
 	<li>Unit Tests Passed</li>
 	<li>Acceptance Criteria Met</li>
 	<li>Code Reviewed</li>
 	<li>Functional Tests Passed</li>
 	<li>Non-Functoinal Requirements Met</li>
 	<li>Product Owner Accepts User Story</li>
</ul>

##### User Story Example
The following is an example of a user story.

<img src="https://raw.githubusercontent.com/Code2Bits/Software-Engineering-Guidelines/master/images/user_story_example.png" width="640" />

##### Reference
<ul>
 	<li>Cohn, Mike. User Stories Applied: For Agile Software Development. 1st ed., Addison-Wesley Professional, 2004.</li>
 	<li>Wake, William C. Extreme Programming Explored. Addison Wesley, 2002.</li>
</ul>


> One must learn by doing the thing; for though you think you know it, you have no certainty, until you try. ~ Sophocles

[1]: https://www.spectacleapp.com/
[2]: https://brew.sh/
[3]: {{site.url}}/assets/images/cheatsheets/cheatsheet-homebrew.jpg
[4]: {{site.url}}/assets/cheatsheets/cheatsheet-homebrew.pdf
