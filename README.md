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

## 🧪 Beispiel-Usecase: Portscan-Erkennung

1. .pcap-Datei mit Nmap-Scan (z. B. SYN-Flood) in Testnetz einspielen  
2. Snort erkennt Aktivität via Regel: `sid:1000001; msg:"Possible Nmap SYN Scan";`  
3. Ereignis erscheint in Splunk → Dashboard zeigt Quelle, Ziel, Portverteilung  
4. Awareness-Dokumentation erklärt Angriff, Erkennung, Auswirkung

🔗 Weitere Usecases: siehe `docs/usecases/` (folgt)


📷 Screenshots (folgt)



🚧 Status
🟡 In Überarbeitung (Stand: Juni 2025)
Verbesserte Regelbasis, Visualisierung & Trainingsmaterialien folgen sukzessive.

🤝 Mitmachen
Pull Requests, Feedback oder Kollaboration im Detection-Bereich sind willkommen.
Kontakt via GitHub oder LinkedIn/Xing (siehe Profil).

🛡️ Lizenz
MIT License – frei nutzbar & veränderbar.
Hinweis: Projekt dient ausschließlich zu Schulungs-, Awareness- und Demonstrationszwecken.

„Real Security is not silence. It’s Detection. Documentation. Repeatability.“
– Sergiu-Gelu Stoica

