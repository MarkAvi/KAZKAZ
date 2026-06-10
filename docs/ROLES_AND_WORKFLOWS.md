# Roles and Workflows

## Roles

Customer:
- creates shipment requests;
- sees only customer-safe shipment data;
- does not see supplier costs, competing quotes, or internal margin.

Logistics manager:
- reviews requests;
- sends RFQs;
- enters and compares quotes;
- creates shipments;
- updates shipment statuses;
- generates document checklist records.

Admin:
- controls carriers and air cargo partners;
- verifies partners;
- sees audit and system control data.

Accountant:
- sees finance fields;
- tracks document visibility;
- reviews shipment economics.

Carrier:
- represents road, rail, or multimodal transport providers.

Air cargo partner:
- represents air cargo offices, agents, GSA/GSSA style partners, or demo aviation providers.

## Shipment Request Flow

```txt
Customer request -> logistics review -> RFQ -> quote comparison -> selected quote -> shipment
```

## RFQ Rules

- Auto requests go to auto-capable carriers.
- Rail requests go to rail-capable carriers.
- Multimodal requests go to multimodal-capable carriers.
- Air requests go to air cargo partners.
- Non-air RFQs must not include air cargo partners.

## Shipment Rules

Shipments are created from selected quotes. Status changes are tracked through status events.

Initial operational statuses include:

- confirmed
- pickup scheduled
- picked up
- at terminal
- in transit
- customs
- arrived
- delivered
- closed
- cancelled

## Document Rules

Document checklists depend on transport mode.

Auto examples:
- CMR
- TTN
- invoice
- delivery act

Air examples:
- AWB
- security checklist
- invoice
- packing list
- MSDS

Rail examples:
- rail note
- wagon or container list
- customs draft
- invoice

Multimodal examples:
- multimodal note
- handover act
- customs draft
- invoice
- packing list
