User Story Template
This template integrates the core concepts of user-centric design (As a..., I want..., so that...), the I.N.V.E.S.T. criteria, and a comprehensive structure for technical and testing requirements.

User Story Title:
A brief, descriptive title. Example: "Export Access Log Data as CSV"



1. User Persona & Goal (Who, What, Why)
This section frames the story from the user's perspective, establishing the core value proposition.

WHO (User Persona): As a...

Describe the user role. Who are they? What is their relationship to the product? Example: "As a community manager with access to the portal..."

WHAT (Action): I want to...

Describe the action or feature they need. Example: "...export access log data from the access log page in CSV format, applying any current filters..."

WHY (Value): So that I can...

Describe the goal or benefit the user achieves. This is the value proposition. Example: "...analyze access patterns offline, create reports for property management, or maintain records for compliance purposes."



2. I.N.V.E.S.T. Checklist
Use this checklist to ensure the story is well-formed and ready for a sprint.

[ ] Independent: Can this story be completed without depending on another story?

[ ] Negotiable: Is there room for discussion on the details of implementation?

[ ] Valuable: Does this deliver clear value to the end-user or customer?

[ ] Estimable: Is the scope clear enough for the team to estimate the effort?

[ ] Small: Can this story be completed within a single sprint?

[ ] Testable: Are there clear criteria to confirm this story is done?



3. Acceptance Criteria (AC)
This is the "Testable" component of I.N.V.E.S.T. Describe specific, testable scenarios using the Gherkin Given-When-Then format. Cover happy paths, edge cases, and error handling.

✓ Scenario 1: [Name of Scenario]

Given: [The initial context or state before the action.]
When: [The specific action taken by the user.]
Then: [The expected outcome or system response.]

✓ Scenario 2: [Name of Scenario]

Given: [Context...]
When: [Action...]
Then: [Outcome...]

✓ Scenario 3: Error Handling

Given: [A specific pre-condition for an error.]
When: [An action is performed that will result in an error.]
Then: [The system should respond with a specific error message or state.]



4. Non-Functional Requirements (NFRs)
Define the quality attributes and constraints of the system. These are not what the system does, but how it does it.

Performance:

e.g., Page load times, API response times, thresholds for background processing.

Security:

e.g., Authentication, authorization, data encryption, specific link security (time-limited, private).

Usability:

e.g., UI/UX guidelines, feedback mechanisms (loading indicators, success/error messages).

Data Integrity:

e.g., Data sources, formatting rules, naming conventions.



5. Technical Implementation Notes (Optional)
Provide guidance or suggestions for the development team. This is a collaborative section and can be updated by the team.

API Endpoints:

e.g., New or modified endpoints, request/response structure.

Data Model / Schema:

e.g., Changes to database collections or tables.

System Integration:

e.g., Notes on interacting with other services like S3, email servers, background job systems.

Key Algorithms:

e.g., Logic for estimations, calculations, or processing.



6. Dependencies
List any other stories, technical components, or external factors that must be in place for this story to be completed.

e.g., Requires user authentication system to be complete.

e.g., Dependent on S3 bucket configuration.

e.g., Awaiting final UI mockups from the design team.



7. Definition of Done (DoD)
This is the final, high-level checklist agreed upon by the team. A story is only "Done" when every item here is checked off.

[ ] All Acceptance Criteria have passed.

[ ] Code is peer-reviewed and merged to the main branch.

[ ] Unit and integration tests are written and passing.

[ ] NFRs have been met.

[ ] Any required documentation (for support, end-users, etc.) is created/updated.

[ ] The Product Owner has reviewed and approved the feature.

AI Prompt to Generate a User Story
You can use the following prompt with an AI assistant to automatically generate a comprehensive user story based on the template above. Just copy the text below and replace the bracketed information with your feature details.

Markdown

As a product development AI assistant, please generate a complete user story using the provided template.

**My Feature Idea:**
[Describe your feature in 1-3 sentences. For example: "I want users to be able to reset their password if they forget it. They should get an email with a secure link that expires after a certain time."]

**Target User Persona:**
[Describe the user who will use this feature. For example: "Any registered user of our web application."]

**Instructions for the AI:**
Based on my feature idea and target user, please generate a complete user story. Fill out all the following sections in detail:

1.  **User Story Title:** A short, descriptive title.
2.  **User Persona & Goal (WHO, WHAT, WHY):** Create the "As a..., I want..., so that..." statement.
3.  **I.N.V.E.S.T. Checklist:** Leave this as a checklist for the team to fill out.
4.  **Acceptance Criteria (AC):** Write at least three detailed scenarios using the `Given/When/Then` format. Include a "happy path" scenario, a scenario for what happens after the main action (e.g., clicking the reset link), and an error handling scenario (e.g., using an expired link).
5.  **Non-Functional Requirements (NFRs):** Detail requirements for Performance (how fast the email sends), Security (link expiration, secure token), and Usability (clear instructions in the email).
6.  **Technical Implementation Notes:** Suggest potential technical details, such as the need for a new API endpoint (`/request-password-reset`), the data model for the reset token (token, userId, expiration timestamp), and integration with an email service.
7.  **Dependencies:** List potential dependencies, like the email sending service.
8.  **Definition of Done (DoD):** Provide a standard, high-level checklist for when the story is truly complete.

Please format the entire output in Markdown.
