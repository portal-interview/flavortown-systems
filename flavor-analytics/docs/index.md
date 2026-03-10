# Flavor Analytics

We're turning RAW DATA into FLAVOR GOLD! Analytics that hit different.

Flavor Analytics is our data and ML platform. It ingests event streams from every system in Flavortown — orders, clicks, deliveries, kitchen metrics — transforms them through our ETL pipelines, and produces insights that drive the business. The crown jewel is our Flavor Predictor, an ML model that recommends dishes based on customer preferences, ordering history, and trending flavors.

## Components

- **The Smokehouse** — Python-based data pipeline and ETL service. Ingests raw events, transforms them, and loads them into our analytics warehouse. Named after the art of slow smoking — we take raw data and turn it into something beautiful.
- **Flavor Predictor** — ML recommendation engine built with scikit-learn. Analyzes customer behavior to predict what they'll love next. "You liked the sriracha burger? Try the ghost pepper fries."

## Architecture

Events flow from all Flavortown services into The Smokehouse via our event bus. The Smokehouse runs transformation pipelines that clean, enrich, and aggregate the data. Clean data feeds into the Flavor Predictor's training pipeline, which continuously improves our recommendation models.
