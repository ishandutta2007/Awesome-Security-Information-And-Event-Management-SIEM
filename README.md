# Awesome-Security-Information-And-Event-Management-SIEM

## Top Security Information and Event Management (SIEM) Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Log Aggregation, Threat Detection & Open-Source Security Analytics*  

**Last updated: October 2026**



This repository tracks notable **commercial SIEM platforms** and **open-source projects** that collect, correlate, and analyze security events from across an organization's infrastructure. These tools help security teams detect threats, investigate incidents, and meet compliance requirements.



**Examples** include Microsoft Sentinel, Splunk Enterprise Security, Google Chronicle SIEM, IBM QRadar, Exabeam, Securonix, LogRhythm, Elastic Security, Sumo Logic Cloud SIEM, and Rapid7 InsightIDR (the category leaders).



**Open-source emphasis**: SIEM is a domain where open-source tools provide genuine production alternatives. **Wazuh** leads as the most balanced open-source SIEM with native XDR and compliance capabilities . **Security Onion** delivers a complete network security monitoring platform . **Matano** brings a serverless, AWS-native security data lake approach . This section is heavily expanded.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Microsoft Sentinel](https://azure.microsoft.com/en-us/products/microsoft-sentinel)**  

  Cloud-native SIEM and SOAR integrated with Azure, Microsoft 365, and third-party sources. **Consumption-based pricing** per GB ingested. **The leading cloud SIEM** for Microsoft-centric organizations.



- **[Splunk Enterprise Security](https://www.splunk.com/en_us/products/enterprise-security.html)**  

  **The enterprise SIEM standard** with mature UEBA, correlation, and the largest app ecosystem. **Pricing scales with data volume** — $150-$2,000 per GB/day depending on tier . **Best for large SOCs** with dedicated teams and budget.



- **[Google Chronicle SIEM](https://cloud.google.com/chronicle)**  

  Google's cloud-native SIEM with **petabyte-scale ingestion**, UDM normalization, and YARA-L detection rules. **Best for organizations needing massive scale** without infrastructure management.



- **[IBM QRadar](https://www.ibm.com/products/qradar-siem)**  

  Enterprise SIEM with offense management, flow analysis, and QRadar SOAR integration.



- **[Exabeam](https://www.exabeam.com/)**  

  SIEM with **behavioral analytics (UEBA)** and automated incident timelines for accelerated investigations.



- **[Securonix](https://www.securonix.com/)**  

  Cloud-native SIEM with UEBA, SOAR, and NDR capabilities. **Best for large enterprises** needing integrated security analytics.



- **[LogRhythm](https://logrhythm.com/)**  

  SIEM with **native log management and SOAR** capabilities. **Best for mid-market** organizations wanting an integrated platform.



- **[Sumo Logic Cloud SIEM](https://www.sumologic.com/solutions/cloud-siem/)**  

  Cloud-native SIEM built on the Sumo Logic observability platform with automated threat detection.



- **[Rapid7 InsightIDR](https://www.rapid7.com/products/insightidr/)**  

  SIEM with **user behavior analytics**, endpoint detection, and honeypot integration. **Best for organizations wanting SIEM + EDR convergence**.



## Open-Source GitHub Projects



- **[Wazuh](https://github.com/wazuh/wazuh)**  

  **The leading open-source security platform with SIEM and XDR capabilities**, GPLv2 licensed with 16,646+ GitHub stars . **Native HIDS, FIM (File Integrity Monitoring), rootkit detection, vulnerability detection, and 1,000+ MITRE ATT&CK pre-configured rules** . **OpenSearch is the default backend** since v4.4 — Apache 2.0 licensed with no restrictions . **Single-node handles 5,000-10,000 EPS** (1,000-2,000 agents) on 8 vCPU / 16 GB RAM . **The best-balanced open-source SIEM** for most organizations — deployment is moderate, rules are ready-to-use, and compliance modules (PCI-DSS, NIST 800-53) are native . **Trade-off**: lacks advanced ML-based behavioral detection and kernel-level EDR telemetry of commercial tools .



- **[Security Onion](https://github.com/Security-Onion-Solutions/securityonion)**  

  **Free and open platform for network security monitoring, log management, and case management**, built by defenders for defenders . **Integrates Suricata (NIDS), Zeek (network metadata), Elastic Stack (storage/search), Elastic Agent (host visibility), Strelka (file analysis), and OpenCanary honeypots** into a unified grid . **Full packet capture** provides "a video camera for your network" — hard to deceive and captures everything in transit . **Scales from a single appliance to a grid of a thousand nodes** . **Over 2 million downloads** . **Trade-off**: requires significant resources — Standalone node needs 4 cores / 24 GB RAM / 200 GB storage minimum, with 32 GB+ recommended for real traffic . **Best for network-focused monitoring and threat hunting** with dedicated hardware.



- **[Matano](https://github.com/matanolabs/matano)**  

  **Open-source, serverless SIEM alternative for AWS**, Apache-2.0 licensed . **Security data lake in your AWS account** — ingest petabytes of logs, store in Apache Iceberg Parquet files on S3 . **Detection-as-code in Python** — manage rules in Git with test, code review, and audit lifecycle . **No vendor lock-in** — query directly from AWS Athena, Snowflake, etc. . **Fully serverless (Lambda, S3, SQS)** with Rust for performance . **Trade-off**: AWS-specific, 576 commits from 16 contributors, last commit over a year ago . **Best for AWS-native teams** wanting a modern security data lake.



- **[OSSIM (AlienVault)](https://github.com/AlienVault-OTX/OSSIM)**  

  **Open-source SIEM with event collection, correlation, and OpenVAS integration**, GPLv2 licensed. **Scored well in comparative analysis** — third best open-source SIEM after Wazuh and Graylog . **Trade-off**: open-source version **lacks reporting, real-time alerting console, and log tagging** available in commercial version . **Best for organizations wanting vulnerability assessment integrated with SIEM**.



- **[OSSEC](https://github.com/ossec/ossec-hids)**  

  **Host-based intrusion detection system (HIDS)** — the foundation that Wazuh was built upon. **Log analysis, file integrity checking, rootkit detection, and active response** . **Trade-off**: Wazuh has largely superseded OSSEC with better maintenance and expanded capabilities. **Best for understanding SIEM foundations** or legacy deployments.



- **[Graylog Open](https://github.com/Graylog2/graylog2-server)**  

  **Centralized log management with search, streams, and alerting**, SSPL licensed . **Scored second best in comparative analysis** . **Trade-off**: **advanced correlation requires Enterprise edition** . Versions 6.2 and 6.3 are past end-of-life as of mid-2026 — **verify support window before deployment** . **Best for log management** with SIEM as secondary use case.



- **[ELK Stack (Elastic Security)](https://github.com/elastic/elasticsearch)**  

  **Elasticsearch + Logstash + Kibana + Beats** for log storage, processing, and visualization. **Elastic Security provides SIEM/EDR features** . **Trade-off**: **free version lacks correlation engine, built-in security rules, and native alerting** — advanced features require subscription . **Elastalert** partially fills the correlation gap . **Best for organizations already using Elastic Stack** for observability.



- **[OpenSearch](https://github.com/opensearch-project/OpenSearch)**  

  **Apache 2.0 licensed fork of Elasticsearch/Kibana** (from 7.10), led by AWS . **Security Analytics includes Sigma rules, alerting, and anomaly detection at no cost** . **The default backend for Wazuh** since v4.4 . **Best for organizations wanting Elasticsearch functionality without licensing concerns**.



- **[Apache Metron](https://github.com/apache/metron)**  

  **Apache's retired SIEM platform** — historically significant as a big-data security analytics framework. **Development ended** — not recommended for new deployments.



- **[Prelude SIEM](https://github.com/Prelude-SIEM)**  

  **Hybrid SIEM with agent-based and agentless collection**, GPL licensed. **Open-source alternative to commercial SIEMs** with correlation and alerting.



- **[SIEMonster](https://github.com/SIEMonster-Project)**  

  **Open-source SIEM with multi-tenancy** for MSSPs. **Best for service providers** managing multiple client environments.



### Additional Strong Open-Source Options



- **Suricata** — Network IDS/IPS with deep packet inspection, TLS, and application-layer detection. **Not a SIEM** but essential as a detection source .

- **Zeek** — Network metadata and file extraction. **Not a SIEM** but provides critical network context .

- **Snort** — Network IDS focused on DDoS, port scans, and OS fingerprinting. **Not a SIEM** .

- **Fluentd** — Log collector and forwarder. **Not a SIEM** — no detection or correlation .

- **Elastalert** — Alerting on Elasticsearch data, partially fills ELK's correlation gap .



**Frameworks for building custom SIEM solutions**: Choose based on team capacity and use case. **Wazuh** for the most balanced open-source SIEM — native XDR, compliance modules, and MITRE ATT&CK rules with moderate deployment complexity . **Security Onion** for network-focused monitoring with full packet capture and integrated tooling . **Matano** for AWS-native security data lakes with detection-as-code . **Graylog** for log management with SIEM as secondary . **ELK/OpenSearch** for organizations already invested in the Elastic ecosystem .



**Critical consideration**: Open-source SIEM requires **engineering overhead** — maintaining indices, tuning rules, patching agents, and managing storage are ongoing responsibilities . A senior security engineer dedicated to SIEM maintenance typically costs more per year than a mid-market commercial SIEM license . Commercial platforms provide **curated detection content** (2,000+ MITRE-mapped rules in Log360 vs. community rules requiring customization) and **audit-ready compliance reports** . The choice depends on whether you have engineering capacity or budget for vendor support.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- SIEM platforms process sensitive security telemetry and may contain PII. Self-hosted solutions require proper security hardening, access controls, and compliance with data privacy regulations.

- **Open-source SIEM has hidden costs**: engineering overhead, detection coverage gaps, limited UEBA, manual compliance reporting, and higher false-positive rates increase analyst triage time . A senior engineer dedicated to SIEM maintenance costs more than many commercial licenses.

- **Resource requirements are real**: Security Onion Standalone needs 24 GB RAM minimum, 32 GB+ recommended . Wazuh single-node handles 5,000-10,000 EPS on 8 vCPU / 16 GB RAM . Size infrastructure before committing.

- **Graylog versions 6.2 and 6.3 are end-of-life** as of mid-2026 . Verify support windows for any open-source component.

- The open-source ecosystem provides strong log aggregation, detection, and compliance foundations, but **curated detection content, vendor support SLAs, and UEBA** remain primarily commercial offerings.



---



**Made for security analysts, SOC teams, and organizations seeking SIEM sovereignty.**

Let's make security information and event management more open, transparent, and accessible.
