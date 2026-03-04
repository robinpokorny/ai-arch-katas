# Kata 8: Sentinel

**A city-wide public infrastructure monitoring system.**

A European city government wants a system to monitor bridges, tunnels, water mains, and electrical grids using a combination of existing SCADA systems, new IoT sensors, and drone inspections. The goal: predict failures before they become emergencies.

**Users:** 30 infrastructure engineers, 10 city planners, emergency response teams (fire, police), elected officials (dashboard only). 12,000 sensors across the city.

## Requirements

- Ingest data from heterogeneous sources (SCADA, IoT sensors, drone footage, weather APIs)
- Anomaly detection with configurable thresholds per asset type
- Predictive maintenance models (bridge stress, pipe corrosion, cable wear)
- Emergency alert system with escalation workflows
- GIS-based visualisation of all monitored assets
- Public dashboard (limited data, citizen-facing)

## Constraints

- Must integrate with legacy SCADA systems (some from the 1990s, speaking Modbus/DNP3)
- Critical alerts must reach responders within 30 seconds
- System must meet government security certifications (BSI IT-Grundschutz)
- Data classification: some sensor data is restricted, some is public
- Government procurement: hosted on-premise or on sovereign cloud only

## Additional context

The city had a near-miss incident where a bridge showed stress fractures that sensors detected but nobody noticed for 3 weeks because the data was trapped in a silo. This project is the response.

[Back to all katas](../README.md#the-katas)
