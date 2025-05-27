# OpenData Exporter für contentdesk.io

Dieses Repository enthält ein Python-Skript, das Daten aus der Plattform [contentdesk.io](https://www.contentdesk.io) automatisiert ausliest und diese als maschinenlesbare Formate (`.json`, `.csv`) speichert.
Ziel ist es, diese Daten über eine öffentliche OpenData-Domain wie `https://opendata.domain.tld` Dritten zur Weiterverwendung zur Verfügung zu stellen.

---

## Funktion

Das Skript:

1. Stellt eine Verbindung zur API von contentdesk.io her.
2. Liest strukturierte Inhalte aus (z. B. touristische Daten, Events, Orte, etc.).
3. Exportiert diese Daten regelmäßig in zwei Formate:
   - **JSON**: Für Entwickler und APIs.
   - **CSV**: Für klassische Tabellenanwendungen.
4. Speichert die Dateien versioniert in diesem Git-Repository (Branch: `main`).

---

## Setup & Ausführung

### Voraussetzungen

- Python 3.10 oder höher
- Abhängigkeiten aus `requirements.txt` (oder in `pyproject.toml`, falls vorhanden)

### Installation

```bash
git clone https://github.com/TSO-AG/opendata.demo.contentdesk.io.git
cd opendata.demo.contentdesk.io
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
