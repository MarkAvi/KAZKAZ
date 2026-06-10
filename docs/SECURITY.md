# Security Rules

## Data Visibility

Customers must never see:

- supplier costs;
- internal margins;
- competing partner quotes;
- internal comments;
- private partner verification data.

Internal finance data belongs only to logistics, accounting, senior management, and admin roles.

## Input Safety

- Validate server action input.
- Never trust client-side form values.
- Keep workflow decisions on the server.
- Avoid hardcoded tariffs, taxes, margins, and partner names in UI components.

## Environment Safety

- Store secrets in environment variables.
- Keep `.env.example` updated.
- Do not commit real `.env` files.
- Use safe defaults for local development.

## Documents

Documents should default to private/internal visibility unless a workflow explicitly marks them as customer-safe.

## Partner Data

Do not create fake real partnerships or claim official airline relationships. Demo partners must remain clearly demo or unverified unless verified by the business.
