# HGT Ableton Extensions — Quellen und Drittanbieterhinweise

**Aktuell dokumentierte Versionen**
- Drum Construction Kit 0.7.0
- Genre Remap 3.3.0
- Genre Converter 9.6.2

Dieses Dokument fasst die Quellen und Kompatibilitätshinweise zusammen, die in den bereitgestellten Source-Paketen dieser Versionen dokumentiert sind. Die einzelnen Extension-Pakete enthalten jeweils eigene Dateien zu `LICENSE`, `SOUND-ASSETS` und `THIRD-PARTY-NOTICES`. Für release-spezifische Formulierungen sind diese Paketdateien maßgeblich.

## 1. Audio-Material — Phazite Sounds

Alle drei aktuellen Extensions enthalten 37 eingebettete MP3-Audio-Payloads aus **Phazite Sounds**:

- Quellprojekt: https://github.com/august-byrne/phazite-sounds
- Angegebene Lizenzwidmung der Sounds: **CC0 1.0 Universal**
- CC0-Lizenztext: https://creativecommons.org/publicdomain/zero/1.0/

Der Soundbestand umfasst jeweils vier Velocity-Layer für Kick, Snare, Rim / Side Stick, Low Tom, Mid Tom, High Tom, Closed Hi-Hat, Open Hi-Hat und Ride (36 Payloads) sowie einen eigenen Crash-One-Shot mit langem Ausklang (1 Payload). Die dokumentierten MIDI-Velocity-Bereiche sind 1–31, 32–63, 64–95 und 96–127.

Die Source-Pakete enthalten Sound-Asset-Manifeste mit SHA-256-Prüfsummen und Dateigrößen der eingebetteten MP3-Payloads. Die ursprünglichen WAV-/FLAC-Aufnahmen werden in diesen Source-Paketen nicht als lose Dateien weitergegeben. Die MP3-Payloads sind entsprechend der jeweiligen Projektdokumentation in der Anwendung beziehungsweise Quellrepräsentation eingebettet.

Das Phazite-Projekt unterscheidet seine Sounddateien vom Anwendungscode. Die Extensions verwenden ausschließlich die Sounddateien und enthalten keinen Phazite-Anwendungscode. CC0 verlangt keine Namensnennung; HGT nennt die Quelle freiwillig aus Gründen der Transparenz.

**Hinweis zum Umfang:** Die CC0-Angabe entspricht der Lizenzdeklaration des Phazite-Projekts und den bereitgestellten HGT-Manifests. Diese Dokumentation hält die Herkunft fest, stellt aber keine unabhängige rechtliche Bestätigung sämtlicher Rechte an den ursprünglichen Aufnahmen dar.

## 2. Toontrack / EZdrummer — ausschließlich MIDI-Zuordnung

Toontrack und EZdrummer sind in den aktuellen Versionen keine Quellen für Audio-Material. Es sind keine Toontrack-/EZdrummer-Aufnahmen, Samples, Presets, Programme, Logos oder sonstigen Produktdateien enthalten.

Wenn eine Extension ein Toontrack-/EZdrummer-Drumlayout anbietet, bezeichnet der Produktname **ausschließlich eine MIDI-Noten-Zuordnung beziehungsweise Kompatibilitätsoption**. Damit wird beschrieben, welchen Schlagzeug-Instrumenten MIDI-Noten zugeordnet werden. Es werden dadurch keine Toontrack-Audios verwendet oder weitergegeben.

Toontrack und EZdrummer sind Produktnamen beziehungsweise Marken ihrer jeweiligen Rechteinhaber. Die Nennung dient ausschließlich der Kennzeichnung technischer Kompatibilität und bedeutet weder Unterstützung noch Partnerschaft oder geschäftliche Verbindung.

## 3. Weitere MIDI-Mapping-Referenzen

Je nach Extension können Produktnamen wie Native Instruments Battery/Kontakt oder Korg Drumlogue als MIDI-Mapping- beziehungsweise Kompatibilitätsreferenzen erscheinen. Diese Angaben bezeichnen ausschließlich Notenlayouts. Sie bedeuten nicht, dass Aufnahmen, Samples, Presets, Software oder andere Produktdateien dieser Hersteller enthalten sind.

