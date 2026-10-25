# Real-Time Disaster Response Coordination Platform

A modern disaster response coordination system designed to connect citizens, volunteers, administrators, and relief agencies in one platform. The project helps manage emergency reports, map affected areas, assign field tasks, track resources, and maintain a clear operational picture during critical events.

The application is built around the real-world need for faster communication, better coordination, and data-driven decision-making during floods, cyclones, landslides, and other emergencies.

## 1. Introduction

### Project Overview
The platform, also called "দুর্যোগ সাড়া" (Disaster Response), brings together multiple stakeholders in a single digital system:

- Citizens can report incidents with images, locations, and descriptions.
- Volunteers can see active tasks, accept assignments, and update progress.
- Administrators can verify reports, assess severity, and allocate resources.
- Relief teams can monitor inventory, distribution, and operational status from one dashboard.

### Objectives
The main objectives of the project are to:

- reduce the delay between disaster detection and response action
- improve coordination between local communities and emergency teams
- make emergency decisions faster with live information and risk assessment
- ensure resources are allocated according to priority and urgency
- provide transparency for all stakeholders during disaster management

### Motivation
Natural disasters often create chaos because information arrives from scattered sources and response teams work without a unified system. In many emergency situations, delays in verification, poor communication, and lack of visibility lead to waste, confusion, and slower assistance.

This project was motivated by the need for a digital response platform that can:

- centralize emergency information
- map affected zones in real time
- prioritize high-risk areas
- assign volunteers and resources effectively
- give all users a clear operational picture in a crisis

## 2. Project Description

### Key Features

#### 1. Real-Time Disaster Reporting
Citizens can submit disaster reports including title, description, impact, district, coordinates, and images. Reports are stored centrally and become visible to administrators and response teams for review.

#### 2. Interactive Disaster Map
The system provides a map-based view of reported incidents, volunteer activity, task locations, affected zones, and relief resources. This makes it easier to identify hotspots and coordinate field operations.

#### 3. Volunteer Task Management
Volunteers can view assigned tasks, accept them, update status, and report progress. This keeps field teams connected to response priorities without requiring constant phone calls or manual updates.

#### 4. Report Verification and Approval
Administrators can review incoming reports, check authenticity, assign severity, and approve or reject submissions. This helps prevent false or duplicate reports while maintaining a trusted emergency channel.

#### 5. Severity Analysis
The platform calculates risk levels based on factors such as affected population, damage, infrastructure disruption, and emergency urgency. This allows critical cases to be prioritized first.

#### 6. Resource Allocation and Inventory Management
The platform helps manage food, medicine, water, shelter materials, and other supplies. Inventory can be tracked and allocated to the highest-priority incident zones.

#### 7. Field Issue Reporting
Volunteers can report field problems such as blocked roads, missing medical support, damaged infrastructure, or emergency needs at the ground level. These issues are fed into the dashboard for rapid action.

#### 8. Training and Volunteer Readiness
The platform supports training events and enrollment management so volunteers can improve readiness and operational capability before or during emergencies.

#### 9. Donations and Public Support
A public donation page enables people to contribute resources or funds through structured support flows, making community support easier to organize.

#### 10. Global Chat and Coordination Feed
A chat system allows administrators and volunteers to coordinate across roles and maintain situational awareness in a shared communication layer.

### Screenshots of the Project

The following images show the main interfaces of the platform:

![Dashboard Overview](docs/screenshots/dashboard.svg)

![Disaster Map View](docs/screenshots/map.jpeg)

![Admin Operations Dashboard](docs/screenshots/admin-dashboard.jpeg)

![Volunteer Operations Dashboard](docs/screenshots/volunteer-dashboard.jpeg)

## 3. Tech Stack

### Frontend
- React + TypeScript
- Vite for fast development and build tooling
- Tailwind CSS for clean, responsive UI design
- React Router for navigation between citizen, volunteer, and admin views
- Recharts for dashboards and analytics
- Leaflet + React Leaflet for interactive maps

### Backend
- Node.js
- Express.js
- TypeScript
- REST API architecture
- Multer for file uploads (proof images, incident media)

### Database
- MySQL 8+
- Structured schema for users, reports, tasks, issues, resources, allocations, inventory, and training events
- Relational design for role-based access and operational tracking

### AI / Intelligence Layer
- Rule-based severity scoring engine for incident prioritization
- Risk classification logic to highlight high-priority disaster zones
- Future-ready structure for integrating machine learning or predictive analysis

### Authentication and Security
- JWT-based authentication
- Role-based access control for citizen, volunteer, and admin accounts
- Password hashing and secure API handling

### APIs and Integrations
- Public and authenticated REST endpoints
- File upload support for disaster images
- CORS configuration for frontend-backend communication
- Structured API response handling and validation

### Testing and Collaboration
- Type-checking and build validation using TypeScript
- Version control with Git/GitHub
- Project structured for iterative feature delivery and team collaboration

## 4. Future Work

### Problems Faced
The platform addresses major emergency coordination problems, but some challenges still remain:

- delayed information flow between local communities and response teams
- duplicate or conflicting reports during large-scale disasters
- difficulty prioritizing incidents without a unified scoring model
- limited visibility into available resources across districts and agencies
- manual coordination causing slower operations in high-pressure situations

### Planned Upgrades and Enhancements

1. AI-Powered Forecasting
   Add predictive models that estimate risk based on rainfall, flood history, location data, and past incidents.

2. SMS and WhatsApp Alerts
   Send notifications directly to volunteers, local authorities, and affected communities for faster response.

3. Real-Time GIS Intelligence
   Use advanced geospatial analysis to highlight vulnerable zones, blocked routes, and resource coverage gaps.

4. Offline Mobile Support
   Add mobile-friendly offline syncing for field officers working in low-connectivity regions.

5. Multi-Language Support
   Expand support for Bangla, English, and local dialects to increase accessibility for all users.

6. Automated Resource Optimization
   Build smarter allocation logic for balancing relief supplies across multiple active disaster sites.

7. Better Analytics and Reporting
   Add trend dashboards for disaster patterns, response efficiency, and long-term preparedness planning.

8. Community Trust and Verification Tools
   Improve public credibility by adding stronger verification workflows and transparent response tracking.

## Getting Started

### Install frontend dependencies
```bash
npm install
```

### Start the frontend app
```bash
npm run dev
```

### Install backend dependencies
```bash
cd server
npm install
```

### Start the backend server
```bash
cd server
npm run dev
```

### Database setup
Import the SQL schema from the project root:

```bash
mysql -u root -p < database.sql
```

## License
This project is developed for emergency coordination and disaster response demonstration purposes. Please adapt and extend it appropriately for your own deployment, institutional, or research context.

## Summary
The Real-Time Disaster Response Coordination Platform is designed to transform emergency response from fragmented and delayed communication into a coordinated, transparent, and data-driven operation. By connecting public reporting, volunteer action, severity assessment, and relief logistics, the platform helps emergency teams respond faster and more effectively when every minute matters.
