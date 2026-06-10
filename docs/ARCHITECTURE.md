# Architecture

KazTransCargo MVP is implemented as a simple Next.js monolith.

## Application Stack

- Next.js App Router for routes and server rendering.
- React and TypeScript for UI.
- Tailwind CSS for styling.
- Prisma for database access.
- PostgreSQL for persistent data.

## Main Layers

```txt
src/app         route segments and pages
src/components  reusable UI components
src/server      server actions and session logic
src/lib         shared utilities
src/constants   small app constants
prisma          schema and seed data
docs            project documentation
```

## Business Logic Rule

Business logic should stay in `src/server` or `src/lib`. UI components should render data and call actions, not own workflow rules.

## Key Server Areas

- `src/server/auth`: demo login, session cookie, role routing.
- `src/server/logistics`: RFQ, quote, shipment, and document workflow actions.
- `src/server/admin`: partner verification and audit actions.
- `src/server/i18n`: locale persistence.
- `src/server/shipments`: shipment status operations.

## Data Model Areas

The Prisma schema covers:

- users and roles;
- organizations;
- shipment requests;
- carriers;
- air cargo partners;
- RFQs and recipients;
- quotes;
- shipments;
- status events;
- documents;
- margin calculations;
- audit logs.

## Design Direction

The interface follows a dark logistics command-center style inspired by the Stitch design references in `stitch_design_system_blueprint`.

The UI should remain operational, dense, and clear. It should not become a marketing landing page inside the app.
