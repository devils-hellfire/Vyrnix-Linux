# Vyrnix Linux

**Vyrnix Linux** ist eine minimalistische, modulare Linux-Distribution, inspiriert von der Klarheit und Struktur von FreeBSD und der Flexibilität von Arch Linux.

Das Ziel:  
👉 Ein schlankes, performantes System, das sich **automatisch an die Hardware anpasst**  
👉 Maximale Kontrolle ohne unnötigen Ballast  
👉 Klare Struktur statt Chaos

---

## 🧭 Philosophie

Vyrnix folgt einer Kombination aus:

### 🧱 BSD-Philosophie
- Klare Trennung von Systemkomponenten
- Modularer Aufbau
- Vorhersehbares Verhalten
- Fokus auf Einfachheit und Kontrolle

### ⚙️ Arch Linux Prinzipien
- KISS (Keep It Simple, Stupid)
- Rolling Release
- Nutzer hat die Kontrolle
- Minimale Defaults, maximale Anpassbarkeit

---

## 🧩 Architektur

Vyrnix ist **kein klassisches monolithisches System**, sondern:

- 🔹 **Modular aufgebaut** (ähnlich FreeBSD Ports / Modules)
- 🔹 Basierend auf Arch Linux als stabile Grundlage :contentReference  
- 🔹 Eigene Paketstruktur (`vyrnix-*`) für Hardware- und Systemmodule  
- 🔹 Eigene Repository-Struktur für Kernel + Module  

---

## 🚀 Konzept

### 1. Minimaler Base-Kernel

Ein bewusst reduzierter Kernel:

- ❌ Kein Debugging
- ❌ Kein Audit-System
- ❌ Keine unnötigen Energiesparfeatures
- ❌ Keine unnötigen Treiber
- ✅ Nur Boot + Netzwerk + Basisfunktionalität

➡️ Ziel: **Maximale Performance + minimale Komplexität**

Zusätzlich integriert:

- Kyber / BFQ I/O Scheduler  
- PDS Scheduler  
- 1000Hz Scheduling  
- Hard Kernel Preemption  
- TCP BBR2  

:contentReference[oaicite:2]{index=2}

---

### 2. Hardware-Erkennung nach Installation

Nach dem ersten Start:

1. Hardware-Scan wird durchgeführt  
2. Nur notwendige Module werden installiert  
3. System bleibt minimal und effizient  

Beispiel: "vyrnix-hwdetect scan"


➡️ Kein unnötiger Ballast. Kein generisches System.

---

### 3. Dynamische Systemprofile

Während Laufzeit umschaltbar:

- 🎮 Gaming
- ⚡ Realtime
- 💼 Office
- 🔋 Balanced

➡️ Umsetzung über Systemregeln (Runtime Switching)

---

### 4. Vyrnix Module System

Beispiele:

- `vyrnix-module-gpu-amd`
- `vyrnix-module-wifi-intel`
- `vyrnix-module-audio-pipewire`

➡️ Nur das, was wirklich gebraucht wird

---

## 🖱️ Usability Features

- Moused-Unterstützung in **jeder Shell** (wie FreeBSD)
- Funktionaler Maus-Support:
  - im Installer
  - im Live-System
  - im laufenden System

---

## 💿 Installer

Minimalistisch, klar, funktional:

### Auswahlmöglichkeiten:

- Sprache
- Tastatur
- Netzwerk (Ethernet / WLAN)
- Internetverbindung
- Laufwerke
- Partitionierung
- Benutzer
- Shell

➡️ **Keine unnötigen Optionen**

Zusätzlich:
- Installer bootet immer direkt
- Shell jederzeit verfügbar

---

## 🎯 Ziel von Vyrnix

Vyrnix ist gebaut für:

- 🧠 Leute, die verstehen wollen, wie ihr System funktioniert
- ⚡ Performance-Enthusiasten
- 🛠️ Minimalisten
- 🎮 Gamer / Realtime-User
- 🧩 Menschen, die modulare Systeme lieben

---

## ⚠️ Status

🚧 Work in Progress  
Dieses Projekt befindet sich aktiv im Aufbau.

---

## 🤝 Mitmachen

Contributions sind willkommen – besonders in:

- Kernel-Tuning
- Modul-System
- Installer
- Hardware Detection

---

## 📜 Lizenz

BSD-inspirierter Ansatz – offen, flexibel, frei.

---

## 💡 Vision

> Ein Linux-System, das nicht alles kann –  
> sondern genau das, was du brauchst.  

