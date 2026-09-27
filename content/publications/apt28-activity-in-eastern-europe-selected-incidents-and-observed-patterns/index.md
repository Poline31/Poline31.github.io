---
title: "APT28 Activity in Eastern Europe: Selected Incidents and Observed Patterns"
date: 2026-09-27
draft: false
description: "Analysis of selected APT28 incidents in Eastern Europe between September 2025 and March 2026."
tags: ["APT28", "Threat Intelligence", "Eastern Europe", "Cyber Espionage", "CTI"]
categories: ["Threat Intelligence"]
---

# 1. Executive Summary

The aim of this report is to present the activity of APT28, an actor which, based on the data collected for this tracker, is one of the most active actors in the region.

Although the data is based on a selected set of sources and reflects my own research, it indicates that the actor has targeted countries such as Poland, Ukraine and Romania. This fits the main purpose of this tracker, which was created not only as a space for me to expand my own knowledge, but also to build a picture of the current threat landscape in Eastern Europe.

# 2. Scope & Methodology

The activity of APT28 is discussed based on three incidents recorded in the tracker, covering the period from September 2025 to March 2026.

The information I was able to collect from available sources allowed me to identify the artifacts and tools used by this actor during this period, within the scope of this tracker.

I would like to stress that the classification of artifact types presented in this report is my own interpretation. The purpose of this approach is mainly to show trends, identify possible patterns of activity and propose a way to aggregate this type of data using relational models.

# 3. APT28 Activity in Eastern Europe

In Eastern Europe, the term hybrid warfare is becoming increasingly important. In the face of growing threats from the East, it seems reasonable to try to connect different types of events – including diplomatic activities, hostile actions below the threshold of war, the way events are presented by official media and social media, as well as cyber attacks – and look at them in the context of specific situations, meetings, summits, political decisions and wars.

The main motivation of APT28 appears to be espionage. Recent activity by this actor has targeted Ukraine and countries supporting it, including countries that are also within the scope of this tracker – Poland and Romania.

At this point, the tracker does not contain incidents involving APT28 that would support the assumption that the Baltic states are also a target.

According to MITRE, the actor has been active since 2004, making it the oldest group currently included in the tracker. Open-source reporting links the group to the GRU, Russia's military intelligence service.

# 4. Selected Incidents – 2025/2026

| Category | Incident 1 – PRISMEX | Incident 2 – CVE-2026-21509 | Incident 3 – BadPaw / MeowMeow |
|---|---|---|---|
| **Date** | 25 September 2025 | 28–30 January 2026 | 5 March 2026 |
| **Target** | Ukrainian and NATO-supporting organizations | Military, government, diplomatic and transport organizations | Ukrainian organizations and individuals |
| **Geography** | Ukraine, Poland, Slovakia, Czech Republic, Romania, Slovenia and Turkey | Poland, Slovenia, Turkey, Greece, UAE and Ukraine | Ukraine |
| **Sector** | Defence, transport, logistics and maritime | Defence, government, transport and logistics | Not specified |
| **Attack vector** | Spear-phishing + malware | Spear-phishing + CVE exploitation | Phishing + malicious HTA + steganography |
| **Key artifacts** | CVE-2026-21509, CVE-2026-21513, PrismexSheet, MiniDoor, COVENANT, PrismexDrop, PrismexLoader, PrismexStager | CVE-2026-21509, SimpleLoader, NotDoor, BeardShell | BadPaw, MeowMeow |
| **Objective** | Espionage / potential disruption | Espionage | Espionage |
| **Attribution** | APT28 | APT28 | Russian state-aligned actor; low-confidence APT28 |
| **Impact** | Information collection; file deletion in one documented case | Access to government networks | Remote access, reconnaissance and file manipulation |
| **CTI relevance** | Interest in military logistics and supply chains supporting Ukraine | Interest in defence, government and transport organizations | Use of phishing, malware and steganography; APT28 attribution remains low-confidence |

## Incident 1

### APT28 Deploys PRISMEX Malware in Campaign Targeting Ukraine and NATO Allies

**Date:** 25 September 2025  
**Target:** Ukrainian and NATO-supporting organizations  
**Geography:** Ukraine, Poland, Slovakia, Czech Republic, Romania, Slovenia and Turkey  
**Sector:** Defence, transport, logistics and maritime  
**Attack vector:** Spear-phishing and malware deployment  
**Objective:** Espionage / potential disruption  
**Actor:** APT28

### What happened

APT28 used PRISMEX malware, steganography, COM hijacking and cloud services to target organizations supporting Ukraine. Targets included transport, maritime and logistics organizations.

### Impact

The activity provided access to information about logistics and operational planning. One documented case also involved file deletion.

### CTI relevance

The targeting of logistics and transport organizations may help collect information about the movement of military equipment and supplies.

---

## Incident 2

### APT28’s Stealthy Multi-Stage Campaign Leveraging CVE-2026-21509 and Cloud C2 Infrastructure

**Date:** 28–30 January 2026  
**Target:** Military, government, diplomatic and transport organizations  
**Geography:** Poland, Slovenia, Turkey, Greece, UAE and Ukraine  
**Sector:** Defence, government, transport and logistics  
**Attack vector:** Spear-phishing and exploitation of CVE-2026-21509  
**Objective:** Espionage  
**Actor:** APT28

### What happened

APT28 used spear-phishing and a known vulnerability to target organizations across Europe. The attacks also used compromised government accounts and cloud infrastructure for C2.

