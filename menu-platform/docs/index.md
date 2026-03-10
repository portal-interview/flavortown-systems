# Menu Platform

The MENU is where it all starts, folks! You can't order flavor if you can't see what's cooking.

The Menu Platform manages all menu content across Flavortown. Seasonal specials, daily features, permanent classics, allergen info, nutritional data, pricing, and those mouthwatering descriptions that make you order twice as much as you planned.

## Components

- **Menu Service** — Node.js CRUD service for menu management. Create menus, add items, update prices, manage categories. The single source of truth for everything on the menu.

## How It Works

Menu data is managed through the Menu Service API and consumed by the Flavor Portal, Burger Builder, and Triple D Mobile. When a menu changes, all frontends pick up the updates in real-time. We support multiple menu versions for A/B testing different layouts and item orderings.
