---
tags:
  - informational
  - monitoring
  - in-progress
  - tools
Creation date: Wednesday August 6th 2025
---
On the server with BMS, [[Grafana]] is used in tandem. Both are ran using Proxmox LXCs.
#### Key Aspects 
- **Time Series Database**
	A time series database are sequences of data points indexed by time. This allows for efficient storage and querying of historical data, enabling trend analysis and performance monitoring over time.
- **Exporters**
	 Exporters *(specialized tools)* are used to gather metrics from various sources. Exporters convert the data into a format that Prometheus understands and expose it via HTTP endpoints.
- **Pull-Based Architecture/Scraper**
	Actively fetches metrics from configured targets *(e.g., applications, servers)* using HTTP requests. This contrasts with push-based systems where targets send metrics to a central server.
- **Integration with Grafana**
	Allows users to create dynamic dashboards and visualizations based on the metrics collected by Prometheus
- **Alerting and Monitoring**
	It can track metrics from various sources, including applications, databases, and infrastructure components. Prometheus also provides alerting capabilities, allowing users to define rules and receive notifications when certain thresholds are breached
#### Links:
1. [What is Prometheus](https://www.google.com/search?q=what+is+prometheus&oq=what+is+prometheus&gs_lcrp=EgZjaHJvbWUyDAgAEEUYORixAxiABDIHCAEQABiABDIHCAIQABiABDIHCAMQABiABDIHCAQQABiABDIHCAUQABiABDIHCAYQABiABDIHCAcQABiABDIHCAgQABiABDIHCAkQABiABNIBCDQxMzJqMGo3qAIAsAIA&client=ubuntu-chr&sourceid=chrome&ie=UTF-8)
2. [Community Script Install](https://community-scripts.github.io/ProxmoxVE/scripts?id=prometheus)
3. [Community Script Exporter Install](https://community-scripts.github.io/ProxmoxVE/scripts?id=prometheus-pve-exporter)