# 🛰️ Analyzing Network Traffic with Moloch and Elastic

## 📖 **Introduction**

While diving deeper into the realm of Cybersecurity, I decided to explore the inner workings of **network traffic** and how anomalies can be detected in real-time. This project titled **"Analyzing Network Traffic with Moloch and Elastic"** became a stepping stone for me to blend **packet inspection, data indexing, and visualization** — all in one flow.

The core goal was to integrate **Moloch** (now known as [Arkime](https://arkime.com)) with the **Elastic Stack** to build a robust network monitoring setup. This hands-on implementation sharpened my understanding of how professionals detect **suspicious behavior**, analyze **performance bottlenecks**, and draw insights from raw PCAP files.

---

## 🧰 **Tools & Technologies Used**

- 🧠 **Moloch (Arkime)** — Full packet capture and indexing system.
- 🧱 **Elasticsearch** — Distributed search and analytics engine.
- 📊 **Kibana** — Visualization layer for traffic patterns.
- 🔁 **Logstash** — Optional for ingest pipelines and filtering.
- 🧪 **Wireshark** — For deep packet inspection and PCAP parsing.
- 📂 **PCAP files** — Captured network traffic data.
- 🛡️ **SIEM Integration (Optional)** — For correlation with broader security systems.
- 🐧 **Ubuntu** — Deployment and testing environment.

---

## ⚙️ **Project Workflow**

1. **📥 Moloch Setup & Configuration**
   - Installed Arkime/Moloch on Ubuntu.
   - Configured interface to capture traffic (e.g., `eth0`).
   - Set up PCAP storage, viewer, and capture service.

2. **📡 Capturing Network Traffic**
   - Captured live traffic using Moloch or imported `.pcap` files via `moloch-capture`.
   - Verified session data in Moloch Viewer UI.

3. **🔍 Indexing & Storage (Elastic Integration)**
   - Moloch pushed metadata and indexes to **Elasticsearch**.
   - Defined index patterns in Kibana for querying sessions.

4. **📊 Visualization & Dashboarding**
   - Built dashboards in **Kibana** to view:
     - Top IP talkers
     - Anomalous port usage
     - Protocol-specific analysis (HTTP, DNS, etc.)

5. **🧠 Traffic Analysis**
   - Identified:
     - Suspicious activities (port scans, high data transfers)
     - Performance issues (packet loss, high RTT)
     - Protocol-level misuse

6. **✅ Final Audit**
   - Shared improvement suggestions for securing the network perimeter based on insights.

---

## 🗂️ **Repository Structure**

> 📁 Total Files: 7

- 📄 `setup_guide.md` — Step-by-step setup of Moloch and Elastic Stack.
- 📄 `pcap_samples/` — Contains demo `.pcap` files used during testing.
- 📄 `screenshots` — Visual outputs from Kibana and Moloch Viewer.
- 📄 `README.md` — You're here.

Each folder contains its own `README.md` (where required) for context-specific instructions.

---

## 📸 **Screenshots**

- 🖥️ `kibana-dashboard.png` — Overview of active sessions and traffic heatmap.
- 🧾 `moloch-session-view.png` — Detailed PCAP-level session drilldown.
- 🔍 `protocol-distribution.png` — Traffic by protocol breakdown (HTTP, DNS, TLS).

---

## 🎯 **Final Takeaway**

This project transformed raw network data into insightful security stories. For the first time, I worked with real traffic datasets to identify potential **threats**, **bottlenecks**, and **behavioral patterns**. It refined my understanding of:

- How packet data is captured and stored at scale.
- How Elastic’s search engine can be tailored for security.
- How visualization plays a key role in interpreting raw traffic.

Most importantly, I now see **network analysis as an art** — one that sits at the core of Cyber Defense.

---

## 🔗 **References / Learning Resources**

1. 📘 [Moloch Documentation](https://arkime.com/faq)
2. 📘 [Elastic Documentation](https://www.elastic.co/guide/index.html)
3. 📘 [Wireshark User Guide](https://www.wireshark.org/docs/wsug_html_chunked/)
4. 📘 [Intro to Network Traffic Analysis - Blog](https://www.varonis.com/blog/network-traffic-analysis)
5. 📘 [Tutorial: Moloch + Elastic](https://www.geeksforgeeks.org/using-arkime-moloch-for-network-traffic-analysis/)

---
