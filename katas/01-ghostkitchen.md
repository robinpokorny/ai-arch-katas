# Kata 1: GhostKitchen

**A platform for restaurants that exist only online.**

A startup wants to build a platform where chefs can launch virtual restaurant brands without a physical storefront. Multiple "brands" can operate from a single kitchen. Customers order through the platform, and the system must route orders to the correct kitchen and brand, manage menus that change daily, and handle surge pricing during peak hours.

**Users:** 50,000 customers in a single city at launch, scaling to 10 cities within a year. 200 kitchens at launch.

## Requirements

- Real-time order routing to the correct kitchen/brand combination
- Dynamic menu management (chefs update menus daily, some items have limited quantities)
- Surge pricing engine based on demand, weather, and time of day
- Driver dispatch integration (use existing delivery APIs, not building our own fleet)
- Customer order tracking from kitchen to doorstep

## Constraints

- Average order-to-delivery must be under 35 minutes
- The system must handle a 10× spike during lunch/dinner peaks without degradation
- Budget for infrastructure: €15,000/month at launch
- Team: 8 developers, 2 of whom are junior

## Additional context

The founder insists on "no microservices — keep it simple." The CTO disagrees. This tension is part of the problem.

[Back to all katas](../README.md#the-katas)
