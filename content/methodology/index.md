---
title: "Methodology"
---

## Project Scope

This project focuses on monitoring cyber incidents, threat actors and information operations targeting Eastern Europe.

The current geographic focus includes:

- Poland
- Ukraine
- Romania
- Baltic States

The analysis focuses on:

- government institutions
- critical infrastructure
- strategic industries
- information operations

The project tracks both cyber activity and related influence operations when they are connected to identified incidents or threat actors.

## Data Collection

The project is based on publicly available Cyber Threat Intelligence sources.

Information is collected from:

- security reports
- government advisories
- CERT publications
- threat intelligence and trusted open-source intelligence sources (Hacker News, Recorded Future, Dragos, Daily CyberSecurity etc.)
- Twitter/X
- Russian-language media

## Data Model

The tracker uses a structured CTI database approach.

It is created in Excel and transferred to Power BI for creating dashboards and reaching conclusions.

Each incident is analyzed using multiple dimensions:

### Incident / Artifacts / Actors / Narratives / Key Events

### Incident

- Incident_ID
- Incident
- Attack_motivation
- Data_start
- Data_end
- Description
- Actor_ID
- Actor
- Attack_type
- Source
- Target_Industry
- Target_Region
- Target_Organization
- Consequences

### Artifacts

- Incident_ID
- Incident
- Artifacts
- Artifact_Type

### Narratives

- Narrative_ID
- Account
- Narrative
- Narrative_type
- Date
- Source
- Language
- Tag
- Target_audience

### Key Events

- Event_ID
- What_happened/Event
- When
- Source
- News_type

## Incident Classification

Each identified incident is classified using several analytical categories defined in the project's dictionary.

### Attack Type

Examples:

- DDoS
- Ransomware
- Wiper
- Supply Chain
- Credential misuse/abuse
- Initial access / phishing
- Credential theft
- Exploitation of public-facing vulnerability

### Target Industry

Examples:

- Energy
- Water
- Transport
- Government
- Telecom
- Defense
- Unknown

### Attack Motivation

Examples:

- Espionage
- Financial gain
- Disruption
- Hacktivism
- Destruction
- Sabotage
- Unknown

### Affiliations

Examples:

- if possible, connected to intelligence services or countries
- if possible, connected to link type (narrative before attack, narrative after attack, simultaneous)

### Data Quality

Each entry is reviewed and linked to available sources to maintain traceability and reduce unsupported assumptions.

## Limitations

This project is based on publicly available information and is a private research project.

Some cyber activities may remain unidentified due to:

- limited visibility into threat actor operations
- lack of public reporting
- incomplete technical data
- attribution challenges