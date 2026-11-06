# Advanced Web Development Frameworks (ITUE301) - Final Project
> Semester 5th Capstone: Complete End-to-End Solutions for Practicals 1 through 13.

![CI Status](https://img.shields.io/badge/CI%20Pipeline-Passing-brightgreen?style=flat-square&logo=githubactions)
![React 18](https://img.shields.io/badge/React-18.2-blue?style=flat-square&logo=react)
![Vite 5](https://img.shields.io/badge/Vite-5.2-purple?style=flat-square&logo=vite)
![Express](https://img.shields.io/badge/Express-4.18-black?style=flat-square&logo=express)
![MongoDB](https://img.shields.io/badge/MongoDB-6.0-green?style=flat-square&logo=mongodb)
![Docker](https://img.shields.io/badge/Docker-Ready-2496ED?style=flat-square&logo=docker)

---

## 📌 Project Overview

This repository houses the full-stack capstone implementation designed to address all course learning outcomes (**CO1, CO2, CO3, CO4, CO5, CO6**) across **Practicals 1 to 13**:

| Practical | Title | Core Technologies | Location |
| :---: | :--- | :--- | :--- |
| **1** | Introduction to React & Component Architecture | React 18, Vite, JSX, Props | `student-portfolio/src/components/*` |
| **2** | React Router & Reactive State | React Router v6, useState, NavLink | `student-portfolio/src/pages/Contact.jsx` |
| **3** | REST API Consumption & Async States | Fetch API, useEffect, Spinner, Error UI | `student-portfolio/src/pages/Projects.jsx` |
| **4** | Express RESTful API & Middleware Pipeline | Express.js, Custom Logger, Morgan | `backend/server.js`, `backend/routes/tasks.js` |
| **4 Ext** | Richardson Maturity Model & HATEOAS | Level 0–3 Analysis, `_links` | `MATURITY.md`, `backend/models/Task.js` |
| **5** | MongoDB & Mongoose Schema Design | Mongoose ODM, Schema Validation | `backend/models/Task.js`, `backend/models/User.js` |
| **6** | Full-Stack Integration (React + Node + Mongo) | CORS, Central API Client, Optimistic UI | `student-portfolio/src/services/api.js`, `Tasks.jsx` |
| **7** | JWT Authentication & Input Validation | bcryptjs, jsonwebtoken, Auth Middleware | `backend/routes/auth.js`, `backend/middleware/*` |
| **8** | Performance Optimization & Code Splitting | `React.lazy()`, `<Suspense>`, Vite Chunks | `student-portfolio/src/App.jsx` |
| **9** | In-Memory Caching & Query Optimization | node-cache, Cache Invalidation, TTL | `backend/cache.js`, `backend/routes/tasks.js` |
| **10** | Event-Driven Architecture | Node EventEmitter, Async Notifications | `backend/events.js`, `backend/listeners.js` |
| **11** | Containerization with Docker & Compose | Dockerfile (Multi-stage), docker-compose | `Dockerfile`, `docker-compose.yml` |
| **12** | Automated CI/CD Pipeline | GitHub Actions, Jest, Supertest | `.github/workflows/ci.yml`, `backend/tests/*` |
| **13** | AI API Integration | OpenAI / Gemini API, Graceful Fallback | `backend/routes/ai.js`, `student-portfolio/Tasks.jsx` |

---

## 🚀 Running the Project

### Local Development (Concurrent)
1. **Start Backend API:**
   ```bash
   cd backend
   npm run dev
   # Runs on http://localhost:5000
   ```
2. **Start Frontend Client:**
   ```bash
   cd student-portfolio
   npm run dev
   # Runs on http://localhost:5173
   ```

### Run Automated Tests (Practical 12)
```bash
cd backend
npm test
```
*Result: 5 test suites pass verifying health, cache metrics, JSON header checks, AI fallback, and 404 responses.*

### Run via Docker Compose (Practical 11)
```bash
docker-compose up --build
```
*Spins up `awdf_frontend`, `awdf_backend`, and `awdf_mongodb` on the isolated `app-network`.*

---

## 📖 Complete Lab Manual & Theoretical Solutions
Refer to [**PRACTICAL_GUIDE.md**](./PRACTICAL_GUIDE.md) for full architectural diagrams, analysis questions, and step-by-step instructions.

