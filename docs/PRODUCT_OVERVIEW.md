# Product Overview

KazTransCargo Platform is an MVP logistics operating system for companies that need transparent and controlled freight management.

The platform covers the operational chain:

```txt
Request -> RFQ -> Quote comparison -> Shipment -> Documents -> Accounting control
```

## Product Goal

The MVP proves that KazTransCargo can move shipment operations out of WhatsApp, Excel, and scattered documents into one structured workflow.

## Core Users

- Customer: creates shipment requests and tracks visible shipment progress.
- Logistics manager: reviews requests, sends RFQs, compares quotes, and manages shipments.
- Admin: manages users, partners, verification, and audit visibility.
- Accountant: tracks shipment economics and document availability.
- Carrier: participates in non-air RFQ workflows.
- Air cargo partner: participates in air cargo RFQ workflows.

## Transport Modes

- Auto freight
- Air cargo
- Rail freight
- Multimodal freight

Mode separation is important. Air partners must not receive non-air RFQs, and customer screens must never expose supplier costs or internal margins.

## Current MVP Capabilities

- Demo role-based login.
- RU/EN localization.
- Customer shipment request creation.
- Mode-aware partner selection for RFQs.
- Manual quote entry.
- Quote selection with margin preview.
- Shipment status progression.
- Mode-specific document checklist.
- Admin verification controls.
- Accounting margin and document visibility.

## Out of Scope for MVP

- Real payments.
- Escrow.
- Blockchain.
- GPS integrations.
- WhatsApp Business API.
- 1C integration.
- Real airline booking APIs.
- Public freight marketplace.
