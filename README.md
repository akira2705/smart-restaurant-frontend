# Smart Restaurant — Angular Frontend

> Angular 20 frontend for the Smart Restaurant Queue & Table Management System. Provides a responsive dashboard for managing tables, queues, and reservations in real time.

---

## Pages

| Route | Page | Description |
|---|---|---|
| `/dashboard` | Dashboard | Overview of live table status and queue |
| `/tables` | Tables | View and update table availability |
| `/queue` | Queue | Add, call, and remove customers from queue |
| `/reservation` | Reservations | Create and manage upcoming reservations |
| `/manager` | Manager | Admin controls and settings |

## Tech Stack

| Technology | Version |
|---|---|
| Angular | 20 |
| Angular Material | 20 |
| TypeScript | 5.9 |
| RxJS | 7.8 |

## Getting Started

### Prerequisites

- Node.js >= 18
- Angular CLI (`npm install -g @angular/cli`)
- Backend running at `http://localhost:3000` (see [smart-restaurant-backend](https://github.com/akira2705/smart-restaurant-backend))

### Installation

```bash
git clone https://github.com/akira2705/smart-restaurant-frontend.git
cd smart-restaurant-frontend

npm install
```

### Run

```bash
ng serve
```

App runs at `http://localhost:4200`

### Build for Production

```bash
ng build
```

Output goes to `dist/`

### Run Tests

```bash
ng test
```

## Project Structure

```
src/app/
├── pages/
│   ├── dashboard/     # Live overview
│   ├── queue/         # Queue management
│   ├── tables/        # Table status
│   ├── reservation/   # Reservations
│   └── manager/       # Admin panel
├── services/
│   ├── queue.service.ts
│   ├── table.service.ts
│   └── user.service.ts
├── shared/
│   └── navbar/        # Shared navigation component
└── app.routes.ts      # Route definitions
```

## Environment Config

Edit `src/environments/environment.ts` to point to your backend:

```ts
export const environment = {
  production: false,
  apiBaseUrl: 'http://localhost:3000'
};
```

---

Made by Team 38 — Kumaraguru College of Technology
