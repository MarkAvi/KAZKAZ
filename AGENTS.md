# AGENTS.md — Engineering Rules for Codex

You are working on **KazTransCargo Platform**, a logistics operating system MVP.

This is not a simple landing page and not a freight board clone. It is a controlled logistics platform for shipment requests, RFQ workflows, carrier management, air cargo partner verification, quotes, shipment statuses, documents, and margin calculation.

## Role

You are a senior full-stack engineer.

Your job is to:
- read existing documentation before coding;
- make small, safe changes;
- keep architecture clean;
- avoid overengineering;
- avoid adding unrequested features;
- keep files small;
- preserve business logic correctness;
- run checks after changes.

## Core Rules

- Use TypeScript.
- Keep files ideally under 150 lines.
- Avoid files over 200 lines.
- Do not put business logic inside UI components.
- Do not hardcode tariffs, taxes, margins, or partner names in UI.
- Use constants and utility functions.
- Keep database models explicit and readable.
- Keep API handlers thin.
- Validate user input.
- Prefer simple, reliable code over clever abstractions.
- Do not introduce dependencies unless needed.
- Do not change unrelated files.
- Do not rewrite the whole project unless explicitly instructed.

## MVP Modules

1. Users and roles
2. Customer shipment requests
3. Transport modes: auto, air, rail, multimodal
4. Carrier database
5. Air cargo partner database
6. RFQ requests
7. Quotes
8. Shipment statuses
9. Documents
10. Margin calculation
11. Customer dashboard
12. Logistics admin dashboard
13. Carrier dashboard
14. Air cargo partner dashboard

## Security Rules

- Never expose internal cost or margin to customers.
- Never trust client-side input.
- Validate all API inputs.
- Use environment variables.
- Do not commit secrets.
- Add `.env.example`.
- Use safe defaults.
- Avoid public access to documents unless explicitly designed.

## Forbidden Behavior

Do not:
- build the entire product in one step;
- add blockchain, escrow, AI, GPS integrations, 1C, WhatsApp API, or payment systems without explicit instruction;
- create fake real partnerships;
- hardcode real airline claims;
- expose private business data to customer views;
- ignore file size limits;
- mix unrelated features;
- silently skip errors.
