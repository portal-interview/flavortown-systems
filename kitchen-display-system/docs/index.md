# Kitchen Display System

The COMMAND CENTER of the kitchen! Every ticket, every station, every order — right here on the screen.

The Kitchen Display System (KDS) is what the kitchen crew sees. It manages the flow of orders from the moment they're fired to the moment they're plated and ready for pickup or delivery. Real-time updates, station assignments, timing alerts, and order prioritization all run through this system.

## Components

- **Kitchen API** — Node.js/Express service that manages order queues, station assignments, and kitchen display state. The nerve center of kitchen operations.
- **Deep Fryer** — Async job processor that handles background tasks like notification dispatching, inventory updates, and order completion workflows. It takes the heavy lifting off the Kitchen API's plate.

## Architecture

The Kitchen API receives orders from the Grill Master Service and manages them through the fulfillment pipeline. Orders are assigned to stations, tracked through preparation stages, and marked complete. The Deep Fryer handles all async side effects so the main API stays fast and responsive.
