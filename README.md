<span id="23-de-fevereiro">
<img width="1800" height="526" alt="image" src="https://github.com/user-attachments/assets/9c2f315d-9621-4fed-be78-2aaac163f5b7" />

<p align="center">
    <a href="#introduction">Introduction</a> |
    <a href="#challenge">Challenge</a> |  
    <a href="#solution">Solution</a> |   
    <a href="#product-backlog">Product Backlog</a> |
    <a href="#project-evolution-timeline">Project Evolution Timeline</a> |
    <a href="#sprint-timeline">Sprint Timeline</a> |
    <a href="#technologies">Technologies</a> |
    <a href="#project-structure">Project Structure</a> |
    <a href="#run-use-and-test-the-project">Run, Use and Test the Project</a> |
    <a href="#documentation">Documentation</a> |
    <a href="#team">Team</a>
</p>

<span id="introduction">
    
## 📍 Introduction
This project was developed by the **23 de fevereiro** group, composed of students from the 5th semester of the `Banco de Dados` course at Fatec São José dos Campos.

The goal is to create `Lunae`, an extraction, data processing, and analytical visualization tool integrated with the databases of the partner company SIATT, focused on creating dashboards from the information the company possesses. Lunae will enable managers to perform historical and strategic analyses, generating relevant indicators for program and project management.

### SIATT: The Client Company
This project is a solution designed for SIATT – **Sistemas Integrados de Alto Teor Tecnológico (High Technology Integrated Systems)**, a Brazilian company founded in 2015 and headquartered in the São José dos Campos Technology Park (SP). Specializing in the development and integration of high-tech systems for the defense and aerospace sectors, the company focuses on creating advanced solutions such as missiles and smart weapons, guidance and navigation systems, radars, avionics, and communication and control systems. With a team predominantly composed of engineers and specialists, SIATT participates in strategic projects for the Brazilian Armed Forces, including the development of MANSUP (National Anti-Ship Missile), in addition to collaborating on technological initiatives focused on security, monitoring, and communication in complex environments.

---

<span id="challenge">

## 🧩 Challenge

<details>

<summary>Click here</summary>
<br>
The company develops strategic projects organized into institutional programs, involving engineering activities, material acquisition, and specialized technical task execution.
<br>
<br>
Currently, information related to purchase requests, orders, material commitments, inventory control, development tasks, and hours worked are distributed across different tables and systems, lacking a consolidated analytical view. <br> <br> The absence of data integration hinders the analysis of the actual cost of projects, comparison between programs, and the tracking of material consumption and technical hours over time. Project managers and those responsible for financial monitoring face difficulties in answering questions such as: how much did each project consume in materials? What is the total cost of technical hours? What is the actual cost of the product considering materials and development effort?
<br>
<br>
The challenge lies in designing and implementing an analytical environment capable of integrating information from project, procurement, and development areas, structuring the data appropriately to support historical and strategic analyses. The solution should allow multidimensional exploration of information, enabling the generation of relevant indicators for program and project management.
<br>
<br>
The detailing of business rules, definition of metrics, consolidation criteria, and prioritization of analyses must be built by the students together with the partner throughout the project, through interactions via Slack, following the incremental approach of the adopted agile methodology.

</details>

→ <a href="#23-de-fevereiro">Back to top</a>

---

<span id="solution">

## 🏅 Solution

<details>

<summary>Click here</summary>
<br>
Lunae is an analytical platform that integrates data from tasks, projects, programs, purchases, and hours worked, consolidating information that is currently scattered across different systems and tables. Through the import of CSV files provided by the partner, the data is processed, treated, and stored in a structured database, enabling precise analytical queries.
<br>
<br>
The solution provides an interactive dashboard with bar and line charts that allow managers to track resource consumption, cost evolution, and technical effort by project and program, as well as apply filters to explore different scenarios. With this, Lunae offers a consolidated and multidimensional view, supporting decision-making and strategic management of the company's institutional programs.

</details>

→ <a href="#23-de-fevereiro">Back to top</a>

---

<span id="product-backlog">

## 📋 Product Backlog

