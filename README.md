# CareBridge AI

CareBridge AI is a role-based healthcare web application that connects **patients**, **doctors**, and **guardians** in one workflow-driven platform. The app combines healthcare coordination features with AI-assisted symptom checking to help users manage care, assign providers, and track patient-related activity from dedicated dashboards.

## Overview

This project is built with **Next.js**, **React**, **TypeScript**, and **Tailwind CSS**. It provides authentication and dashboard experiences for multiple user roles and integrates with a backend API for registration, login, doctor assignment, guardian assignment, prescriptions, patient management, and symptom-based treatment suggestions.

## Key Features

- **Role-based authentication** for patients, doctors, and guardians
- **Dedicated dashboards** for each healthcare user type
- **AI-assisted symptom checking** for treatment suggestions
- **Doctor assignment** for patients
- **Guardian assignment** and guardian-patient relationship management
- **Assigned patient views** for doctors and guardians
- **Prescription creation workflow** for care management
- **Toast notifications** for important user actions and feedback

## User Roles

### Patient
- Create an account and sign in
- View a personal dashboard
- Check symptoms and receive possible treatment guidance
- Browse available doctors and assign a doctor

### Doctor
- Sign in to a dedicated dashboard
- View assigned patients
- Create prescriptions and support patient care workflows

### Guardian
- Sign in to a dedicated dashboard
- View assigned patients
- Track linked patient and doctor relationships

## Tech Stack

- **Framework:** Next.js 15
- **Language:** TypeScript
- **UI:** React 19, Tailwind CSS, Radix UI
- **Forms & validation:** React Hook Form, Zod
- **Notifications:** react-hot-toast
- **Icons:** lucide-react

## Project Structure

```text
src/
  app/              # App Router pages, auth flows, and dashboards
  components/       # Shared UI and domain components
  context/          # Authentication context and session state
  lib/              # Utility helpers
  services/         # API service functions
  types/            # Shared TypeScript types
```

## Getting Started

### Prerequisites

- Node.js 18+
- npm
- A running backend API compatible with the expected endpoints

### Installation

```bash
git clone https://github.com/msodiq19/healthcare-ai.git
cd healthcare-ai
npm install
```

### Environment Variables

Create a `.env.local` file in the project root and add:

```bash
NEXT_PUBLIC_BASE_URL=http://localhost:5000
```

Update the value to match your backend server URL.

### Run the Development Server

```bash
npm run dev
```

Then open `http://localhost:3000` in your browser.

## Available Scripts

```bash
npm run dev      # Start development server
npm run build    # Build for production
npm run start    # Start production server
npm run lint     # Run lint checks
```

## API Integration

The frontend expects a backend API exposed through `NEXT_PUBLIC_BASE_URL` and uses endpoints for:

- Authentication (`/api/v1/login`, `/api/v1/register`)
- Doctor assignment
- Guardian assignment
- Assigned patients
- Doctors, patients, and guardians listing
- Prescription creation
- Symptom treatment suggestions

## Suggested Repository Rename

If you want a less generic repository name, a stronger option is:

**`carebridge-ai`**

Alternative names:
- `medsync-ai`
- `triageflow`
- `carepath-ai`
- `healthnav-ai`

## Suggested About Description

**Smart healthcare platform for patients, doctors, and guardians.**

## Notes

- Authentication state is stored client-side using tokens.
- The project currently depends on an external backend service for core data and workflows.
- The repository was originally scaffolded from a Next.js starter and has now been tailored into a healthcare coordination application.

## Future Improvements

- Add screenshots for each dashboard
- Document backend setup and API contracts
- Add test coverage
- Add deployment instructions
- Replace placeholder/sample dashboard data with live production data where needed

## License

Add your preferred license information here.
