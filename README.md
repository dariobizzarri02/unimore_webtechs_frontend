# Daimon Esports

The following thesis describes and supports the development of Daimon Esports, a web portal dedicated to the creation and management of mainly amateur esports competitions, without excluding potential official applications.

![[Pasted image 20240831230240.png]]
_Main screen of the platform._

# Installation Requirements

- Internet connection
- Local Linux, Windows or MAC device
- Git
- Docker

# Backend Installation

- git clone https://github.com/mbentity/daimon_esports
- docker build -t daimon_esports daimon_esports
- docker run -p 8000:8000 daimon_esports

# Frontend Installation

- git clone https://github.com/mbentity/daimon_esports_frontend
- docker build -t daimon_esports_frontend daimon_esports_frontend
- docker run -p 3000:3000 daimon_esports_frontend

# Access

- in case of need to perform tests, there is a account admin:
- username: techweb
- password: techweb

# Delivery

### As reported in the project proposal email:
"Web application for organizing, participating in and viewing esports tournaments.
Designed to be usable by anonymous and registered users:
- anonymous users can consult the rankings of all tournaments, and tune into the broadcast channels of the matches currently in progress
- registered users can sign up for tournaments, creating teams or requesting to join existing teams
- registered users can receive authorization to organize tournaments, specifying the discipline, the meeting platform, the broadcast channel and the dates of the tournament
The system must allow the search for tournaments based on criteria such as discipline, start date and availability of registrations.
The system must independently manage the available places for each team and for each tournament, and allow basic communication between users to send and approve team requests.
Every action must be modifiable and reversible: organizers must be able to modify or cancel a tournament, team leaders must be able to modify or disband a team, and players must be able to abandon a team, and consequently the tournament."

# Structure

The project is divided into three parts:

- Presentation thesis
- Frontend: multipage application in NextJS (Node, Typescript)
- Backend: API in Django Rest Framework (Django, Python)

Frontend and Backend are dockerized, as can be deduced from the installation process, and must both be executed for the correct functioning of the platform.
The Docker images were built based on Alpine, a lightweight and efficient Linux distribution.
Once both images are built and executed, the portal can be reached locally at http://localhost:3000, while the admin platform can be reached, always locally, at http://localhost:8000/admin.

# Tools

Frontend and Backend were developed with Visual Studio Code as the preferred IDE.
The thesis was written on Obsidian.md and compressed into PDF via Pandoc.