Rank | Priority | User Story | Story Points | Sprint | Client Requirement
-- | -- | -- | -- | -- | --
1 | 🔴 High | As a project manager, I want to view a bar chart of hours worked per employee to understand the team's effort distribution, separated by project | 8 | 1 | [CR05](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/3.-Documenta%C3%A7%C3%A3o-de-Produto#requisitos-funcionais)/[CR07](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/3.-Documenta%C3%A7%C3%A3o-de-Produto#requisitos-funcionais)
2 | 🔴 High | As a manager, I want to filter a specific project and view summary indicators like total cost and total time to quickly understand its overall status | 3 | 1 | [CR11](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/3.-Documenta%C3%A7%C3%A3o-de-Produto#requisitos-funcionais)/[CR12](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/3.-Documenta%C3%A7%C3%A3o-de-Produto#requisitos-funcionais)
3 | 🔴 High | As a manager, I want to view the evolution of hours worked per project over time in a multi-line chart to track activity progress | 8 | 1 | [CR05](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/3.-Documenta%C3%A7%C3%A3o-de-Produto#requisitos-funcionais)/[CR08](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/3.-Documenta%C3%A7%C3%A3o-de-Produto#requisitos-funcionais)
4 | 🔴 High | As a manager, I want to view the evolution of costs per project over time in a multi-line chart to track spending growth | 8 | 1 | [CR06](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/3.-Documenta%C3%A7%C3%A3o-de-Produto#requisitos-funcionais)/[CR09](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/3.-Documenta%C3%A7%C3%A3o-de-Produto#requisitos-funcionais)
5 | 🔴 High | As a manager, I want to view the cost invested in each material through a materials table to assess the financial impact of projects | 3 | 1 | [CR06](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/3.-Documenta%C3%A7%C3%A3o-de-Produto#requisitos-funcionais)
6 | 🟡 Medium | As a manager, I want to view the evolution of hours worked per program over time to track aggregate effort at a strategic level | 8 | 2 | [CR05](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/3.-Documenta%C3%A7%C3%A3o-de-Produto#requisitos-funcionais)/[CR10](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/3.-Documenta%C3%A7%C3%A3o-de-Produto#requisitos-funcionais)
7 | 🟡 Medium | As a manager, I want to view the evolution of costs per program over time to analyze the financial behavior of programs | 8 | 2 |[CR06](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/3.-Documenta%C3%A7%C3%A3o-de-Produto#requisitos-funcionais)/[CR10](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/3.-Documenta%C3%A7%C3%A3o-de-Produto#requisitos-funcionais)
8 | 🟡 Medium | As a manager, I want to filter a specific program and view summary indicators such as estimated cost, actual cost, estimated hours, actual hours, and total number of projects in the program to quickly understand its overall status | 5 | 2 | [CR06](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/3.-Documenta%C3%A7%C3%A3o-de-Produto#requisitos-funcionais)/[CR10](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/3.-Documenta%C3%A7%C3%A3o-de-Produto#requisitos-funcionais)/[CR12](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/3.-Documenta%C3%A7%C3%A3o-de-Produto#requisitos-funcionais)
9 | 🟡 Medium | As a manager, I want to view a bar chart of hours worked per program to compare effort across different projects | 5 | 2 | [CR05](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/3.-Documenta%C3%A7%C3%A3o-de-Produto#requisitos-funcionais)/[CR10](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/3.-Documenta%C3%A7%C3%A3o-de-Produto#requisitos-funcionais)/[CR12](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/3.-Documenta%C3%A7%C3%A3o-de-Produto#requisitos-funcionais)
10 | 🟡 Medium | As a manager, I want to view the distribution of project statuses for a program in a donut chart to quickly understand the progress of initiatives | 5 | 2 | [CR05](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/3.-Documenta%C3%A7%C3%A3o-de-Produto#requisitos-funcionais)/[CR06](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/3.-Documenta%C3%A7%C3%A3o-de-Produto#requisitos-funcionais)/[CR10](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/3.-Documenta%C3%A7%C3%A3o-de-Produto#requisitos-funcionais)
11 | 🟡 Medium | As a manager, I want to navigate between program and project views directly from the dashboards to explore data from the strategic to operational level | 5 | 2 | [CR11](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/3.-Documenta%C3%A7%C3%A3o-de-Produto#requisitos-funcionais)/[CR13](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/3.-Documenta%C3%A7%C3%A3o-de-Produto#requisitos-funcionais)
12 | 🟡 Medium | As a manager, I want to view a table of projects with hour deviations containing information such as estimated hours, actual hours, task progress, and deviation to identify projects that need attention | 8 | 2 | [CR05](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/3.-Documenta%C3%A7%C3%A3o-de-Produto#requisitos-funcionais)/[CR11](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/3.-Documenta%C3%A7%C3%A3o-de-Produto#requisitos-funcionais)/[CR12](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/3.-Documenta%C3%A7%C3%A3o-de-Produto#requisitos-funcionais)
13 | 🟡 Medium | As a manager, I want to view material consumption per project over time in a depletion chart to understand how physical resources are used in projects | 5 | 3 | [CR06](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/3.-Documenta%C3%A7%C3%A3o-de-Produto#requisitos-funcionais)/[CR11](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/3.-Documenta%C3%A7%C3%A3o-de-Produto#requisitos-funcionais)
14 | 🔴 High | As a manager, I want to identify materials with insufficient stock through alert cards showing the most critical materials for project execution to anticipate the need for new purchases | 8 | 3 | [CR11](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/3.-Documenta%C3%A7%C3%A3o-de-Produto#requisitos-funcionais)
15 | 🔴 High | As a manager, I want to view the deadline for placing a purchase request based on projected consumption and material lead time to avoid project delays | 8 | 3 | [CR06](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/3.-Documenta%C3%A7%C3%A3o-de-Produto#requisitos-funcionais)/[CR11](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/3.-Documenta%C3%A7%C3%A3o-de-Produto#requisitos-funcionais)
16 | 🟢 Low | As a manager, I want to export dashboard information in formats like CSV or Excel to share analyses with other areas of the organization | 3 | 3 | [CR11](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/3.-Documenta%C3%A7%C3%A3o-de-Produto#requisitos-funcionais)/[CR13](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/3.-Documenta%C3%A7%C3%A3o-de-Produto#requisitos-funcionais)

→ <a href="#23-de-fevereiro">Back to top</a>

---

<span id="project-evolution-timeline">
    
## ⏱️ Project Evolution Timeline

| Etapa            | Kick-Off | Sprint 1 | Sprint 2 | Sprint 3 |
| ---------------- | -------- | -------- | -------- | -------- |
| Planning         | ████████ | ████████ | ████     |          |
| DW Modeling      | ████████ | ██       |          |          |
| Backend (Django) |          | ████████ | ████████ | ████████ |
| Frontend (Vue)   |          | ████████ | ████████ | ████████ |
| Dashboards       |          | ████████ | ████████ | ████████ |
| Testing          |          | ████████ | ████████ | ████████ |

→ <a href="#23-de-fevereiro">Back to top</a>

---

<span id="sprint-timeline">
    
## 📅 Sprint Timeline

| Sprint | Start | End | History | Delivery |
|-|-|-|-|-|
| Kick off | 02/03/2026 | 15/03/2026 | --- | --- |
| SPRINT 1 | 16/03/2026 | 05/04/2026 | [Sprint 1 Docs](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/5.-Documenta%C3%A7%C3%A3o-das-Sprints#sprint-1) | [Vídeo - TODO]() |
| SPRINT 2 | 13/04/2026 | 03/05/2026 | [Sprint 2 Docs](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/5.-Documenta%C3%A7%C3%A3o-das-Sprints#sprint-2) | [Vídeo - TODO]() |
| SPRINT 3 | 11/05/2026 | 31/05/2026 | [Sprint 3 Docs](https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki/5.-Documenta%C3%A7%C3%A3o-das-Sprints#sprint-3) | [Vídeo - TODO]() |
| Solutions Fair | 11/06/2026 | --- | --- | --- |

→ <a href="#23-de-fevereiro">Back to top</a>

---

<span id="technologies">

## 💻 Technologies

<p align="center">
  <img src="https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vuedotjs&logoColor=4FC08D" />
  <img src="https://img.shields.io/badge/django-%23092E20.svg?style=for-the-badge&logo=django&logoColor=white" />
  <img src="https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white" />
  <img src="https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white" />
  <img src="https://img.shields.io/badge/Slack-4A154B?style=for-the-badge&logo=slack&logoColor=white" />
  <img src="https://img.shields.io/badge/VS_Code-CED4DA?style=for-the-badge&logo=visual-studio-code&logoColor=0078D4" />
  <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" />
  <img src="https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=swagger&logoColor=black" />
</p>

→ <a href="#23-de-fevereiro">Back to top</a>

---

<span id="project-structure">
    
## 🗂️ Project Structure

TODO

→ <a href="#23-de-fevereiro">Back to top</a>

---

<span id="run-use-and-test-the-project">
    
## 🚀 Run, Use and Test the Project

TODO

→ <a href="#23-de-fevereiro">Back to top</a>

---

<span id="documentation">

## 📚 Documentation

<a href="https://www.figma.com/design/UGtbRBRk3JZqQ7Vx9TMAQ8/API-5-Sem?node-id=0-1&p=f&t=2RMKV3keLHuhPPgL-0">Wireframe</a>

<a href="https://github.com/23deFevereiro/FATEC-API-5-Semestre/wiki">Documentation</a>

→ <a href="#23-de-fevereiro">Back to top</a>

---

<span id="team">

## :busts_in_silhouette: Team

<div align="center">

| Name | Role | Networking | Identification |
|---|---|---|---|
| Augusto Piatto | Product Owner | [![Linkedin](https://img.shields.io/badge/Linkedin-blue?logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/augusto-piatto/) [![GitHub](https://img.shields.io/badge/GitHub-111217?logo=github&logoColor=white)](https://github.com/augustopiatto) | <img src="https://media.licdn.com/dms/image/v2/D4D03AQHIufwtUAtP-g/profile-displayphoto-shrink_800_800/B4DZTbun62HAAg-/0/1738853220594?e=1774483200&v=beta&t=3HthESSDspBYXny1gmIWKqkbhdxXaLLZe_UnTdCidng" width="60"> |
| Davi Soares | Scrum Master | [![Linkedin](https://img.shields.io/badge/Linkedin-blue?logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/dsf21/) [![Github](https://img.shields.io/badge/GitHub-111217?logo=github&logoColor=white)](https://github.com/DaviSFS21) | <img src="https://media.licdn.com/dms/image/v2/D5603AQH4Mq-L9oCcvQ/profile-displayphoto-crop_800_800/B56ZlN660SIsAI-/0/1757948918646?e=1774483200&v=beta&t=LtvBfkP3zSOK9FI9lFlSDA6BNhOMU4pn0wfoAXT0taw" width="60"> |
| João Paulista | Dev Team | [![Linkedin](https://img.shields.io/badge/Linkedin-blue?logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/joaopaulista/) [![Github](https://img.shields.io/badge/GitHub-111217?logo=github&logoColor=white)](https://github.com/joaopaulista) | <img src="https://media.licdn.com/dms/image/v2/D4E03AQHC8f40eim1BA/profile-displayphoto-shrink_800_800/profile-displayphoto-shrink_800_800/0/1727891030117?e=1774483200&v=beta&t=lUqkcfaiVL7nnI_lQQv-LacAhXSHAnGYpSZAuWyGMvc" width="60"> |
| João Ventura | Dev Team | [![Linkedin](https://img.shields.io/badge/Linkedin-blue?logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/joão-pedro-ventura-51988a21b/) [![Github](https://img.shields.io/badge/GitHub-111217?logo=github&logoColor=white)](https://github.com/jauventur) | <img src="https://media.licdn.com/dms/image/v2/D4D03AQEyWGUnjpFoXw/profile-displayphoto-shrink_800_800/B4DZVYUR3sG4Ac-/0/1740943467142?e=1774483200&v=beta&t=C8fTzvieLo4sY47TwCb5v3i1Kt8jgn9WUKYdP2vfyBM" width="60"> |
| Matheus Marciano | Dev Team | [![Linkedin](https://img.shields.io/badge/Linkedin-blue?logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/matheus-marciano-leite/) [![Github](https://img.shields.io/badge/GitHub-111217?logo=github&logoColor=white)](https://github.com/marcyleite) | <img src="https://media.licdn.com/dms/image/v2/D4D03AQGpkZizsf7guQ/profile-displayphoto-shrink_800_800/profile-displayphoto-shrink_800_800/0/1697472746080?e=1774483200&v=beta&t=fE97NHSmwVgyuFCQ8Ww81XJ7eXD4wLcttk3PWcW4CoM" width="60"> |
| Tiago Alberto | Dev Team | [![Linkedin](https://img.shields.io/badge/Linkedin-blue?logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/tiago-alberto-303909167/) [![Github](https://img.shields.io/badge/GitHub-111217?logo=github&logoColor=white)](https://github.com/Tiago17santos) | <img src="https://media.licdn.com/dms/image/v2/D4D03AQGueuuOSlgVKA/profile-displayphoto-shrink_800_800/profile-displayphoto-shrink_800_800/0/1719004996407?e=1774483200&v=beta&t=58jo0Tm7oeStLml2Ww5upJGJc7suChq6QjrFphHjabw" width="60"> |
| Tiago Torres | Dev Team | [![Linkedin](https://img.shields.io/badge/Linkedin-blue?logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/tiago-torres-dos-reis/) [![Github](https://img.shields.io/badge/GitHub-111217?logo=github&logoColor=white)](https://github.com/TiagoTReis) | <img src="https://media.licdn.com/dms/image/v2/D4D35AQHO-0RsXZghfw/profile-framedphoto-shrink_800_800/profile-framedphoto-shrink_800_800/0/1737581648985?e=1773601200&v=beta&t=Ho2cWDEntTd8jQ1kWM9KX4ioJSCADEat7pCHhtE6JLc" width="60"> |

</div>

→ <a href="#23-de-fevereiro">Back to top</a>
