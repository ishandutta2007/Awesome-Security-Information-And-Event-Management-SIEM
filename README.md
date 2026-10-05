<!-- Banner -->
<p align="center">
  <img src="assets/banner.svg" alt="Awesome Security Information and Event Management (SIEM) Ecosystem Banner" width="100%" />
</p>

# 🛡️ Awesome Security Information & Event Management (SIEM)

<p align="center">
  <a href="https://github.com/ishandutta2007/Awesome-Awesome-Awesome"><img src="https://img.shields.io/badge/Awesome-%E2%9C%94-blueviolet?style=flat-square&logo=github" alt="Awesome"/></a>
  <a href="https://discord.gg/jc4xtF58Ve"><img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Discord" /></a>
  <a href="https://github.com/ishandutta2007/Awesome-Security-Information-And-Event-Management-SIEM/stargazers"><img src="https://img.shields.io/github/stars/ishandutta2007/Awesome-Security-Information-And-Event-Management-SIEM?style=flat-square&color=gold" alt="GitHub_Stars"/></a>
  <a href="https://github.com/ishandutta2007/Awesome-Security-Information-And-Event-Management-SIEM/network/members"><img src="https://img.shields.io/github/forks/ishandutta2007/Awesome-Security-Information-And-Event-Management-SIEM?style=flat-square&color=blue" alt="GitHub Forks"/></a>
  <a href="https://github.com/ishandutta2007/Awesome-Security-Information-And-Event-Management-SIEM/pulls"><img src="https://img.shields.io/badge/PRs-Welcome-brightgreen.svg?style=flat-square" alt="PRs Welcome"/></a>
  <a href="LICENSE"><img src="https://img.shields.io/github/license/ishandutta2007/Awesome-Security-Information-And-Event-Management-SIEM?style=flat-square" alt="License"/></a>
  <a href="https://github.com/ishandutta2007"><img alt="GitHub followers" src="https://img.shields.io/github/followers/ishandutta2007?label=Follow" /></a>
</p>

> **A curated, battle-tested list of enterprise SaaS platforms, cloud-native SIEMs, open-source security log analytics, UEBA, and threat detection systems.**

---

## 📌 Overview & Market Context

Security Information and Event Management (**SIEM**) serves as the nerve center for modern Security Operations Centers (**SOC**). SIEM solutions ingest, correlate, and analyze log data from across cloud workloads, endpoints, network telemetry, and identity providers to detect cyber threats, automate incident response (**SOAR**), and maintain audit compliance (PCI-DSS, SOC 2, ISO 27001, HIPAA).

---

## 📑 Table of Contents

