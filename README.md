# Network Traffic Analyzer 🌐🔍🛡️

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)  
[![Python 3.x](https://img.shields.io/badge/Python-3.x-blue)](https://www.python.org/downloads/)

A Python-based tool for **capturing, inspecting, and analyzing network traffic**. This project helps users understand network behavior, detect unusual patterns, monitor data flow, and generate meaningful insights through automated traffic analysis.

## 🌟 Features

- **📶 Live Network Traffic Capture:** Real-time monitoring of active network interfaces.
- **📁 Offline Analysis:** Process saved packet capture files (`.pcap`) or custom data formats.
- **📊 Protocol Distribution Analysis:** Visualize and track the usage of various network protocols (TCP, UDP, ICMP, etc.).
- **🌐 Communication Tracking:** Identify and monitor data flow between source and destination IP addresses.
- **🚨 Anomaly Detection Module:** Use built-in models to flag suspicious patterns and potential threats.
- **📄 Export Logs and Reports:** Generate detailed reports and logs of the analysis results (optional feature).

## 🛠️ Requirements

- **Python 3.x**
- All required dependencies listed in `requirements.txt`.

### Installation

Install all necessary Python packages using pip:

```bash
pip install -r requirements.txt
```

## 🚀 Getting Started

1. Clone the Repository

```bash
git clone https://github.com/tejasparate1611/Network_traffic_analyzer.git
cd Network_traffic_analyzer
```

2. Install Dependencies

```bash
pip install -r requirements.txt
```

3. Run the Analyzer

Live Traffic Analysis

```bash
python Traffic_analyzer/main.py
```

Offline File Analysis

```bash
python analyzer/analyze.py path/to/file.pcap
```

> ⚠️ Note: Live network packet capture may require Administrator/Sudo privileges on most operating systems.

## ⚙️ Optional Arguments

The main execution scripts can support optional arguments for flexibility:

Argument | Description | Example
--|--|--
--interface <name> | Select the specific network interface to monitor. | --interface eth0
--mode live|offline | Explicitly define the capture mode. | --mode offline
--output <file> | Specify a file path to save the analyzed results/logs. | --output results.json
--threshold <value> | Adjust the sensitivity of the anomaly detection system. | --threshold 0.05

## 🧠 Anomaly Detection

The dedicated `anomaly_detection` module is crucial for security and performance monitoring. It actively looks for:

- Unusual spikes in traffic volume or connection counts.
- Suspicious port scanning or abnormal port activity.
- Irregular IP communication patterns.
- Protocol misuse or malformed packets.

Machine learning or heuristic models for detection can be implemented and stored inside the `models` directory.

## 📂 Project Structure

To help users understand the architecture of the project:

```markdown
.
├── README.md
├── requirements.txt
├── db.sqlite3
├── /Traffic_analyzer/       # Main execution scripts and Django settings
├── /analyzer/               # Core logic for packet inspection and analysis
├── /anomaly_detection/      # Logic for identifying unusual network activity
├── /models/                 # Stores machine learning models for detection
├── /network/                # Scripts for live capture and interface handling
├── /network_data/           # Stores captured data or supplementary files
└── /static/                 # Web assets (CSS, JS, Images) if using a web interface
```

## 🤝 Contributing

We welcome contributions to enhance this tool!

- Fork the repository.
- Create a new feature branch:

```bash
git checkout -b feature/new-feature
```

- Commit your changes:

```bash
git commit -m "feat: Add new feature"
```

- Push to the branch:

```bash
git push origin feature/new-feature
```

- Open a Pull Request describing your changes.

## ⚖️ License

This project is licensed under the MIT License.

## 📬 Author

Tejas Parate  
GitHub: https://github.com/tejasparate1611
