🔐 Cybersecurity: Web Threat Interaction
This project explores cyber threat detection through real-world web interaction data collected from a production web server using AWS CloudWatch. The goal is to analyze suspicious patterns, detect anomalies, and strengthen web application security using machine learning and data visualization.

📌 Project Objective
To detect, analyze, and classify patterns in web traffic to identify suspicious or potentially malicious activities such as unauthorized access, data breaches, and cyberattacks. The project focuses on leveraging anomaly detection techniques to uncover abnormal interaction behavior.

🗂️ Dataset Overview
Source: AWS VPC Flow Logs & CloudWatch monitoring

Type: Real-time web traffic logs with metadata

Key Features:

bytes_in, bytes_out

src_ip, dst_ip, dst_port, protocol

response_code, rule_names, detection_types

src_ip_country_code, observation_name

Usage: Threat intelligence, anomaly detection, security analytics

🧠 Techniques Used
Data Preprocessing:

Handling missing values, outliers, inconsistencies

Exploratory Data Analysis (EDA):

Summary stats, histograms, scatter plots, heatmaps

Feature Engineering:

Calculated duration, traffic_rate, avg_packet_size

Visualization:

Country-wise interactions, port-based suspicious activity

Anomaly Detection Model:

Isolation Forest with a contamination factor of 0.05

Labels: -1 (anomalous), 1 (normal)

📊 Key Visual Insights
Top countries & ports involved in suspicious activity

Scatter plots and pairplots highlighting anomalies

Geographic anomaly distribution using maps (optional)

🔍 Major Findings
Anomalies with high bytes_in but low bytes_out → possible exfiltration

Traffic spikes on critical ports like 22 (SSH), 3389 (RDP) → brute-force/DDoS

High-risk source IPs identified through repetitive short sessions

Geographic patterns revealing threat origin hotspots

✅ Recommendations
Enforce IP filtering and port restrictions

Use anomaly-based IDS for real-time detection

Conduct DPI and log correlation to investigate anomalies

Monitor traffic on non-standard ports proactively

💡 Potential Use Cases
Cybersecurity research

Intrusion Detection System (IDS) enhancement

Threat intelligence development

Security rule optimization

👩‍💻 Author
Sri Abhirami J. L

