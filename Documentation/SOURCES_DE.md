# SOURCES_DE.md

## HGT Ableton Extensions

**Projekte:** Genre Converter · Genre Remap · Drum Construction Kit\
**Dokumentationssprache:** Deutsch\
**Letzte Überarbeitung:** 19. November 2026

Dieses Dokument erfasst die wesentlichen musikalischen, technischen und
gestalterischen Referenzen der HGT-Ableton-Extensions. Außerdem
beschreibt es die Herkunft der eigens für die Projekte erstellten
visuellen und klanglichen Bestandteile.

Die drei Extensions sind eigenständige Projekte. Sie haben teilweise
eine gemeinsame Entwicklungsgeschichte und verwenden -- soweit
dokumentiert -- einzelne gemeinsame Assets oder Entwicklungskonzepte.

------------------------------------------------------------------------

## 1. Projekt- und Entwicklungsumfeld

Die Extensions werden für Ableton Live und das
Ableton-Extensions-Framework entwickelt.

-   **Host-Anwendung:** Ableton Live. Entwicklung und Tests fanden auch
    mit Ableton Live 13 Beta statt.
-   **Extension-Framework:** Ableton Extensions SDK.
-   **JavaScript-Laufzeitumgebung:** Node.js. Für die jüngere
    Entwicklungsumgebung ist Node.js 24.16.0 dokumentiert.
-   **Paketverwaltung und Build-Werkzeuge:** npm. In der dokumentierten
    Entwicklungsumgebung wurde npm 11.13.0 verwendet.
-   **TypeScript:** In der Entwicklungsumgebung wurde Version 5.9.3
    eingesetzt.

Diese Angaben beschreiben dokumentierte Entwicklungsstände. Sie bedeuten
nicht, dass jede veröffentlichte Version exakt dieselben
Werkzeugversionen verwendet. Maßgeblich sind jeweils das konkrete
Release-Paket und dessen Build-Konfiguration.

## 2. Musikalische und pädagogische Referenzwerke

Die folgenden Veröffentlichungen dienen als Hintergrund- und
Lernmaterial für Drum-Programming, rhythmisches Vokabular und
musikalische Arrangements. Ihre Nennung dokumentiert Quellen der
Beschäftigung und Inspiration. Sie bedeutet nicht, dass urheberrechtlich
geschützte Buchseiten, vollständige Arrangements oder komplette
Patternfolgen in den Extensions vervielfältigt werden.

### 2.1 *260 Drum Machine Patterns*

