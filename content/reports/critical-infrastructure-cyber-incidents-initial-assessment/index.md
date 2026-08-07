---
title: "Critical Infrastructure Cyber Incidents - Initial Assessment"
date: 2026-08-07
draft: false
description: "Initial assessment of cyber incidents affecting critical infrastructure and strategically important organisations across Eastern Europe."

tags:
  - Cyber Threat Intelligence
  - CTI
  - Critical Infrastructure
  - Incident Analysis
  - Eastern Europe
  - OSINT

categories:
  - Intelligence Reports
---

# Executive Summary

The **Critical Infrastructure Cyber Attack Tracker** is an ongoing monitoring project focused on documented cyber incidents affecting critical infrastructure and strategically important organisations across Eastern Europe.

Monitoring for the current dataset began in June 2026. The dataset primarily covers incidents identified between January and August 2026. One additional incident targeting Poland's power system in December 2025 was retained as a historical reference due to its strategic relevance.

The objective of the project is not to provide a comprehensive record of all cyber activity in the region, but to develop a structured intelligence dataset that can be used to identify recurring patterns in threat actor activity, targeting, operational characteristics, malware-related artefacts, sectors and geographic distribution.

At the current stage, the dataset contains **13 documented incidents associated with seven threat actors**. Although the dataset remains limited in size, it provides an initial baseline for analysing the regional threat landscape and demonstrates how structured CTI data can support further analytical work.

---

# Key Findings

- **13 cyber incidents** affecting critical infrastructure and strategically important organisations were identified between January and August 2026.

- The dataset currently contains activity associated with **seven threat actors**, including established state-sponsored groups and more recently observed actors.

- Ukraine was the most frequently represented target country, followed by Poland, Romania and Lithuania.

- APT28 and Ghostwriter accounted for the highest number of documented incidents in the current dataset.

- Espionage was the most frequently identified operational motivation among incidents where the available reporting provided sufficient information to assess motivation.

- Initial Access, particularly phishing-related activity, was the most frequently observed operational characteristic associated with incidents attributed to Ghostwriter in the current dataset.

- Government and Defence were the two most frequently represented target sectors, together accounting for **56.5% of recorded sector assignments**.

- The current dataset should be treated as an initial analytical baseline, rather than a comprehensive representation of cyber activity across Eastern Europe.

---

# Regional Threat Landscape

The geographic distribution of incidents in the dataset reflects the broader security environment in Eastern Europe.

Ukraine represents the most frequently observed target country, followed by Poland, Romania and Lithuania.

![Geographic distribution of documented cyber incidents across Eastern Europe](/images/incident-distribution-by-region.jpg)
*Figure 1. Geographic distribution of documented cyber incidents identified within the current dataset.*

This concentration is consistent with the strategic importance of the region and the continuing impact of the war in Ukraine on the regional cyber threat environment.

However, the dataset should not be interpreted as a measurement of the absolute volume of cyber activity in individual countries. The number of incidents recorded is influenced by several factors, including:

- availability of public reporting,
- source coverage,
- inclusion criteria used for the tracker.

At the current stage of the project, the dataset contains insufficient observations for Latvia and Estonia. These countries therefore remain underrepresented in the current analysis.

As monitoring continues, additional incidents will be incorporated into the dataset. This should allow geographic distribution and differences between target countries to be assessed with greater confidence.

It should also be noted that a single incident may involve more than one country or organisation. Consequently, country-level counts represent recorded targeting assignments rather than necessarily representing an equal number of unique incidents.

# Threat Actor Landscape

During the analysed period, activity associated with seven threat actors was identified within the dataset.

The identified actors represent different levels of operational experience, capabilities and organisational maturity. The dataset includes both long-established groups and actors associated with more recent activity.

The distribution of documented incidents shows that APT28 and Ghostwriter account for the largest share of observed activity within the current dataset.

The following visualisation presents the number of documented incidents associated with each analysed threat actor.

![Threat actors](/images/actors-activity-per-incident.jpg)
*Figure 2. Distribution of documented incidents associated with identified threat actors.*

---

# Threat Actor Geographic Relationship

The geographic relationship between threat actors and their observed targets provides an additional analytical perspective.

The tracker allows individual actors to be mapped against the countries represented in the incident dataset.

![Threat actor activity by geographic region](/images/actor-activity-by-region.jpg)
*Figure 3. Relationship between identified threat actors and observed target regions.*

The current visualisation indicates a concentration of activity involving Ukraine, although this finding should be interpreted in the context of the relatively limited observation period and the availability of public reporting.

The dashboard represents recorded target regions, rather than the total operational footprint of each threat actor.

---

# Threat Actor Longevity

Another useful analytical dimension is the estimated year in which each threat actor first became publicly associated with cyber activity.

The dataset includes actors with significantly different operational histories.

APT28 is the oldest actor represented, with publicly reported activity dating back to approximately 2003.

![Threat actor activity timeline](/images/threat-groups-active-since.jpg)
*Figure 4. Estimated year of first publicly reported activity associated with threat actors represented in the dataset.*

The presence of both long-established and more recently observed actors illustrates the changing composition of the regional cyber threat landscape.

The emergence of actors such as UAC-0226 and Qilin in the dataset occurs within the broader context of the evolving cyber environment associated with the war in Ukraine.

This temporal relationship should not be interpreted as evidence of causation.

# Incident Characteristics

The relationship between threat actors and the operational characteristics observed in individual incidents provides another analytical dimension of the tracker.

Rather than treating these characteristics as formal campaign classifications, the dataset records the operational characteristics of individual incidents based on the available reporting.

The classifications used in this project were developed specifically to provide a consistent analytical framework across the collected dataset. They are based on publicly available intelligence (OSINT), analytical judgement and AI-assisted classification.