### Impact

The activity could provide access to government networks and sensitive information.

### CTI relevance

The targeting of defence, government and transport organizations shows a focus on military and logistical activities.

---

## Incident 3

### BadPaw and MeowMeow: Russian Cyber Offensive Targets Ukraine with Novel Malware Duo

**Date:** 5 March 2026  
**Target:** Ukrainian organizations and individuals  
**Geography:** Ukraine  
**Sector:** Not specified  
**Attack vector:** Phishing → malicious HTA → steganography → malware  
**Objective:** Espionage  
**Actor:** Russian state-aligned actor; low-confidence attribution to APT28

### What happened

Attackers sent phishing emails with a fake Ukrainian border-crossing message. A malicious HTA file used a hidden image to deliver BadPaw, which then downloaded the MeowMeow backdoor.

### Impact

The malware provided remote access, reconnaissance and file manipulation.

### CTI relevance

The attack combines simple phishing with malware hiding and anti-analysis techniques. Attribution to APT28 remains low-confidence.

# 5. Observed Patterns

Based on the analysis of the information related to the incidents described above, APT28 targeted European military and government entities, as well as maritime, transport and logistics organizations during 2025–2026.

The activity was mainly related to military supply chains, ammunition transport and railway logistics. As mentioned earlier, the main motivation of the group appears to be espionage.

The activity may allow the actor to collect information about routes, schedules and the movement of military equipment or ammunition. The same access and knowledge could potentially also support future disruption or sabotage of these deliveries.

# 6. Broader Strategic Context

Because the incidents involving this group are closely linked to the Russian state and its strategic interests, one possible hypothesis is that its cyber activity is connected with actions that remain below the threshold of kinetic war. Such actions may therefore avoid triggering stronger responses from the targeted states.

For the purpose of this report, I would also like to mention some facts and observations from the report *White Paper on Russian Acts of Sabotage and Diversion against Members of the Council of the Baltic Sea States*. I consider them relevant to the analysis presented in this tracker.

Russia’s approach towards Poland and other European and NATO countries in the region can be considered in the context of official Russian documents. The above-mentioned report refers to the 2012 Military Doctrine of the Russian Federation, the 2021 National Security Strategy and the 2024 Nuclear Doctrine, which identify NATO as a major source of threat.

The report also points to General Valery Gerasimov as a person who helped define the framework of so-called new-generation or hybrid warfare. In 2013, he described hostile actions against an opponent as potentially involving economic, informational, social and political measures, as well as taking advantage of social divisions within a country.

The report also discusses the targeting of critical infrastructure as part of such activities, with the potential aim of creating fear among the population and making it more difficult for state institutions to operate.

The incidents included in this tracker may also be consistent with elements of this broader strategy and could potentially support Russia’s strategic objectives.

# 7. Artifact Analysis

The information I was able to collect from available sources allowed me to identify the artifacts and tools used by this actor during this period, within the scope of this tracker.

![APT28 Artifacts](/images/artefacts-apt28.jpg)

If the data is standardized by artifact type, we get the following visualization:

![APT28 Artifact Types](/images/artefacts-types-apt-28.jpg)

I would like to stress once again that the artifact types are my own interpretation. The aggregation method used here is intended to support data visualization and help identify possible trends and patterns.

# 8. Key Findings / Assessment

The analysis of the selected incidents shows that APT28 activity in Eastern Europe is mainly focused on espionage and information collection.

The observed targeting of defence, government, transport, maritime and logistics organizations suggests a particular interest in organizations connected to Ukraine and its supporting countries.

One of the most relevant patterns is the focus on organizations connected to military logistics and transport. This may provide the actor with information about routes, schedules and the movement of military equipment and supplies.

Across the three incidents, phishing and malware were repeatedly observed, with malware present in all three cases. CVE exploitation and steganography were observed in two incidents. The artifact data shows different roles, including loaders, infostealers, droppers, backdoors and a C2 framework. This shows repeated use of some techniques while the specific tools varied between incidents.

At the same time, the available data does not allow me to conclude that all observed activity has a single operational objective or that all incidents are part of one campaign. The attribution of Incident 3 to APT28 also remains low-confidence.

# 9. Sources

1. *White Paper on Russian Acts of Sabotage and Diversion against Members of the Council of the Baltic Sea States*  
   [PISM – PDF](https://pism.pl/webroot/upload/files/Raport/Bia%C5%82a%20ksi%C4%99ga%20rosyjskich%20akt%C3%B3w%20sabota%C5%BCu%20i%20dywersji%20wobec%20cz%C5%82onk%C3%B3w%20Rady%20Pa%C5%84stw%20Morza%20Ba%C5%82tyckiego.pdf)

2. Trellix – *APT28’s Stealthy Multi-Stage Campaign Leveraging CVE-2026-21509 and Cloud C2 Infrastructure*  
   https://www.trellix.com/blogs/research/apt28-stealthy-campaign-leveraging-cve-2026-21509-cloud-c2/

3. The Hacker News – *APT28 Deploys PRISMEX Malware in Campaign Targeting Ukraine and NATO Allies*  
   https://thehackernews.com/2026/04/apt28-deploys-prismex-malware-in.html

4. SecurityOnline – *BadPaw and MeowMeow: Russian Cyber Offensive Targets Ukraine with Novel Malware Duo*  
   https://securityonline.info/badpaw-and-meowmeow-russian-cyber-offensive-targets-ukraine-with-novel-malware-duo/