- [☁️ SaaS & Hosted Enterprise SIEM Platforms](#️-saas--hosted-enterprise-siem-platforms)
- [🔓 Open-Source SIEM & Security Analytics GitHub Projects](#-open-source-siem--security-analytics-github-projects)
- [🛠️ Complementary Detection & Collector Tools](#️-complementary-detection--collector-tools)
- [🤝 How to Contribute](#-how-to-contribute)
- [⚠️ Disclaimer & Trade-Off Analysis](#️-disclaimer--trade-off-analysis)
- [📈 Star History](#-star-history)
- [💖 Support & Sponsorship](#-support--sponsorship)

---

## ☁️ SaaS & Hosted Enterprise SIEM Platforms

> 📊 **Estimated Sector Market Size**: The global SIEM market is valued at **$5.5 Billion - $7.8 Billion in 2026** and is projected to reach **$12.5+ Billion by 2030** (CAGR ~14.5%).  
> 🏢 **Market Fragmentation**: The SIEM sector is **Moderately Fragmented**, dominated by hyperscale cloud service providers (Microsoft Sentinel, Google Chronicle) alongside specialized enterprise cybersecurity titans (Splunk/Cisco, IBM QRadar, Exabeam, Securonix).

*The table below compares top commercial SaaS SIEM solutions, sorted by **Company Size / Revenue / Valuation** in descending order:*

| Platform / Vendor | Company Size / Valuation | Starting Price (Specific Tiers) | Free Tier / Free Trial Limit | Key Focus & Primary Use Case |
| :--- | :--- | :--- | :--- | :--- |
| **[Microsoft Sentinel](https://azure.microsoft.com/en-us/products/microsoft-sentinel)** | **~$3.1 Trillion** Market Cap (Microsoft) / >$20B Security ARR | **$2.46 / GB ingested** (Pay-as-you-go); Commitment tiers start at **$1.50 / GB** (100 GB/day = $150/day) | **31-Day Free Trial** (up to 10 GB/day log ingestion free); 5 MB/user/month free M365 E5 log ingestion | Cloud-native SIEM & SOAR tightly integrated into Azure, M365, & multi-cloud enterprise logs |
| **[Google Chronicle SIEM](https://cloud.google.com/chronicle)** | **~$2.1 Trillion** Market Cap (Alphabet Inc.) | **~$45 / active user / year** or **$10 / GB ingested** (Enterprise base starts at **$25,000 / year**) | **30-Day Free Trial** on Google Cloud with **$300 in free cloud credits** | Petabyte-scale cloud log ingestion with Unified Data Model (UDM) normalization & YARA-L detection rules |
| **[Splunk Enterprise Security](https://www.splunk.com/en_us/products/enterprise-security.html)** | **~$210 Billion** Market Cap (Cisco) / $28B Acquisition | **$150 / GB / day** workload tier (**~$1,800 / month** minimum workload price) | **14-Day Free Trial** (Splunk Cloud); **60-Day Free Trial** for Splunk Enterprise (**up to 500 MB/day free forever** local ingest) | Enterprise SIEM standard with mature UEBA, correlation engine, and massive app ecosystem |
| **[IBM QRadar SIEM](https://www.ibm.com/products/qradar-siem)** | **~$200 Billion** Market Cap (IBM) / ~$2.5B Security ARR | **$1,200 / month** base SaaS package (or **$800 / month** per 50 EPS tier) | **14-Day Free Trial** with full SaaS console access & sample security telemetry | Enterprise threat intelligence, offense management, network flow analysis, and QRadar SOAR |
| **[Rapid7 InsightIDR](https://www.rapid7.com/products/insightidr/)** | **~$2.5 Billion** Market Cap (Rapid7) / ~$800M ARR | **$2.15 / asset / month** (billed annually, minimum 500 assets = **$1,075 / month**) | **30-Day Free Trial** with unlimited asset monitoring and full UEBA features | Combined SIEM + XDR with User Behavior Analytics, endpoint detection, & honeypot traps |
| **[Exabeam](https://www.exabeam.com/)** | **~$2.4 Billion** Valuation (Merged with LogRhythm 2024) | **$6.00 / user / month** (**~$2,000 / month** base platform license) | **14-Day Interactive Sandbox** trial with pre-loaded attack scenario playbooks | Advanced Behavioral Analytics (UEBA), automated incident timeline creation, & risk scoring |
| **[Sumo Logic Cloud SIEM](https://www.sumologic.com/solutions/cloud-siem/)** | **~$1.7 Billion** Valuation (Francisco Partners) / ~$300M ARR | **$2.50 / GB ingested** for Cloud SIEM package (**~$250 / month** starter commit) | **30-Day Free Trial** with **1 GB / day** ingestion limit & 30-day log data retention | Multi-tenant cloud-native SIEM built on log analytics & automated threat correlation |
| **[Securonix](https://www.securonix.com/)** | **~$1.2 Billion** Valuation (Vista Equity Partners) / ~$150M ARR | **$3.00 / GB / day** (**~$1,500 / month** entry enterprise tier) | **30-Day Sandbox Demo Trial** with up to **50 GB total ingestion limit** | Cloud-native SIEM with deep UEBA, SOAR automation, & Network Detection & Response (NDR) |
| **[LogRhythm](https://logrhythm.com/)** | **~$1.2 Billion** Valuation (Merged into Exabeam) | **$1,500 / month** starting base price for LogRhythm Axon SaaS platform | **14-Day Free Trial** of LogRhythm Axon SaaS cloud instance | Mid-market SIEM platform offering log management, simplified threat lifecycle, & SOAR |

---

## 🔓 Open-Source SIEM & Security Analytics GitHub Projects

> 🚀 **Open-Source SIEM Advantage**: Self-hosted open-source SIEM solutions provide full data sovereignty, zero ingestion vendor lock-in, customizable detection-as-code (Sigma, YARA, Python rules), and cost savings for high-volume log environments.

*The table below lists open-source SIEMs, security data lakes, and log security management platforms, sorted by **GitHub Stars_Count** in descending order:*

| Repository / Project | GitHub_Stars | License | Core Capabilities & Architecture |
| :--- | :---: | :--- | :--- |
| **[Elasticsearch (Elastic Security)](https://github.com/elastic/elasticsearch)** | <a href="https://github.com/elastic/elasticsearch/stargazers"><img src="https://img.shields.io/github/stars/elastic/elasticsearch?style=social&color=white" alt="elastic/elasticsearch stars"/></a> | Elastic License 2.0 / SSPL | Distributed search & analytics engine underpinning Elastic Security SIEM, built-in threat correlation, & Kibana security dashboards. |
| **[Vector](https://github.com/vectordotdev/vector)** | <a href="https://github.com/vectordotdev/vector/stargazers"><img src="https://img.shields.io/github/stars/vectordotdev/vector?style=social&color=white" alt="vectordotdev/vector stars"/></a> | MPL-2.0 | Ultra-fast, high-performance Rust log processor and routing pipeline for SIEM ingestion, filtering, and data transformation. |
| **[Wazuh](https://github.com/wazuh/wazuh)** | <a href="https://github.com/wazuh/wazuh/stargazers"><img src="https://img.shields.io/github/stars/wazuh/wazuh?style=social&color=white" alt="wazuh/wazuh stars"/></a> | GPLv2 | **The leading open-source SIEM & XDR platform**. Integrates HIDS, File Integrity Monitoring (FIM), rootkit detection, & 1,000+ MITRE ATT&CK rules. |
| **[OpenSearch](https://github.com/opensearch-project/OpenSearch)** | <a href="https://github.com/opensearch-project/OpenSearch/stargazers"><img src="https://img.shields.io/github/stars/opensearch-project/OpenSearch?style=social&color=white" alt="opensearch-project/OpenSearch stars"/></a> | Apache-2.0 | Apache 2.0 community search & analytics engine with built-in Security Analytics plugin, native Sigma rule execution, & anomaly detection. |
| **[Fluentd](https://github.com/fluent/fluentd)** | <a href="https://github.com/fluent/fluentd/stargazers"><img src="https://img.shields.io/github/stars/fluent/fluentd?style=social&color=white" alt="fluent/fluentd stars"/></a> | Apache-2.0 | CNCF unified log collector & forwarder used to structure, aggregate, and ship security logs to SIEM backend storage. |
| **[Sigma Rule Standard](https://github.com/SigmaHQ/sigma)** | <a href="https://github.com/SigmaHQ/sigma/stargazers"><img src="https://img.shields.io/github/stars/SigmaHQ/sigma?style=social&color=white" alt="SigmaHQ/sigma stars"/></a> | CC0-1.0 / MIT | Generic, open signature format for SIEM detection rules. Translates detection logic into Splunk, Elastic, QRadar, and SQL queries. |
| **[T-Pot Honeypot Platform](https://github.com/telekom-security/tpotce)** | <a href="https://github.com/telekom-security/tpotce/stargazers"><img src="https://img.shields.io/github/stars/telekom-security/tpotce?style=social&color=white" alt="telekom-security/tpotce stars"/></a> | GPLv3 | Multi-honeypot platform running Dockerized honeypots integrated with Elastic Stack SIEM for threat intelligence log collection. |
| **[Graylog Open](https://github.com/Graylog2/graylog2-server)** | <a href="https://github.com/Graylog2/graylog2-server/stargazers"><img src="https://img.shields.io/github/stars/Graylog2/graylog2-server?style=social&color=white" alt="Graylog2/graylog2-server stars"/></a> | SSPL | Centralized log management & security search platform featuring structured parsing, stream routing, & real-time alerting. |
| **[Zeek Network Security Monitor](https://github.com/zeek/zeek)** | <a href="https://github.com/zeek/zeek/stargazers"><img src="https://img.shields.io/github/stars/zeek/zeek?style=social&color=white" alt="zeek/zeek stars"/></a> | BSD-3-Clause | Deep network traffic analyzer & metadata generator providing structured protocol logs for SIEM threat hunting. |
| **[Suricata NIDS](https://github.com/OISF/suricata)** | <a href="https://github.com/OISF/suricata/stargazers"><img src="https://img.shields.io/github/stars/OISF/suricata?style=social&color=white" alt="OISF/suricata stars"/></a> | GPLv2 | High-performance Network Intrusion Detection (NIDS), IPS, and network security monitoring engine feeding event logs into SIEMs. |
| **[MISP Threat Intelligence](https://github.com/MISP/MISP)** | <a href="https://github.com/MISP/MISP/stargazers"><img src="https://img.shields.io/github/stars/MISP/MISP?style=social&color=white" alt="MISP/MISP stars"/></a> | AGPL-3.0 | Open-source threat intelligence sharing platform (IoCs, threat actors, vulnerability indicators) integrating with SIEM platforms. |
| **[Cuckoo Sandbox](https://github.com/cuckoosandbox/cuckoo)** | <a href="https://github.com/cuckoosandbox/cuckoo/stargazers"><img src="https://img.shields.io/github/stars/cuckoosandbox/cuckoo?style=social&color=white" alt="cuckoosandbox/cuckoo stars"/></a> | GPLv3 | Automated malware analysis system generating forensic behavioral logs for SOC incident triage & SIEM correlation. |
| **[OSSEC HIDS](https://github.com/ossec/ossec-hids)** | <a href="https://github.com/ossec/ossec-hids/stargazers"><img src="https://img.shields.io/github/stars/ossec/ossec-hids?style=social&color=white" alt="ossec/ossec-hids stars"/></a> | GPLv2 | Open-source Host Intrusion Detection System providing log analysis, file integrity monitoring (FIM), and active response. |
| **[Security Onion](https://github.com/Security-Onion-Solutions/securityonion)** | <a href="https://github.com/Security-Onion-Solutions/securityonion/stargazers"><img src="https://img.shields.io/github/stars/Security-Onion-Solutions/securityonion?style=social&color=white" alt="Security-Onion-Solutions/securityonion stars"/></a> | GPLv3 | Complete Linux distribution for threat hunting, enterprise security monitoring, network metadata, full packet capture, & log management. |
| **[TheHive Incident Response](https://github.com/TheHive-Project/TheHive)** | <a href="https://github.com/TheHive-Project/TheHive/stargazers"><img src="https://img.shields.io/github/stars/TheHive-Project/TheHive?style=social&color=white" alt="TheHive-Project/TheHive stars"/></a> | AGPL-3.0 | Scalable 4-in-1 Security Incident Response Platform (SIRP/SOAR) designed to ingest SIEM alerts & streamline analyst investigations. |
| **[Snort 3 NIPS](https://github.com/snort3/snort3)** | <a href="https://github.com/snort3/snort3/stargazers"><img src="https://img.shields.io/github/stars/snort3/snort3?style=social&color=white" alt="snort3/snort3 stars"/></a> | GPLv2 | Next-generation network intrusion prevention system sending real-time attack events and anomaly telemetry to SIEM collectors. |
| **[Shuffle SOAR](https://github.com/Shuffle/Shuffle)** | <a href="https://github.com/Shuffle/Shuffle/stargazers"><img src="https://img.shields.io/github/stars/Shuffle/Shuffle?style=social&color=white" alt="Shuffle/Shuffle stars"/></a> | CC-BY-4.0 | Open-source Security Orchestration, Automation, and Response (SOAR) platform for workflow automation with SIEMs. |
| **[Matano Data Lake SIEM](https://github.com/matanolabs/matano)** | <a href="https://github.com/matanolabs/matano/stargazers"><img src="https://img.shields.io/github/stars/matanolabs/matano?style=social&color=white" alt="matanolabs/matano stars"/></a> | Apache-2.0 | Serverless AWS-native security data lake SIEM storing Apache Iceberg Parquet files on S3 with Python detection-as-code. |
| **[Panther Analysis Rules](https://github.com/panther-labs/panther-analysis)** | <a href="https://github.com/panther-labs/panther-analysis/stargazers"><img src="https://img.shields.io/github/stars/panther-labs/panther-analysis?style=social&color=white" alt="panther-labs/panther-analysis stars"/></a> | Apache-2.0 | Public detection-as-code repository containing Python detection rules and schemas for Panther cloud security analytics. |

---

## 🛠️ Complementary Detection & Collector Tools

While not standalone SIEMs, these critical security utilities feed essential telemetry into SIEM indexers:

- **[Snort 3](https://github.com/snort3/snort3)** — Network IDS/IPS for packet inspection & protocol analysis.
- **[Suricata](https://github.com/OISF/suricata)** — Multi-threaded network threat monitoring engine.
- **[Zeek](https://github.com/zeek/zeek)** — Protocol metadata parser delivering structured JSON network logs.
- **[Vector](https://github.com/vectordotdev/vector)** — Lightweight log transform & streaming pipeline.
- **[Fluentd](https://github.com/fluent/fluentd)** — Universal log collector and shipper.

---

## 🤝 How to Contribute

Contributions are warmly welcomed! Please follow these simple steps:

1. **Fork** this repository.
2. Create your feature branch (`git checkout -b feature/add-new-siem`).
3. Add your entry under the corresponding table in proper alphabetical or metric order.
4. Ensure factual descriptions, exact link URLs, and verified pricing/star metrics.
5. Submit a **Pull Request** with a brief summary of additions.

See our awesome list guidelines at **[Awesome-Awesome-Awesome](https://github.com/ishandutta2007/Awesome-Awesome-Awesome)**.

---

## ⚠️ Disclaimer & Trade-Off Analysis

> 💡 **Engineering Overhead vs SaaS Cost**: Open-source SIEMs require ongoing infrastructure management (index lifecycle management, rule tuning, agent patching). A senior security engineer dedicated to maintaining open-source SIEM infrastructure typically costs more annually than mid-tier commercial SaaS licenses.

- **Data Privacy**: SIEM platforms process high-density security logs that may contain PII or secret credentials. Ensure data masking and access controls.
- **Hardware Sizing**: Security Onion standalone nodes require a minimum of 24 GB RAM (32 GB+ recommended). Wazuh single-node requires 8 vCPUs / 16 GB RAM for 5,000–10,000 Events Per Second (EPS).
- **Maintenance Windows**: Ensure support windows for self-hosted components (e.g., Graylog versions 6.2/6.3 reach EOL by mid-2026).

---

## 📈 Star History

[![Star History Chart](https://star-history.dera.page/svg?repos=ishandutta2007/Awesome-Security-Information-And-Event-Management-SIEM&type=date&legend=top-left)](https://star-history.dera.page/#ishandutta2007/Awesome-Security-Information-And-Event-Management-SIEM&type=date&legend=top-left)

---

## 💖 Support & Sponsorship

Thank you for exploring the **Awesome Security Information & Event Management (SIEM)** repository! If this resource has helped your SOC team, security research, or infrastructure design, please consider supporting the project:

- 🌟 **Star this repository** to help others discover it.
- 🔀 **Fork and share** it with your fellow security analysts and DevOps engineers.
- ☕ **Sponsor / Buy me a coffee**: Support ongoing maintenance and curated security tooling lists via the [GitHub Sponsor Dashboard](https://github.com/sponsors/ishandutta2007).

<p align="center">
  <a href="https://github.com/sponsors/ishandutta2007">
    <img src="https://img.shields.io/badge/Sponsor-%E2%9D%A4-pink?style=for-the-badge&logo=github" alt="Sponsor on GitHub" />
  </a>
</p>

---

<p align="center">
  <i>Made with ❤️ for security analysts, threat hunters, and SOC engineering teams worldwide.</i>
</p>
