# 🏠 Casa IDS Lab – Realistische Detection-Architektur für Heim- und KMU-Netzwerke

**Casa IDS Lab** ist eine modular aufgebaute Testumgebung für praxisnahe Intrusion Detection, Loganalyse und Security Awareness.  
Das Ziel: **Detection. Dokumentation. Repeatability.**  
Gedacht für alle, die Sicherheit nicht nur denken – sondern nachweisen wollen.

---

## 🔍 Zielsetzung

- Aufbau und Test von IDS-Mechanismen (Snort-basiert)
- Visualisierung von Events via Splunk / SIEM
- Analyse echter Netzwerkverkehrsdaten (.pcap)
- Erstellen und Evaluieren eigener Detection Rules
- Vorbereitung auf Blue-Team- & SOC-Rollen

---

## ⚙️ Komponenten

| Komponente         | Funktion                                |
|--------------------|------------------------------------------|
| 🐍 **Snort**       | Paketbasierte Angriffserkennung          |
| 📊 **Splunk**      | Logsammlung, Analyse & Visualisierung    |
| 🐧 **Linux Host**  | Syslog, pcap-Handling, Testruns           |
| 📦 **Testdaten**   | Simulierter Netzwerkverkehr & Events     |
| 🧠 **Awareness**   | Schulungsunterlagen & Regelbeispiele     |

---

## 📁 Verzeichnisstruktur

```plaintext
Casa-IDS-Lab/
├── rules/                → Eigene Snort-Regeln
├── test-pcaps/           → Beispielhafte .pcap-Dateien
├── dashboards/           → Splunk Dashboards & Queries
├── docs/                 → Setup-Anleitungen & Visuals
└── scripts/              → Bash/Python für Setup & Analyse
