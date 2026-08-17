# AI-Based Student Performance Evaluation and Monitoring System

*Last updated 2026-08-17 by Teokan Duran D. Demircan*

## Project Description

The AI-Based Student Performance Evaluation and Monitoring System (APMS) is a centralized platform for tracking class records, assessments, evaluations, and student progress. The APMS helps faculty and academic administrators identify performance trends, generate student performance predictions, and provide timely and personalized student feedback.

APMS uses a shared Expo and React Native frontend for web and mobile, with Supabase providing authentication, PostgreSQL data storage, row-level security, audit logging, and serverless Edge Functions. Role-based access control supports system administrators, super administrators, academic administrators, faculty members, graders, and students.

Core features include:

- Dashboards and academic performance analytics;
- Class, assessment, and evaluation record management;
- AI-assisted student performance prediction and feedback;
- Configurable evaluation criteria and academic rules;
- User, role, and permission management;
- Audit logging, account onboarding, and system backup tools; and
- Responsive web and mobile interfaces.

## Setup Instructions

### Prerequisites

- [Node.js](https://nodejs.org/) v24.0 or above and npm
- A [Supabase](https://supabase.com/) project
- Expo SDK version 57.0 or later
- Latest version of Google Chrome

### 1. Install the application dependencies

From the repository root, open the active frontend project and install its packages:

```bash
npm install
```
### 2. Configure Supabase

Create a `.env` file inside `frontend/student-performance-monitor`:

```env
EXPO_PUBLIC_SUPABASE_URL=https://project-ref.supabase.co
EXPO_PUBLIC_SUPABASE_ANON_KEY=anon-key
```

Make sure to replace the URL and anon-key with the actual values from your Supabase project.

### 3. Run the application

```bash
npx expo start
npm run dev:android
npm run dev:ios
```

## File Structure

```text
APMS/
|-- backend/
|   `-- supabase/
|       `-- functions/             # Backend Edge Functions
|-- database/
|   |-- data.sql             # Database schema
|-- docs/
|   |-- api-spec.md                # API endpoint specification
|   |-- architecture.md            # System architecture overview
|   `-- data-model.md              # Main entities and relationships
|-- frontend/
|   `-- student-performance-monitor/
|       |-- assets/                # Images and application icons
|       |-- src/
|       |   |-- app/               # Expo Router routes
|       |   |-- components/        # Reusable UI components
|       |   |-- constants/         # Theme and access-control definitions
|       |   |-- contexts/          # Authentication context
|       |   |-- hooks/             # Shared React hooks
|       |   |-- screens/           # Application screens
|       |   |-- services/          # Supabase client and API services
|       |   `-- types/             # TypeScript types
|       |-- __tests__/             # Jest test suites
|       |-- app.json               # Expo configuration
|       `-- package.json           # Dependencies and npm scripts
`-- README.md                      # This file
```

## Contact Information

Project developers:
- Teokan Duran D. Demircan <tedu.demircan.swu@phinmaed.com>
- Myco Angel Lou A. Villomo <myal.villomo.swu@phinmaed.com>
- Dian Xane A. Cuadra <dial.cuadra.swu@phinmaed.com>
- Edwin Kyle S. Florendo <edso.florendo.swu@phinmaed.com>

## License

Copyright 2026 Teokan Duran D. Demircan, Myco Angel Lou A. Villomo, Dian Xane A. Cuadra, Edwin Kyle S. Florendo
Copyright 2026 Southwestern University PHINMA