These classifications are intended for the purposes of this project and do not represent an official industry standard.

The dashboard below presents the distribution of incident characteristics associated with the seven identified threat actors.

![Incident characteristics by threat actor](/images/actors-activity-per-incident.jpg)
*Figure 5. Distribution of operational characteristics observed across incidents associated with identified threat actors.*

---

# Ghostwriter: Incident-Level Analysis

For demonstration purposes, the dashboard below has been filtered to display incidents associated with Ghostwriter.

The available data indicates that, between January and August 2026, incidents attributed to Ghostwriter in the dataset were predominantly associated with Initial Access activity.

This should not be interpreted as evidence that other tactics or stages were absent from the actor's wider operations.

Rather, it indicates that Initial Access was the most frequently observed characteristic among the incidents represented in this dataset.

In several documented cases, phishing was identified as an important compromise vector. This suggests that credential theft or user interaction represented a significant component of the observed intrusion activity.

The current dataset contains three documented incidents associated with Ghostwriter, including incidents involving targets in Poland and Ukraine.

![Ghostwriter incident-level analysis](/images/incident-type-per-campaign-ghostwriter.jpg)
*Figure 6. Incident-level characteristics observed in documented Ghostwriter-related incidents within the current dataset.*

The purpose of this analysis is to demonstrate how the underlying data model can be used to examine an individual threat actor across multiple dimensions without treating the available incidents as a single operation.

# Malware and Technical Artefacts

The collected intelligence also enables analysis of the relationship between threat actors and malware-related artefacts.

The current dataset includes references to a range of technical artefacts, including:

- CVEs,
- loaders,
- backdoors,
- stealers.

Within the current dataset, APT28 demonstrates the broadest distribution of malware-related artefacts.

![Technical artefact categories](/images/artifact-type.jpg)
*Figure 7. Distribution of technical artefact categories identified across analysed incidents.*

This may indicate a comparatively diverse operational toolkit, although the limited dataset does not allow this observation to be generalised to the actor's overall capabilities.

For the purposes of this public report, the complete list of malware is not presented but it is available.

The underlying tracker is instead structured to allow relationships between threat actors, incidents and technical artefacts to be explored interactively.

For this report, malware information has therefore been aggregated into broader categories to provide analytical context without reproducing the full technical inventory.

---

# Operational Motivation

Where the available sources provided information about attacker motivation, this information was incorporated into the dataset.

Based on the currently available observations, espionage represents the most frequently identified motivation.

![Threat actor operational motivation analysis](/images/actors-motivation.jpg)
*Figure 8. Operational motivations identified across incidents where sufficient reporting enabled assessment.*

This finding is consistent with the high representation of government and defence targets within the dataset and with the activity associated with established state-sponsored or state-aligned actors.

However, attribution of motivation is dependent on the quality and specificity of the underlying sources.

Where motivation could not be reliably established, it should not be inferred solely from the target sector or technical characteristics of an incident.

The current findings therefore indicate a strong espionage-oriented pattern within the analysed dataset, rather than demonstrating that espionage is the motivation behind all cyber incidents affecting critical infrastructure in Eastern Europe.

As the monitoring project expands, additional observations will make it possible to determine whether this pattern remains consistent over time.

---

# Sector Analysis

The majority of recorded sector assignments are associated with the Government (**34.78%**) and Defence (**21.74%**) sectors.

![Target sector distribution](/images/incidents-per-industry.jpg)
*Figure 9. Distribution of target sectors represented in the current incident dataset.*

Together, these categories account for **56.5% of all recorded sector assignments**, indicating that government and defence organisations represent the dominant target categories within the current dataset.

This distribution is consistent with the previously identified prevalence of espionage-related activity and the strategic importance of these sectors.

The third most frequently represented category is Unknown (**13.04%**).

This classification indicates cases where the available sources did not provide sufficient information to reliably determine the target sector.

Other represented sectors include:

| Sector | Percentage |
|---|---:|
| Energy | 8.7% |
| Combined Heat and Power | 4.35% |
| Diplomacy | 4.35% |
| Logistics | 4.35% |
| Renewable Energy | 4.35% |
| Transport | 4.35% |

**Important note:** a single incident may involve more than one target sector.

Consequently, the percentages above represent sector assignments within the dataset, rather than the percentage of unique incidents.

A multi-sector incident can therefore contribute to more than one category.

---

# Intelligence Assessment

The initial findings suggest that cyber operations targeting critical infrastructure across Eastern Europe remain primarily espionage-driven and are concentrated against strategically important states, particularly Ukraine.

The observed activity is dominated by established threat actors such as APT28 and Ghostwriter, indicating that long-standing state-sponsored cyber operations continue to shape the regional threat landscape.

It should be noted that the current dataset represents only a small subset of cyber incidents affecting Eastern Europe and should not be interpreted as a comprehensive picture of all regional cyber activity.

Nevertheless, even this limited dataset reveals recurring operational patterns and emerging trends in threat actor behaviour, targeting priorities, and threat characteristics.

As the project represents the initial stage of a long-term monitoring initiative, the findings presented in this report should be considered a baseline for future analysis rather than definitive conclusions.

The primary objective of this report is to introduce the project, present the first analytical observations, and demonstrate the capabilities of the underlying intelligence data model.

The tracker has been designed to support flexible analysis across multiple dimensions, including:

- incidents,
- threat actors,
- malware,
- target sectors,
- geographical regions,
- operational motivations.

The model has the potential to support:

- Cyber Threat Intelligence (CTI),
- Security Operations Centers (SOC),
- Incident Response (IR),
- Threat Hunting,
- strategic cyber risk assessment.

As additional intelligence is collected, future reports will provide progressively deeper insight into the evolving cyber threat landscape across Eastern Europe.