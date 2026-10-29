# 🩺 MedCore — Next-Gen Patient Health OS & Clinical Telemetry Suite

[![Next.js 16](https://img.shields.io/badge/Frontend-Next.js%2016-black?style=flat&logo=next.js)](https://nextjs.org/)
[![NestJS](https://img.shields.io/badge/Backend-NestJS%2010-ea2849?style=flat&logo=nestjs)](https://nestjs.com/)
[![PostgreSQL](https://img.shields.io/badge/Database-PostgreSQL%2016-336791?style=flat&logo=postgresql)](https://www.postgresql.org/)
[![Prisma](https://img.shields.io/badge/ORM-Prisma%206-2d3748?style=flat&logo=prisma)](https://www.prisma.io/)
[![TailwindCSS](https://img.shields.io/badge/Styling-TailwindCSS%204-38bdf8?style=flat&logo=tailwindcss)](https://tailwindcss.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> **MedCore** is an enterprise-grade clinical health operating system featuring continuous 60 FPS cardiac EKG telemetry, dual-persona physician & patient portals, interactive e-prescriptions (Rx), appointment scheduling, and automated AI symptom triage.

---

## 🌟 Key Features

### 1. 📈 Continuous 60 FPS Cardiac EKG Telemetry Engine
- Custom HTML5 Canvas rolling phosphor buffer rendering medical P-Q-R-S-T cardiac cycles in real-time.
- Neon cyan/emerald glow traces with clinical oscilloscope grid calibration (25 mm/s, 10 mm/mV).
- Synchronized R-wave peak detection with cardiac beat flashes and live vitals modulation (Heart Rate, Arterial BP, SpO2, Core Temp).
- **Interactive Vitals Stress Simulator:** Instantly simulate Tachycardia (128 BPM), Athlete Bradycardia (52 BPM), and Normal Sinus (72 BPM).

### 2. 🩺 Dual-Persona Role-Based Access Control (RBAC)
- **Patient Portal (Amol Paul):** Schedule specialist appointments, review diagnostic EHR timeline, track allergies, and launch telehealth video visits.
- **Physician Command Center (Dr. Sarah Connor, MD):** Multi-bed ICU telemetry switcher (Bed 04, Bed 02, Bed 08), patient consultation approval queue, and clinical chart note authoring.

### 3. 💊 e-Prescription (Rx) & Pharmacy Dispatch
- Digital prescription generation with drug dosage, administration frequency, and encrypted pharmacy registry dispatch.

### 4. 🤖 AI Clinical Symptom Analyzer (Triage Engine)
- Automated natural language symptom triage evaluating patient complaints against differential diagnostic guidelines.

---

## 🏗️ Tech Stack

- **Frontend:** Next.js 16 (App Router, Turbopack), Tailwind CSS 4, Lucide Icons, HTML5 Canvas 60 FPS Engine
- **Backend:** NestJS 10, TypeScript, REST APIs, Swagger OpenAPI, JWT RBAC
- **Database:** PostgreSQL 16 via Prisma ORM 6, Redis 7 Caching
- **DevOps:** Docker Compose Monorepo Structure

---

## 🚀 Quick Start Guide

### 1. Start Database Containers
```bash
docker compose up -d
```

### 2. Start Backend API (Port 4000)
```bash
cd apps/api
pnpm install
pnpm run start:dev
```

### 3. Start Frontend App (Port 3000)
```bash
cd apps/web
pnpm install
pnpm run dev
```

Visit: `http://localhost:3000/dashboard`

---

## 📄 License
Distributed under the MIT License.