-   **Autor:** René-Pierre Bardet
-   **Verlag:** Hal Leonard
-   **Erscheinungsjahr:** 1987
-   **ISBN:** 978-0-88188-887-4
-   **Nachweis:** [Google Books -- 260 Drum Machine
    Patterns](https://books.google.com/books?id=WGMnPQAACAAJ)

Die Veröffentlichung dient als Referenz für Drum-Machine-Patterns und
rhythmische Konzepte. Die Projektdokumentation führt sie als
musikalisches Referenzwerk. Vollständige Notationsseiten oder komplette
Patternfolgen aus dem Buch sollen nicht als Bestandteil der Extensions
übernommen werden.

### 2.2 *Roland Drum Machine Rhythm Dictionary*

-   **Autor:** Sandy Feldstein
-   **Verlag:** Alfred Publishing Co., Inc.
-   **Copyright/Erscheinungsjahr:** 1985
-   **Nachweis:** [Internet Archive -- Suche nach Roland Drum Machine
    Rhythm
    Dictionary](https://archive.org/search?query=%22Roland+Drum+Machine+Rhythm+Dictionary%22)

Das Buch ist ein praxisorientiertes Nachschlage- und Lehrwerk zur
Rhythmusprogrammierung mit Roland-Drumcomputern. Es behandelt
Drumcomputer-Rhythmen und Programmieransätze und stellt Patterns sowohl
in Notenschrift als auch in maschinenorientierter Form dar. Es wird als
musikalische und pädagogische Referenz genannt, nicht als Quelle für
eine vollständige Übernahme seiner Inhalte in die Extensions.

Der Titel bezieht sich auf Roland-Drumcomputer. Als Autor ist Sandy
Feldstein und als Verlag Alfred Publishing angegeben.

## 3. Technische Referenzen

### 3.1 Ableton Extensions SDK

-   **Herausgeber:** Ableton
-   **Dokumentation:** [Ableton Extensions
    SDK](https://ableton.github.io/extensions-sdk/)

Die offizielle SDK-Dokumentation ist die maßgebliche technische Referenz
für Entwicklung, Build und Paketierung von Ableton Extensions.

### 3.2 Ableton Live Extensions

-   **Herausgeber:** Ableton
-   **Referenz:** [Ableton Live --
    Extensions](https://www.ableton.com/en/live/extensions/)

Offizielle Übersicht zu Extensions und ihrer Funktion innerhalb von
Ableton Live.

### 3.3 Ableton Extensions FAQ

-   **Herausgeber:** Ableton
-   **Referenz:** [Ableton Hilfe -- Extensions
    FAQ](https://help.ableton.com/hc/en-us/articles/27303428331420-Ableton-Extensions-FAQ)

Offizielle Support-Informationen zu Ableton Extensions.

### 3.4 Node.js

-   **Herausgeber:** OpenJS Foundation
-   **Referenz:** [Node.js](https://nodejs.org/)

Node.js ist Bestandteil der JavaScript-basierten Entwicklungs- und
Build-Umgebung.

### 3.5 TypeScript

-   **Herausgeber:** Microsoft
-   **Referenz:**
    [TypeScript-Dokumentation](https://www.typescriptlang.org/docs/)

Die TypeScript-Dokumentation dient als technische Referenz für die
Entwicklung mit typisiertem JavaScript.

### 3.6 Projekt-Lizenzreferenz

-   **Lizenztext:** [PolyForm Noncommercial License
    1.0.0](https://polyformproject.org/licenses/noncommercial/1.0.0/)

Ein Entwicklungsprotokoll von Genre Remap 1.0.1 nennt die PolyForm
Noncommercial License 1.0.0. Welche Lizenz tatsächlich in einem
veröffentlichten Source-Archiv enthalten ist, muss anhand des jeweiligen
Releases geprüft werden. Dieses Quellenverzeichnis ersetzt oder
verändert keine `LICENSE`-Datei eines Releases.

## 4. Eigenständiges visuelles Design und Logo

Das HGT-Projektlogo und die dazugehörige visuelle Gestaltung sind eigene
Kreationen des Projekts.

Das Gestaltungskonzept ist von der **geometrischen Bildsprache Piet
Mondrians** inspiriert, insbesondere von geometrischen
Flächenaufteilungen, geraden Linien und kontrastierenden Farbfeldern.
Das Logo selbst wurde eigenständig für die HGT-Extensions gestaltet. Es
handelt sich weder um eine Reproduktion noch um einen Scan eines
Mondrian-Gemäldes; auch wird kein Mondrian-Kunstwerk als Logo-Asset
eingebunden.

**Urheber-/Herkunftsangabe:** Eigenständige Gestaltung von HGT,
inspiriert von der geometrischen Kunstauffassung Piet Mondrians.

Die Angabe beschreibt einen künstlerischen Einfluss. Sie bedeutet keine
Unterstützung, Lizenzierung oder Zusammenarbeit mit dem
Mondrian-Nachlass oder anderen Rechteinhabern.

## 5. Audio-Assets und Herstellung der Sound-Samples

Die zehn MP3-Audio-Assets des dokumentierten Preview-Audio-Workflows
wurden von HGT mithilfe eines virtuellen Schlagzeuginstruments erstellt.

-   **Virtuelles Instrument:** Toontrack EZdrummer (VST-Instrument)
-   **Drum-Library / Kit:** Jazz Kit
-   **Preset:** `tightprog`
-   **Aufnahme- und Bearbeitungsumgebung:** Ableton Live
-   **Herstellungsprozess:** Die Audioausgabe des Instruments wurde in
    Ableton Live aufgenommen, bearbeitet und anschließend als
    MP3-Dateien gerendert/exportiert.
-   **Dateiformat:** MP3 mit 320 kbit/s für den dokumentierten
    Asset-Satz.

Bei diesen Dateien handelt es sich um im Projekt erzeugte
Audio-Renderings der EZdrummer-Wiedergabe. Sie werden nicht als
unbearbeitete Original-Samples von Toontrack oder als Aufnahmen eines
akustischen Schlagzeugs ausgegeben.

Das zugrunde liegende virtuelle Instrument, die Inhalte des Jazz Kits
und das Preset sind Produkte von Toontrack. Rechte und zulässige
Nutzungen des Instrumenteninhalts und der daraus gerenderten
Audiodateien richten sich nach den jeweils geltenden
Toontrack-Lizenzbedingungen. Dieses Dokument hält die Herstellung und
Herkunft fest, trifft aber keine eigenständige rechtliche Aussage über
eine mögliche Weiterverbreitung.

Wenn eine Extension diese MP3-Dateien enthält, sind die zugehörigen
Third-Party-Hinweise und die geltenden Toontrack-Bedingungen gemeinsam
zu berücksichtigen.

## 6. MIDI-Material und Referenzen für die Pattern-Entwicklung

In der Entwicklungsgeschichte werden MIDI-Dateien genannt, die zur
Analyse, zum Testen, zum Vergleichen und für musikalische Experimente
verwendet wurden. Ein dokumentierter Entwicklungsstand von Genre Remap
verweist beispielsweise auf die Datei `093 Chicken A.mid`, die als
viertaktige MIDI-Referenz mit ungefähr 93 BPM beschrieben wird.

In der Entwicklungsumgebung befinden sich außerdem
MIDI-Pattern-Sammlungen mit Bezeichnungen wie `Instant Drum Patterns`,
`200 Patterns Type 0` und `260 Patterns Type 0`.

Diese Bezeichnungen dokumentieren Material, das im Entwicklungs- und
Testablauf verwendet oder vorgefunden wurde. Sie belegen für sich allein
weder den ursprünglichen Autor noch den Rechteinhaber, die Lizenz oder
eine Erlaubnis zur Weiterverbreitung jeder einzelnen MIDI-Datei.
MIDI-Dateien sollten deshalb nur dann mit einem Release weitergegeben
werden, wenn ihre Herkunft und Lizenz geklärt sind oder feststeht, dass
es sich um eigens erstelltes Projektmaterial handelt.

Die musikalische Analyse und die für die Extensions entwickelte
Transformationslogik sind Projektarbeit. Die Verwendung einer MIDI-Datei
als Testeingabe bedeutet nicht, dass das Projekt Eigentümer dieser Datei
ist.

## 7. Projektspezifische Entwicklungsnachweise

Die folgenden internen Entwicklungsaufzeichnungen dokumentieren
Entscheidungen und Implementierungsarbeiten. Es handelt sich um
Projektunterlagen, nicht um externe Veröffentlichungen.

### 7.1 Genre Converter

Entwicklungsprotokolle dokumentieren genrespezifische Rhythmus-Banks,
Arrangement-Logik, Abschnittsbehandlung und Regressionstests. Ein
dokumentierter Verifikationsstand meldet gültige 4/4-Pattern-Banks pro
Instrumentenspur für 25 angefragte Genres.

### 7.2 Genre Remap

Entwicklungsprotokolle dokumentieren das Laden und Analysieren von
MIDI-Dateien, Genre-Konvertierungsregeln und Preview-Funktionen. Als
musikalische Referenzwerke werden unter anderem *260 Drum Machine
Patterns* und *Roland Drum Machine Rhythm Dictionary* genannt. Ein
Entwicklungsprotokoll dokumentiert außerdem `093 Chicken A.mid` als
Test- bzw. Referenzeingabe.

### 7.3 Drum Construction Kit

Entwicklungsprotokolle dokumentieren die Erstellung von Drum-Parts,
Fills, Variationen, Drummer-Profilen, Solo-Verhalten, Song-Abschnitten
und Audio-Preview-Funktionen. Ein dokumentierter Entwicklungsstand zur
Audio-Vorschau nennt zehn MP3-Dateien im Verzeichnis `assets/mp3-320`.
Wie in Abschnitt 5 beschrieben, handelt es sich dabei um
Projekt-Renderings aus EZdrummers Jazz Kit mit dem Preset `tightprog`.

## 8. Übersicht verwendeter Drittprodukte und Quellen

  ------------------------------------------------------------------------
  Bestandteil             Verwendung im Projekt    Herkunft / Zuordnung
  ----------------------- ------------------------ -----------------------
  Ableton Live            Host-Anwendung und       Ableton
                          Aufnahmeumgebung         

  Ableton Extensions SDK  Entwicklungs-Framework   Ableton
                          für Extensions           

  Node.js                 JavaScript-Laufzeit und  OpenJS Foundation
                          Build-Umgebung           

  TypeScript              Entwicklung mit          Microsoft
                          typisiertem JavaScript   

  EZdrummer -- Jazz Kit,  Virtuelle                Toontrack
  `tightprog`             Schlagzeugquelle für die 
                          erstellten               
                          Audio-Renderings         

  *260 Drum Machine       Musikalisches            René-Pierre Bardet; Hal
  Patterns*               Referenzwerk             Leonard

  *Roland Drum Machine    Musikalisches            Sandy Feldstein; Alfred
  Rhythm Dictionary*      Referenzwerk             Publishing

  HGT-Logo / visuelle     Eigenständige            Gestaltung von HGT;
  Identität               Projektgrafik            inspiriert von
                                                   Mondrians geometrischer
                                                   Bildsprache
  ------------------------------------------------------------------------

Diese Übersicht benennt Produkte und Referenzen. Sie ersetzt nicht die
Lizenztexte, Hinweise oder Nutzungsbedingungen der jeweiligen
Rechteinhaber.

## 9. Geltungsbereich und Aktualität

Dieses Dokument hält die anhand der Entwicklungsunterlagen
identifizierten Quellen und Asset-Herkünfte sowie die vom
Projektverantwortlichen klargestellten Angaben fest. Es soll dem
Source-Code jeder Extension beigefügt und aktualisiert werden, sobald
eine neue externe Abhängigkeit, musikalische Referenz, Grafik oder
Audio-Datei hinzukommt.

Für jedes Release sind das tatsächlich ausgelieferte Source-Archiv, die
Dependency-Manifeste, die enthaltenen Lizenzdateien und die gebündelten
Assets maßgeblich. Aus der Verwendung eines Bestandteils während der
Entwicklung darf nicht automatisch auf Eigentum oder
Weiterverbreitungsrechte geschlossen werden.

------------------------------------------------------------------------

**HGT -- Genre Converter · Genre Remap · Drum Construction Kit**