## 4. Ableton Extensions SDK

Die Extensions wurden für Ableton Live unter Verwendung des Ableton Extensions SDK entwickelt. Die bereitgestellten Pakete enthalten den SDK-Lizenztext und dokumentieren die Trennung zwischen SDK-Laufzeitbestandteilen und Build-Werkzeugen. Das SDK bleibt Material von Ableton und wird durch HGT nicht neu lizenziert.

- Ableton: https://www.ableton.com/
- Ableton Marken- und Trademark-Richtlinien: https://www.ableton.com/en/legal/branding-trademark-guidelines/

Maßgeblich sind die SDK-Bedingungen, die Ableton für die beim jeweiligen Release verwendete SDK-Version bereitstellt. Siehe `ABLETON-EXTENSIONS-SDK-LICENSE.md` beziehungsweise die entsprechenden Drittanbieterhinweise im jeweiligen Source-Paket.

## 5. HGT-Grafiken und Logos

Die in den Extensions verwendeten HGT-Logos und grafischen Elemente sind eigene Gestaltungen von HGT. Ihre geometrische Formensprache ist von Piet Mondrian inspiriert. Es handelt sich nicht um Kopien, Reproduktionen oder weitergegebene Kunstwerke Mondrians.

## 6. HGT-Projektlizenzen

Jede Extension besitzt eine eigene projektbezogene HGT-Lizenzdatei. Diese Lizenzen gelten ausschließlich für ursprüngliches Projektmaterial, dessen Rechte HGT gehören oder von HGT kontrolliert werden. Sie ändern nicht die Lizenzbedingungen der Phazite-Sounds, der Ableton-SDK-Bestandteile, fremder Software oder Marken.

Die genauen Lizenzbezeichnungen und Bedingungen stehen in den jeweiligen Release-Paketen:
- Drum Construction Kit: `HGT License 1.0`
- Genre Remap: `HGT License 1.0`
- Genre Converter: `HGT Free Music Creator License 1.0`

Es handelt sich um projektbezogene Lizenzen, nicht um eine pauschale Lizenz für sämtliche Drittanbieter-Materialien und nicht notwendigerweise um OSI-anerkannte Open-Source-Lizenzen. Bitte immer die Lizenzdatei der jeweiligen Extension beachten.

## 7. Entwicklungswerkzeuge

Die bereitgestellten Source-Pakete dokumentieren Node.js und projektspezifische Build- und Testwerkzeuge, darunter je nach Projekt TypeScript und esbuild. Diese Werkzeuge dienen der Entwicklung und werden nicht als Audio-Material mitgeliefert. Es gelten die jeweiligen Upstream-Lizenzen.

## 8. Nutzung und Eigenverantwortung

Die HGT Ableton Extensions werden ehrenamtlich entwickelt und kostenlos zur Verfügung gestellt.

Sie werden mit Sorgfalt entwickelt und getestet. Dennoch lassen sich Fehler oder Inkompatibilitäten nicht vollständig ausschließen. Die Nutzung erfolgt in eigener Verantwortung.

Bitte sichere deine Ableton-Projekte und zugehörigen Dateien regelmäßig, insbesondere vor der Installation oder Aktualisierung einer Extension.

Eine Garantie für einen fehlerfreien oder unterbrechungsfreien Betrieb wird nicht übernommen. Die Haftung für Schäden oder Datenverluste ist im gesetzlich zulässigen Umfang ausgeschlossen. Zwingende gesetzliche Ansprüche bleiben unberührt.

## 9. Weitergabe und Änderungen

Die aktuellen Release-Pakete dokumentieren:
- 37 eingebettete MP3-Payloads aus Phazite Sounds unter der angegebenen CC0-1.0-Widmung;
- Integritätsprüfsummen für jede Payload in `SOUND-ASSET-MANIFEST.json`;
- getrennte HGT-Projektlizenzen und Ableton-SDK-Hinweise;
- keine Toontrack-/EZdrummer-Audioinhalte.

Für die genaue Herkunft einzelner Dateien, Prüfsummen, Build-Abgrenzungen und release-spezifischen Hinweise bitte die Dokumente im jeweiligen Source-ZIP heranziehen.

---
**HGT — Quellen- und Herkunftsnachweis**
