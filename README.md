# VokabelMeister – Barrierefreier Schriftlicher Vokabeltrainer (Android)

[![Build Android APK](https://github.com/Lauju1909/VokabelMeister-Android/actions/workflows/build-apk.yml/badge.svg)](https://github.com/Lauju1909/VokabelMeister-Android/actions/workflows/build-apk.yml)
[![GitHub Release](https://img.shields.io/github/v/release/Lauju1909/VokabelMeister-Android?color=blue&label=Release)](https://github.com/Lauju1909/VokabelMeister-Android/releases/latest)
[![Accessibility: TalkBack](https://img.shields.io/badge/A11y-TalkBack%20%26%20NVDA-success)](https://github.com/Lauju1909/VokabelMeister-Android)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

**VokabelMeister** ist ein 100% barrierefreier, rein schriftlicher Vokabeltrainer für Android. Die App richtet sich an alle Lernenden und ist speziell für Bildschirmleser (**TalkBack**) sowie Tastatursteuerung optimiert.

---

## ✨ Besonderheiten & Funktionen

- ✍️ **Reine schriftliche Abfrage:** Trainiere aktives Schreiben und Einprägen durch direkte Texteingabe.
- 🎯 **Intelligente Damerau-Levenshtein-Tippfehlertoleranz:** Verzeiht kleine Tippfehler und Buchstabendreher ("Fast richtig!"), ohne direkt als falsch gewertet zu werden.
- 🔀 **Flexible Klammer- und Schrägstrich-Auflösung:** Erkennt Kurzformen wie `(quer) über` oder `ein/e` vollautomatisch als gültige Antworten.
- 🧠 **Gewichtetes Kartensystem:** Vokabeln mit geringer Erfolgsquote werden häufiger wiederholt (Wiederholungsschutz: keine nervige Direkt-Wiederholung).
- 🏷️ **Kategorienverwaltung:** Fertig vorbefüllt mit über 1.700 Vokabeln aus Sprache (Englisch/Deutsch), Fachwörter, Formeln und Tastaturbefehle. Eigene Kategorien können frei erstellt werden.
- 🔊 **Text-to-Speech (TTS):** Liest Begriffe auf Wunsch automatisch in der passenden Sprache vor.
- 📥 **Umfangreicher Import:** Unterstützt Word (.docx), Excel (.xlsx / .csv), reine Textdateien (.txt) und JSON.
- 🔒 **100% Lokal & Sicher:** Keine Registrierung, kein Cloud-Zwang, kein Tracking. Alle Daten verbleiben auf deinem Gerät.

---

## 📲 Download & Installation

1. Lade die neueste Version direkt unter [GitHub Releases](https://github.com/Lauju1909/VokabelMeister-Android/releases/latest) herunter (`app-release.apk`).
2. Öffne die `.apk` auf deinem Android-Gerät und bestätige die Installation.
3. Automatische Updates sind über das [F-Droid Repository von Lauju1909](https://github.com/Lauju1909/fdroid-repo) verfügbar.

---

## 🛠️ Entwicklung & Build

### Voraussetzungen
- Node.js >= 22
- Java JDK 21
- Android SDK

### Lokaler Build
```bash
npm install
npx cap sync android
cd android
./gradlew assembleDebug assembleRelease
```

---

## 📜 Lizenz
Dieses Projekt steht unter der [MIT-Lizenz](LICENSE).
