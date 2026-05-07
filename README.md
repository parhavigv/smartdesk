# SmartDesk – Employee IT Helpdesk Portal

![MEAN Stack](https://img.shields.io/badge/Stack-MEAN-green?style=flat-square)
![Angular](https://img.shields.io/badge/Angular-17-red?style=flat-square&logo=angular)
![Node.js](https://img.shields.io/badge/Node.js-20-green?style=flat-square&logo=node.js)
![MongoDB](https://img.shields.io/badge/MongoDB-7.0-brightgreen?style=flat-square&logo=mongodb)
![Docker](https://img.shields.io/badge/Docker-Containerised-blue?style=flat-square&logo=docker)

> Full-stack IT helpdesk portal – employees raise tickets, agents resolve them, admins monitor SLA compliance in real time.

## Tech Stack
- **Frontend:** Angular 17, Angular Material, TypeScript, SCSS
- **Backend:** Node.js, Express.js, Socket.IO
- **Database:** MongoDB, Mongoose
- **Auth:** JWT + bcrypt, Role-Based Access Control
- **DevOps:** Docker, Docker Compose, GitHub Actions CI/CD

## Features
- Role-based dashboards: Employee / IT Agent / Admin
- Real-time ticket notifications via Socket.IO
- Automated SLA breach alerts (node-cron)
- Analytics dashboard: ticket volume, agent load, category trends
- JWT authentication with RBAC

## Project Structure
\\\
smartdesk/
+-- client/          # Angular 17 frontend
+-- server/          # Node.js + Express backend
¦   +-- config/      # MongoDB connection
¦   +-- src/
¦       +-- controllers/
¦       +-- middleware/  # JWT auth + RBAC
¦       +-- models/      # Mongoose schemas
¦       +-- routes/
¦       +-- utils/
+-- docker-compose.yml
+-- README.md
\\\

## Getting Started
\\\ash
# Backend
cd server && npm install && npm run dev

# Frontend
cd client && npm install && ng serve
\\\

## Author
**Parhavi G.V.** – B.Tech AI & ML, Dayananda Sagar University
[LinkedIn](https://linkedin.com/in/g-v-parhavi-b51030298) | [GitHub](https://github.com/parhavigv)
