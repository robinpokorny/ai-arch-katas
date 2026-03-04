---
title: "04 Greenhouse"
layout: default
parent: Katas
nav_order: 4
redirect_from:
  - /k04
  - /katas/04
---

# Kata 4: Greenhouse

**An IoT platform for urban vertical farms.**

A Berlin-based agritech startup operates vertical farms in repurposed shipping containers across European cities. They need a platform to monitor sensors (temperature, humidity, light, pH, nutrient levels), automate growing cycles, and predict harvest yields using historical data.

**Users:** 50 farm operators, 10 agronomists (data analysts), 5 maintenance technicians. 200 containers, each with ~80 sensors.

## Requirements

- Ingest sensor data from 16,000 sensors at 1-second intervals
- Automated alerts when readings fall outside optimal ranges
- Growing cycle automation (adjust lights, nutrients, irrigation on schedule)
- Yield prediction model that improves with historical data
- Dashboard for farm operators (mobile-first)
- Integration with supply chain systems for harvest scheduling

## Constraints

- Containers have unreliable internet (4G/LTE, sometimes drops for minutes)
- Critical actions (emergency shutoffs) must work even when offline
- Sensor hardware runs on ARM processors with 512MB RAM
- Budget-conscious startup — cloud costs must stay under €3,000/month
- Data retention: 5 years for regulatory compliance

## Additional context

Two containers recently lost an entire crop due to a sensor failure that went undetected for 6 hours. The founders are now obsessed with reliability.