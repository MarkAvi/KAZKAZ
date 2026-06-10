# Local Setup

## Requirements

- Node.js
- npm
- PostgreSQL

## Environment

Create `.env` from the example file:

```bash
cp .env.example .env
```

Use environment variables for secrets and database credentials. Do not commit real secrets.

## Install

```bash
npm install
npm run prisma:validate
npm run prisma:generate
```

## Database Seed

```bash
npm run prisma:seed
```

Seed data includes demo users, carriers, air cargo partners, shipment requests, RFQs, quotes, shipments, documents, and audit records.

## Run

```bash
PORT=3001 npm run dev
```

Open:

```txt
http://localhost:3001
```

## Demo Login

All demo users use:

```txt
demo123
```

Known demo accounts:

- `admin@kaztranscargo.local`
- `logistics@kaztranscargo.local`
- `customer@demo.local`
- `accountant@kaztranscargo.local`
- `carrier@demo.local`
- `air@demo.local`

## Verification

Run before handing off changes:

```bash
npm run lint
npm run typecheck
npm run build
npx prisma validate
```
