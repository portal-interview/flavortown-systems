# Ordering System

The MAIN EVENT at Flavortown! This system handles the entire customer order journey.

From the moment a customer opens the Flavor Portal to the second their food arrives at the door, the Ordering System orchestrates every step. Menu browsing, burger building, cart management, authentication, payment processing, and order routing — it's all here.

## Components

- **Flavor Portal** — The main React web application. The front door to Flavortown.
- **Burger Builder** — Microfrontend for order customization. Build your perfect meal.
- **Triple D Mobile** — React Native mobile app. Flavortown in your pocket.
- **Hot Sauce Gateway** — API gateway that routes all frontend traffic to backend services.
- **Grill Master Service** — Go service that processes and routes orders to the right kitchen stations.
- **The Butcher Shop** — Java/Spring authentication service. Every customer gets a VIP pass.

## Architecture

The ordering system follows a gateway pattern. All client traffic flows through the Hot Sauce Gateway, which handles authentication (via The Butcher Shop), rate limiting, and routing. Orders are processed by the Grill Master Service, which orchestrates the fulfillment workflow across kitchen stations.
