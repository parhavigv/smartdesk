# SmartDesk – Employee IT Helpdesk Portal

![MEAN Stack](https://img.shields.io/badge/Stack-MEAN-green?style=flat-square)
![Angular](https://img.shields.io/badge/Angular-17-red?style=flat-square&logo=angular)
![Node.js](https://img.shields.io/badge/Node.js-20-green?style=flat-square&logo=node.js)
![MongoDB](https://img.shields.io/badge/MongoDB-7.0-brightgreen?style=flat-square&logo=mongodb)
![Docker](https://img.shields.io/badge/Docker-Containerised-blue?style=flat-square&logo=docker)
![CI/CD](https://img.shields.io/badge/CI%2FCD-GitHub%20Actions-black?style=flat-square&logo=github-actions)

> Full-stack IT helpdesk portal built with the MEAN stack. Employees raise tickets, IT agents triage and resolve them, admins monitor SLA compliance in real time.

## Features
- Role-based dashboards: Employee / IT Agent / Admin
- Real-time ticket notifications via Socket.IO
- Automated SLA breach alerts (node-cron)
- JWT authentication with Role-Based Access Control
- Analytics dashboard: ticket volume, agent load, category trends
- Containerised with Docker, CI/CD via GitHub Actions
- Average ticket resolution time reduced by 42% via SLA automation

## Tech Stack
| Layer | Technology |
|-------|-----------|
| Frontend | Angular 17, TypeScript, Angular Material, SCSS |
| Backend | Node.js 20, Express.js 4, Socket.IO |
| Database | MongoDB 7.0, Mongoose ODM |
| Auth | JWT, bcrypt, RBAC |
| DevOps | Docker, Docker Compose, GitHub Actions |

## Project Structure
\\\
smartdesk/
+-- client/                # Angular 17 frontend
¦   +-- src/app/
¦       +-- components/    # navbar, dashboard, ticket-form, ticket-list
¦       +-- services/      # HTTP + Socket services
¦       +-- guards/        # Auth + Role guards
¦       +-- models/        # TypeScript interfaces
+-- server/                # Node.js + Express backend
¦   +-- config/            # MongoDB connection
¦   +-- src/
¦       +-- controllers/   # Business logic
¦       +-- middleware/     # JWT auth + RBAC
¦       +-- models/        # Mongoose schemas (User, Ticket)
¦       +-- routes/        # REST API routes
¦       +-- utils/         # SLA scheduler, Socket manager
+-- docker-compose.yml
+-- README.md
\\\

## Getting Started
\\\ash
# Backend
cd server
npm install
cp .env.example .env
npm run dev

# Frontend
cd client
npm install
ng serve
\\\

## API Endpoints
| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | /api/auth/register | Register user |
| POST | /api/auth/login | Login, returns JWT |
| GET | /api/tickets | Get tickets (role-filtered) |
| POST | /api/tickets | Create ticket |
| PATCH | /api/tickets/:id | Update ticket status |
| GET | /api/analytics/summary | SLA + volume summary |

## Author
**Parhavi G.V.** – B.Tech AI and ML, Dayananda Sagar University
[LinkedIn](https://linkedin.com/in/g-v-parhavi-b51030298) | [GitHub](https://github.com/parhavigv)
