# Ocular Disease Identifier Planning & Documentation 

## Table of Contents
  * [:bulb: Project Description](#bulb-project-description)
  * [:compass: Implementation Plan](#compass-implementation-plan)
  * [:clipboard: Team Management](#clipboard-team-management)
  * [:athletic_shoe: Sprint Planning](#athletic_shoe-sprint-planning)

## :bulb: Project Description

Did you know that over 30% of Canadians over the age of 65 suffer from ocular diseases such as glaucoma, cataracts, and diabetic retinopathy [1]? Unfortunately, many cases go undiagnosed since it is difficult for optometrists to detect them, particularly in their early stages. Although these diseases are more prevalent in the elderly community, they affect people of all demographics and ages. When left untreated, symptoms of eye disease can quickly worsen, potentially leading to blindness. But what if there were a way to change this? Imagine if we could use machine learning to combat this issue by creating a tool that could help identify these diseases.

The goal of the ocular disease identifier is to both detect any symptoms of ocular disease that go unnoticed during examination, and be able to offer a valid second opinion. This project does not aim to replace professional eye examinations, but is rather meant to act as a failsafe mechanism that accounts for human error. To ensure real world usability, the identifier should be quick, simple to use, and store any patient information securely and in compliance with standard privacy policies.

### Objectives
1. Build and train an AI model to identify ocular diseases using patient fundus images (see Figure 1 below).
2. Develop a secure web application that allows Opthamologists to efficiently access the AI model.

![Figure 1](images/Figure1.png)
<p align="center"><em>Figure 1: High Level Overview of Project Back-End.</em></p>

### Stakeholders

- Opthamologists
- Undiagnosed ocular disease patients


## :compass: Implementation Plan

### Project Timeline


- **Milestone 1 (MVP):** Overview of backend minimum viable product requirements. Build a convolutional neural network (CNN) using TensorFlow. Train the model using a public dataset, such as the following [Kaggle Dataset](https://www.kaggle.com/datasets/andrewmvd/ocular-disease-recognition-odir5k). The model should be functioning for ***only one*** ocular disease (Ex. Glaucoma) at this point.
Date to be completed by: *TBD*
- **Milestone 2 (MVP):** Overview of frontend minimum viable product requirements. Develop an API using a python framework (Ex. Flask, Django, etc.). Develop a user-friendly, and aesthetically pleasing web application that is able to handle requests to the API. The frontend application must be able to accept image files and submit them to the API.
Date to be completed by: *TBD*
- **Milestone 3:** Increase the number of diseases that the model can identify. Analyze potential weaknesses of the model, and modify accordingly to increase overall accuracy. Increase functionality of the web application; implement additional features such as ability to login, drag and drop file upload, and possibly storing of patient information. Note: This would require a database. Date to be completed by: *TBD*
- **Milestone 4:** Implement additional image processing, so that the model will inform the user of the location of the disease (See Figure 2). Host and deploy the application. Date to be completed by: *TBD*

### Tech Stack
*Note: The project is ***not*** limited to the technologies listed below!*

- **Frontend Framework Options:**
  - Web Application: ![React](https://img.shields.io/badge/React-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB) ![Angular](https://img.shields.io/badge/Angular-%23DD0031.svg?style=for-the-badge&logo=angular&logoColor=white) ![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
  - API:  ![Flask](https://img.shields.io/badge/Flask-%23000.svg?style=for-the-badge&logo=flask&logoColor=white) ![Django](https://img.shields.io/badge/Django-%23092E20.svg?style=for-the-badge&logo=django&logoColor=white) ![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi)

- **Backend Framework:**
  ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-%23white.svg?style=for-the-badge&logo=opencv&logoColor=white)

- **Other Technologies/Libraries:**
  - Data Processing: ![Pandas](https://img.shields.io/badge/Pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)

  - Hosting & Deployment Tools: ![GKE](https://img.shields.io/badge/GKE-%233498DB.svg?style=for-the-badge&logo=google-cloud&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white) ![Google Cloud](https://img.shields.io/badge/Google%20Cloud-%234285F4.svg?style=for-the-badge&logo=google-cloud&logoColor=white)


  - Styling Options: ![Bootstrap](https://img.shields.io/badge/Bootstrap-%23563D7C.svg?style=for-the-badge&logo=bootstrap&logoColor=white) ![TailwindCSS](https://img.shields.io/badge/TailwindCSS-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white) ![Figma](https://img.shields.io/badge/Figma-%23F24E1E.svg?style=for-the-badge&logo=figma&logoColor=white) ![Canva](https://img.shields.io/badge/Canva-%2300C4CC.svg?style=for-the-badge&logo=Canva&logoColor=white)



### Project Structure 
Backend devs will work in the backend directory in which the model will be developed. The model will then be integrated into the API directory that will be developed by the frontend devs. The frontend can then access the model through the API, and receive a response accordingly. 

![Figure 3](images/Figure3.png)
<p align="center"><em>Figure 3: Potential Structure of Project.</em></p>


  
### Testing & CI/CD
*Your project should have a formal testing plan that will complement the code acceptance of each pull request. The tests themselves may be written by your devs, but you should try to define a plan/framework for how they should write/execute their tests. It be great if you could integrate automated testing and deployment, but manual testing works as well. Describe the test plans, metrics/measures you'll use such as coverage, and tools such as specific testing frameworks that match your tech stack, automation tools like GitHub Actions, Jenkins, etc.*


## :clipboard: Team Management

### Team Members

- **Scrum Master & Product Owner:** [Kristian Diana]
- **Frontend Developers (2):**
  - [Name]
  - [Name]
- **Backend Developers (3):**
  - [Name]
  - [Name]
  - [Name]

  


### Team Communication

- **Communication Platform:** Discord
- **Meeting Schedule:**
  - Sprint Review: [Time and Weekly]
  - Sprint Retrospective: [Time and TBD]
  - Other Meetings: [Potential for in-person coding sessions depending on team availability]

### Roles and Responsibilities
*This section defines the responsibility of each role, you may edit to fit your project's needs.*

- **Scrum Master:**
  - Flush out project's boilerplate 
  - Assign tickets to developers
  - Facilitate scrum ceremonies (sprint reviews, retrospectives)
  - Remove impediments
- **Product Owner:**
  - Define product backlog 
  - Prioritize user stories
  - Accept/reject deliverables
- **Developers:**
  - Develop features through ticket completion
  - Create test cases to for feature/ticket acceptance
  - Thoroughly document code and features through pull requests and README docs
  - Execute tests
  - Report defects

### Collaboration Tools
We will be using Monday.com as a way to organize our project as use of this system will make it easy for us to adhere to the Scrum framework. We will use a Kanban Board style system which will allow sprint progress to be easily monitored. Tickets (tasks) will be assigned to members, and are expected to be completed by a designated due date. 

### Code Acceptance: The Definition of Done

Below we define the Definition of Done for this project, i.e. what needs to the included in a pull request for the pull request to be accepted by the Product Owner:
- Code Complete (satisfies feature associated to the ticket)
- Passed Code Review by Scrum Master
- Passed Unit Tests/Other testing developed for the feature
- Documentation Updated (Sufficient Commenting)
- Ready to be integrated with Main Branch (no merge conflicts)



## :athletic_shoe: Sprint Planning
### High Level Goals for Each Sprint
*This section is meant to facilitate your future sprint planning, and allow you to estimate a more detailed project timeline. For each milestone you defined, break it up into 2-4 sprints, and describe the goals as well as expected duration for each sprint.*

#### <u>Milestone 1</u>

**Sprint 1**: [Description of what features will be achieved by the end of this sprint], [Expected length of sprint in weeks (Should be 1-2 weeks)]. 

**Sprint 2**: ...
 
#### <u>Milestone 2</u>

**Sprint 3**: ... 

...

### Sprint Planning 
*Below is a template for sprint planning for your future use. You can follow it as much as you'd like, so long as you're able to generate reasonably sized tickets for your members each sprint, and said tickets will bring you to your milestones by the target date you declared.*

*Some more resources for sprint Planning:*
- *[Atlassian: Sprint Planning](https://www.atlassian.com/agile/scrum/sprint-planning#:~:text=What%20is%20sprint%20planning%3F,with%20the%20whole%20scrum%20team.)*
- *[Scrum in 20 mins](https://www.youtube.com/watch?v=SWDhGSZNF9M&ab_channel=CodexCommunity)*

#### Sprint Duration
- _Sprint Length:_ [e.g., 2 weeks]
- _Start Date:_ [Date]
- _End Date:_ [Date]

#### High Level Sprint Goals
1. Goal 1
2. Goal 2
3. Goal 3

#### User Stories (Sample)

| ID   | User Story                                  | Priority | Story Points | Assignee |
|------|---------------------------------------------|----------|--------------|----------|
| US01 | As a [user role], I want to [feature]       | High     | 5            | Dev A    |
| US02 | As a [user role], I want to [feature]       | Medium   | 3            | Dev B    |
| US03 | As a [user role], I want to [feature]       | Low      | 2            | Dev C    |
