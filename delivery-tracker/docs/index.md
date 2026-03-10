# Delivery Tracker

From the KITCHEN to your DOOR — we're tracking every mile of the flavor journey!

The Delivery Tracker system handles real-time delivery logistics. Once an order leaves the kitchen, this system takes over — tracking driver locations, calculating ETAs, managing delivery routes, and keeping customers updated on exactly when their food will arrive.

## Components

- **Delivery Tracker API** — Go service for real-time delivery tracking. Handles driver location updates, ETA calculations, delivery status management, and customer notifications. Built in Go for maximum performance because every second counts when someone's waiting for their food.

## How It Works

When an order is marked ready for pickup by the Kitchen Display System, the Delivery Tracker assigns a driver and begins tracking. GPS coordinates are updated in real-time, ETAs are recalculated on every update, and customers can watch their food's journey on a live map in the Flavor Portal or Triple D Mobile app.
