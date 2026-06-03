# Poolpumpe PV-optimiert Advanced

Intelligenter Home-Assistant-Blueprint zur Steuerung einer Poolpumpe anhand von:

- Mindestlaufzeiten
- separaten Zeiten für Werktage und Wochenende
- PV-Überschuss
- optionalem Batteriespeicher
- manuellen Overrides
- optionaler Temperaturlogik
- optionaler Poolsperre

## Features

### Mindestlaufzeit
Die Poolpumpe läuft garantiert innerhalb definierter Zeitfenster.

### PV-Überschussnutzung
Zusätzliche Laufzeit bei vorhandenem Solarstrom-Überschuss.

### Wochenende / Werktage
Separate Zeitfenster möglich.

### Manueller Override
Unterstützt künftig:

- Poolpumpe für X Stunden erzwingen EIN
- Poolpumpe für X Stunden erzwingen AUS
- Bademodus
- Wartungsmodus

### Home Assistant kompatibel
Optimiert für:

- Home Assistant
- EVCC
- Shelly / Tasmota / Smart Plugs
- Photovoltaik-Anlagen
- Batteriespeicher

---

# Installation

Blueprint importieren über:

https://raw.githubusercontent.com/zu3st-de/poolpumpe-blueprint/main/blueprints/automation/poolpumpe/poolpumpe_pv_advanced.yaml

---

# Empfohlene Sensoren

## EVCC Überschuss

Sensor:

sensor.evcc_grid_power

Empfohlene Schwelle:

-500 W bis -1000 W

Negativ = Einspeisung / Überschuss
Positiv = Netzbezug

---

# Roadmap

## Version 1.1

- Manueller EIN-Override
- Manueller AUS-Override
- Laufzeit in Stunden definierbar

## Version 1.2

- Temperaturabhängige Mindestlaufzeit
- Automatische Umwälzungsberechnung

## Version 1.3

- Wetterprognose
- Algenprävention
- Pooltemperatur-Integration

---

# Lizenz

MIT License
