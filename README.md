🔐 Praxisnahe Testumgebung für Intrusion Detection & Awareness - dokumentiert, messbar, wiederholbar.

🏠 Casa IDS Lab – Realistische Detection-Architektur für Heim- und KMU- und Schulnetzwerke

Casa IDS Lab ist eine modular aufgebaute Testumgebung für praxisnahe Intrusion Detection, Loganalyse und Security Awareness.  
Das Ziel: Detection. Dokumentation. Repeatability.
Für alle, die IT Sicherheit nicht nur denken - sondern umsetzen und dokumentieren.
---

🔍 Zielsetzung
Praxisnahe Testumgebung zur Entwicklung effektiver Intrusion Detection, klarer Log-Analyse und dokumentierter Security Awareness

- Aufbau und Test von IDS-Mechanismen (Snort-basiert)
- Visualisierung von Events via Splunk / SIEM
- Analyse echter Netzwerkverkehrsdaten (.pcap)
- Erstellen und Evaluieren eigener Detection Rules
- Vorbereitung auf Blue-Team- & SOC-Rollen

---

 Features 

- IDS-Integration mit Snort (regelbasiert, anpassbar)
- Beispielhafte Netzwerkverkehrsdaten im .pcap-Format
- Splunk Dashboard zur Visualisierung & Analyse
- Awareness-Dokumentation & Usecase-Beschreibung
- Modulares System - erweiterbar für verschiedene Szenarien

⚙️ Komponenten

| Komponente      | Funktion                                |
|-----------------|-----------------------------------------|
| 🐷 Snort       | Paketbasierte Angriffserkennung          |
| 📊 Splunk      | Log-Sammlung, Filterung & Visualisierung    |
| 🐧 Linux Host  | Syslog, pcap-Verarbeitung & Testautomatisierung          |
| 📦 Testdaten   | Reale Netzwerkverkehrsquellen     |
| 🧠 Awareness   | Tutorials, Usecases, Erklärung     |
| O Scripts       | Bash/Python für Setup, Analyse & Automatisches Testing |

---

🔧 Beispiel-Usecase: Portscan-Erkennung

1. Nmap-SYN-Scan aus `test-pcaps/` ausführen  
2. Snort mit Regel `sid:1000001; msg:"Possible Nmap SYN Scan";` erkennen  
3. Splunk zeigt Quelle, Ziel und Portverteilung in Echtzeit  
4. Awareness-Doku erklärt Angriff, Abwehr und Auswirkungen

---

🧭 Projekt-Roadmap

- ✅ Snort 3 Lab & Testregeln eingerichtet  
- ✅ Syslog und PCAP-Handling automatisiert mit Bash/Python  
- 🔲 Splunk-Dashboards finalisieren & Screenshots einpflegen  
- 🔲 Regulatory Mapping (BSI/NIS2/OWASP/NIST) integrieren  
- 🔲 docs/usecases/ mit Home‑, KMU‑ & Schul‑Szenarien befüllen  
- 🔲 Visual Assets (`assets/`-Ordner) ergänzen  
- 🔲 PSAppDeployToolkit-Testfälle für automatisierte Pakete

---

 🛡️ Regulatory Alignment & Compliance Awareness

Das Casa IDS Lab orientiert sich nicht nur an technischen Best Practices, sondern integriert zunehmend regulatorische Anforderungen aus dem deutschen und europäischen Raum.

Berücksichtigte Frameworks & Standards:

- MITRE ATT&CK** – Taktikbasierte Detection-Logik
- OWASP Top 10** – Applikationssicherheit im Kontext von Angriffserkennung
- NIST Cybersecurity Framework (CSF)** – Strukturierte Sicherheitsmaßnahmen entlang Identify–Protect–Detect–Respond–Recover
- BSI IT-Grundschutz (DE)** – Erste Mapping-Ansätze zur Anpassung auf KMU-Infrastrukturen
- NIS2-Richtlinie (EU)** – Kritische Analyse der Auswirkungen auf Detection-Strategien

Ziel ist es, realistische Heim- und KMU-Szenarien nicht nur technisch, sondern auch regulatorisch zu modellieren. So entsteht ein Verständnis für:

- Mindestanforderungen nach BSI & NIS2
- Umsetzbare Maßnahmen mit Open Source Tools (Snort, Suricata, Splunk)
- Machbarkeit im Rahmen von Automatisierung & Ressourcenengpässen

🎯 Use-Case:**
> Das Projekt eignet sich ideal als Demonstrator für KMU, Schulen oder Organisationen mit Compliance-Bedarf und begrenzten Budgets. Es zeigt, dass Detection, Awareness und Reporting nicht nur Sache großer Konzerne ist.

---

🔄 Status & Roadmap

🧪 BSI/NIS2-Mapping ist aktiv in Arbeit. Erste Überlegungen betreffen:

- Zuordnung technischer Controls zu BSI-Standards
- Bedrohungskataloge (z. B. nach IT-Grundschutz-Kompendium)
- Melde- und Reaktionspflichten gemäß NIS2

📍*Work in Progress – Anregungen und Pull Requests willkommen.*


📁 Verzeichnisstruktur

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
🟡 Stand Juni 2025
"Readme überarbeitet"
"Regelverzeichnis aktualisiert"
"Visualisierung in Vorbereitung"
"Weiter Usecases folgen im docs/ -Ordner"

🤝 Mitmachen
Pull Requests, Feedback oder Kollaboration im Detection-Bereich sind willkommen.
Kontakt via GitHub oder LinkedIn/Xing (siehe Profil).

🛡️ Lizenz
MIT License – frei nutzbar & veränderbar.
Hinweis: Projekt dient ausschließlich zu Schulungs-, Awareness- und Demonstrationszwecken.

„Real Security is not silence. It’s Detection. Documentation. Repeatability.“  – Sergiu-Gelu Stoica

