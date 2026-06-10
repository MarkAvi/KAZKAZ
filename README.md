# KazTransCargo Platform MVP

KazTransCargo Platform is a logistics operating system MVP for controlled shipment requests, RFQ workflows, verified partner management, quote comparison, shipment statuses, document control, and internal margin visibility.

It is not a landing page or a freight board clone. The product is designed as an internal command center for KazTransCargo operators, with separate workspaces for customers, logistics managers, admin users, accounting, carriers, and air cargo partners.

## Current Product Scope

- Role-based demo authentication.
- RU/EN interface support.
- Customer shipment request intake.
- Transport modes: auto, air, rail, multimodal.
- Carrier and air cargo partner databases.
- Mode-aware RFQ creation.
- Manual quote entry and quote comparison.
- Shipment creation from selected quote.
- Shipment status timeline.
- Mode-specific document checklist.
- Internal margin and accounting visibility.
- Admin verification and audit control.

## Stack

- Next.js App Router
- TypeScript
- Tailwind CSS
- Prisma
- PostgreSQL

## Local Setup

```bash
npm install
cp .env.example .env
npm run prisma:validate
npm run prisma:generate
npm run prisma:seed
PORT=3001 npm run dev
```

Local app URL:

```txt
http://localhost:3001
```

Demo password:

```txt
demo123
```

## Useful Commands

```bash
npm run lint
npm run typecheck
npm run build
npm run prisma:validate
npm run prisma:generate
npm run prisma:seed
```

## Documentation

- [Product Overview](docs/PRODUCT_OVERVIEW.md)
- [Architecture](docs/ARCHITECTURE.md)
- [Local Setup](docs/LOCAL_SETUP.md)
- [Roles and Workflows](docs/ROLES_AND_WORKFLOWS.md)
- [Security Rules](docs/SECURITY.md)
- [Design System](docs/DESIGN_SYSTEM.md)
