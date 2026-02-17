# blue-team-threat-analysis
Threat analysis case study documenting investigation of suspicious DNS beaconing activity, MITRE ATTACK mapping, detection strategy and defensive hardening recommendations.

# Blue Team Threat Analysis – DNS Tunneling Case Study

## Overview

This project documents a simulated enterprise security incident involving suspicious DNS beaconing activity potentially linked to Command-and-Control (C2) communication.

The objective is to demonstrate structured Blue Team investigation methodology, MITRE ATTACK mapping, detection strategy development and defensive hardening recommendations.

---

## Scenario Summary

An internal workstation generated high-frequency DNS requests to an unknown external domain. The queries contained unusually long and entropy-heavy subdomains.

Initial hypothesis: Possible DNS tunneling used for covert C2 communication or data exfiltration.

---

## Investigation Goals

- Identify anomalous DNS behavior
- Assess potential Command-and-Control activity
- Map techniques to MITRE ATTACK
- Develop detection strategies
- Recommend defensive improvements

---

## Skills Demonstrated

- Threat Analysis
- Indicator of Compromise (IoC) identification
- DNS traffic anomaly recognition
- MITRE ATTACK mapping
- Detection engineering thinking
- Defensive architecture improvement

---

## Documentation

- Scenario Description → docs/scenario.md
- Investigation Process → docs/investigation.md
- MITRE Mapping → docs/mitre-mapping.md
- Detection Strategy → docs/detection-strategy.md
- Lessons Learned → docs/lessons-learned.md

---

## Intended Use

This case study is for educational and defensive security training purposes only.

## Included Sample Data

This repository includes a simulated DNS traffic log file for structured analysis:

logs/dns-traffic-sample.log

The log is intentionally simplified for educational purposes and does not contain malicious payloads.
## Analysis Artifacts

The included DNS log file is simulated for educational purposes.
It does not contain real attack traffic or malicious payloads.

