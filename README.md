# Poolpumpe PV-optimiert Advanced

Intelligenter Home-Assistant-Blueprint zur Steuerung einer Poolpumpe anhand von:

- Mindestlaufzeiten
- separaten Zeiten für Werktage und Wochenende
- PV-Überschuss
- optionalem Batteriespeicher
- optionaler Temperaturlogik
- optionaler Poolsperre

## Features

### Mindestlaufzeit
Die Poolpumpe läuft garantiert innerhalb definierter Zeitfenster.

### PV-Überschussnutzung
Zusätzliche Laufzeit bei vorhandenem Solarstrom-Überschuss.

### Wochenende / Werktage
Separate Zeitfenster möglich.

### Home Assistant kompatibel
Optimiert für:

- Home Assistant
- EVCC
- Shelly / Tasmota / Smart Plugs
- Photovoltaik-Anlagen
- Batteriespeicher

---

# Installation

## Variante 1: Direkt über GitHub

Blueprint importieren:

```text
https://github.com/zu3st-de/poolpumpe-blueprint
```

## Variante 2: Manuell

Datei kopieren nach:

```text
/config/blueprints/automation/poolpumpe/
```

Anschließend in Home Assistant:

```text
Einstellungen → Automatisierungen & Szenen → Blueprints
```

---

# Beispiel-Konfiguration

## Werktage

- 11:00 - 14:00 Uhr

## Wochenende

- 08:00 - 11:00 Uhr

## PV Überschuss

- Start ab 1500W Überschuss

---

# Empfehlung

Für kleinere Pools reicht häufig:

- 2x tägliche Umwälzung
- bevorzugt während PV-Überschuss
- zusätzliche Laufzeit bei heißem Wetter

---

# Lizenz

MIT License
