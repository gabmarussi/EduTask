# EduTask

EduTask is a web task management platform for academic workflows, built to help teachers and advisors organize activities, deadlines, and priorities in one clean interface.

<p align="center">
	<img width="1200" alt="EduTask interface" src="https://github.com/user-attachments/assets/3c7c931b-d029-4ddd-9196-55b25c87a1e6" />
</p>

## Table of Contents

- [Overview](#overview)
- [Academic Context](#academic-context)
- [Key Features](#key-features)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [Environment Variables](#environment-variables)
- [Database and Migrations](#database-and-migrations)
- [Project Structure](#project-structure)
- [License](#license)
- [Team](#team)
- [Repository About (Description and Topics)](#repository-about-description-and-topics)

## Overview

EduTask was developed as an academic software engineering project at FECAP. The main goal is to improve time management and day-to-day planning for education professionals through a modern and intuitive task management experience.

## Academic Context

This project was produced at FECAP (Fundacao de Comercio Alvares Penteado) as part of a Software Engineering and Systems Architecture course.

- Institution: FECAP
- Course: Software Engineering and Systems Architecture
- Academic use case: educational task management for teachers and advisors

## Key Features

- Email/password authentication with Supabase Auth.
- Task CRUD (create, update, delete, complete).
- Custom lists (create, edit, delete).
- Smart filters for Today, Overdue, and High Priority tasks.
- Search by task title.
- Multiple visualizations: List view and Kanban view.
- Responsive interface for desktop and mobile usage.

## Tech Stack

| Layer                | Technology                          |
| :------------------- | :---------------------------------- |
| Frontend             | React 18 + Vite + TypeScript        |
| UI                   | Tailwind CSS + Radix UI + shadcn/ui |
| Data Fetching        | TanStack Query                      |
| Backend and Database | Supabase (Auth + PostgreSQL)        |
| Tooling              | ESLint + PostCSS                    |

## Getting Started

### Prerequisites

- Node.js LTS
- npm
- A Supabase project

### Installation

```bash
npm install
```

### Run in development

```bash
npm run dev
```

### Production build

```bash
npm run build
```

### Preview production build

```bash
npm run preview
```

### Lint

```bash
npm run lint
```

## Environment Variables

Create a `.env` file in the project root:

```env
VITE_SUPABASE_URL=https://<your-project>.supabase.co
VITE_SUPABASE_PUBLISHABLE_KEY=<anon-or-publishable-key>
```

## Database and Migrations

SQL migrations are located in `supabase/migrations/`.

Apply them using either:

- Supabase SQL Editor, or
- Supabase CLI

The schema includes core entities such as user profiles, task lists, and tasks.

## Project Structure

```text
src/
	components/        # UI and feature components (task cards, dialogs, sidebar, views)
	hooks/             # Custom hooks (auth, responsiveness, toast)
	integrations/      # External services (Supabase client and generated types)
	lib/               # Shared helpers and utilities
	pages/             # Route-level pages (Auth, Index, Settings, NotFound)
	types/             # Domain types (tasks and lists)
supabase/
	migrations/        # Database migration scripts
```

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.

## Team

Developed by:

- [Arthur Rodrigues Ferreira](https://www.linkedin.com/in/eduardo-savino-gomes-77833a10/)
- [Gabriel Henrique Coelho Marussi](https://www.linkedin.com/in/gabrielmarussi/)
- [Lucas Kenichi Soares Abe](https://www.linkedin.com/in/lucasskenichi/)
- [Pedro Dimitry Zyrianoff](https://www.linkedin.com/in/pedro-dimitry-zyrianoff-2223b1268/)

Academic advisor:

- [Lucy Mari Tabuti](https://www.linkedin.com/in/lucymari/)

Institution:

- [FECAP - Fundacao de Comercio Alvares Penteado](https://www.fecap.br/)

## Repository About (Description and Topics)

Use the following in your GitHub repository "About" section.

Description:

```text
EduTask is a task management web app for academic workflows, built with React, TypeScript, and Supabase to help teachers and advisors organize tasks, priorities, and deadlines.
```

Suggested topics:

```text
react, typescript, vite, supabase, postgresql, tailwindcss, shadcn-ui, task-manager, kanban, productivity, education, academic-project
```