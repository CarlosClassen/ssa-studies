## Features Overview

This document outlines the key features of the Project Management System, designed to facilitate project creation, team management, project assignment, and project submission.

### 1. Creating Projects

- **Title**: Creating Projects (**MVP**)
- **User Stories**:
    - rofessor logs in to the system and sees all the lectures that he is responsible for.
    - Professor selects one of his lectures and navigates to a page that includes two clickable boxes. Projects and Teams
    - Professor clicks on the projects and sees all of the created projects for the chosen lecture or an info message if no project is created.	
    - Professor clicks on the “Create Project” button and navigates to the page that includes the project creation mask.
    - Professor submits the form with providing necessary information.
        - Project name (mandatory)
        - Deadline (mandatory)
        - Description (optional)
        - Sample solution (optional)
    - System checks the project creation process. A success message is displayed when the project is created, an error message is displayed when one of the mandatory fields is missing or the project name is not unique.

- **Breakdown**:
  - Professor logs in and selects a lecture.
  - Navigates to the project creation interface.
  - Submits a form with project details (name, deadline, etc.).
  - System validates and assigns an ID to the project.
- **Responsibilities**:
  - **Representation**:
    - Correct representation of the projects created
    - Correct visualisation of the project creation form
    - The system correctly notifies the professor about the project creation process

  - **Data Collection**: 
    - Correct fetching of the already created projects in the lecture
    - Correct reading given selection made by professor (All user input in the form)

  - **Data Validation**:
    - Ensures the unique existence of project name
    - Validates that the mandatory fields are filled

  - **Data Assignment**: 
    - Give a valid (unique) identifier for the project
    - Give a creation date for the project when it is successfully created

### 2. Creating Teams

- **Title**: Creating Teams (**MVP**)
- **User Stories**: 
    - Professor logs in to the system and sees all the lectures that he is responsible for.
    - Professor selects one of his lectures and navigates to a page that includes two clickable boxes. Projects and Teams
    - Professor clicks on the teams and sees all of the created teams for the chosen lecture or an info message if no team is created.	
    - Professor clicks on the “Create Team” button and navigates to the page that includes the team creation mask.
    - Team creation mask includes two sections. First one is the name and the second one is the list of the students that are enrolled in the course. Professor gives a unique name to the team and picks at least one student for the team. There is a minimum and a maximum value for the number of students in a team. Professor submits the form with providing necessary information.
    - System checks the team creation process. A success message is displayed when the team is created, an error message is displayed if the number of students is not allowed or the team name is not unique.

- **Breakdown**:
  - Professor accesses team creation interface for a lecture.
  - Inputs team name and selects students.
  - System checks and validates the team creation.
- **Responsibilities**:
  - **Representation**: 
    - Correct representation of the projects created
    - Correct visualisation of the project creation form
    - The system correctly notifies the professor about the project creation process

  - **Data Collection**: F
    - Correct fetching of the already created projects in the lecture
    - Correct reading given selection made by professor (All user input in the form)

  - **Data Validation**: 
    - Ensures the unique existence of project name
    - Validates that the mandatory fields are filled

  - **Data Assignment**: 
    - Give a valid (unique) identifier for the project
    - Give a creation date for the project when it is successfully created


### 3. Assigning Projects to Teams

- **Title**: Assigning Projects to Teams (**MVP**)
- **User Story**: 
    - Professor logs in to the system and sees all the lectures that he is responsible for.
    - Professor selects one of his lectures and navigates to a page that includes two clickable boxes. Projects and Teams
    - Professor clicks on the projects and sees all of the created projects for the chosen lecture or an info message if no project is created.
    - Professor clicks on the assign button in one of the created projects. The assign button is only visible if a project has no team.
    - After clicking the assign button, teams with no projects are displayed. Professor chooses one of the teams and clicks confirm.
    - System checks the assigning process and notifies the professor about the result.

- **Breakdown**:
  - Professor selects a project and assigns it to a team.
  - System validates the assignment process.
- **Responsibilities**:
  - **Representation**:
    - Correct representation of the projects for the given lecture
    - Correct representation of a project with an assigned team and without an assignee (the button next to the team changes accordingly)
    - When clicked on the assign button: Correct representation of teams that have no projects
    - Correctly notifying the professor about the assigning process

  - **Data Collection**: 
    - Correctly fetching the projects and their assignee field for the given lecture
    - Correctly fetching the teams that have no project

  - **Data Validation**:
    - Validates that the project has no assignee
    - Validates that the team has no project

  - **Data Assignment**: 
    - Adds the given team as an assignee field for the given project

### 4. Submitting Projects

- **Title**: Submitting Projects (**MVP**)
- **User Story**: 
    - Student logs in to the system and sees all the lectures that he is enrolled to.
    - Student selects one of his lectures and navigates to a page that includes all of the projects that he is responsible for.
    - Student clicks on the project and navigates to a page that includes project details and a upload button.
    - Student clicks on the upload button and uploads the project file.
    - System checks the uploading project process and notifies the student about the result.

- **Breakdown**:
  - Student selects a project and uploads the file.
  - System checks the upload process and notifies the student.
- **Responsibilities**:
  - **Representation**: 
    - Correct representation of the status of the submission repository
    - Correct representation of the student submit mask
    - Correct representation of the submission history

  - **Data Collection**: 
    - Correctly fetching submission history
    - Persistence of the given GitHub link
    - Correctly fetching the collaborators

  - **Data Validation**: 
    - Validating the consistency of the GitHub link

  - **Data Assignment**: 
    - Assigning new submissions as the latest deliverable

### 5. Notifying Students

- **Title**: Notifying Students
- **User Story**: As a teacher, I want the students to be notified of the assigned projects for their team.

### 6. Messenger Forum

- **Title**: Messenger Forum
- **User Story**: As a student, I would like to communicate with my teammates.
