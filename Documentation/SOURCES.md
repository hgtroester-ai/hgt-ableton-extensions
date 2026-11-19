# SOURCES.md

## HGT Ableton Extensions

**Projects:** Genre Converter · Genre Remap · Drum Construction Kit\
**Documentation language:** English\
**Last revised:** 19 November 2026

This document records the principal musical, technical, and design
references used during the development of the HGT Ableton Extensions. It
also describes the origin of project-created visual and audio assets.

The three extensions are independent projects that share parts of their
development history and, where documented, selected assets or
implementation concepts.

------------------------------------------------------------------------

## 1. Project and development context

The extensions are developed for use with Ableton Live and the Ableton
Extensions framework.

-   **Host application:** Ableton Live. Development and testing have
    also taken place with Ableton Live 13 Beta.
-   **Extension framework:** Ableton Extensions SDK.
-   **JavaScript runtime:** Node.js. The development environment
    recorded for recent builds used Node.js 24.16.0.
-   **Package tooling:** npm. The recorded development environment used
    npm 11.13.0.
-   **TypeScript:** Version 5.9.3 was used in the development
    environment.

These are development-environment records, not a guarantee that every
release uses exactly the same versions. The applicable release package
and its build configuration remain authoritative.

## 2. Musical and educational references

The following publications are used as background references for drum
programming, rhythmic vocabulary, and musical arrangement. Their
inclusion identifies sources of study and inspiration; it does not mean
that copyrighted pages, complete arrangements, or pattern sequences are
reproduced in the extensions.

### 2.1 *260 Drum Machine Patterns*

-   **Author:** René-Pierre Bardet
-   **Publisher:** Hal Leonard
-   **Publication year:** 1987
-   **ISBN:** 978-0-88188-887-4
-   **Reference:** [Google Books -- 260 Drum Machine
    Patterns](https://books.google.com/books?id=WGMnPQAACAAJ)

This publication is a reference for drum-machine pattern concepts and
rhythmic vocabulary. The project documentation records it as a musical
reference. No complete notation pages or complete pattern sequences from
the book are intended to be reproduced as part of the extensions.

### 2.2 *Roland Drum Machine Rhythm Dictionary*

-   **Author:** Sandy Feldstein
-   **Publisher:** Alfred Publishing Co., Inc.
-   **Copyright/publication year:** 1985
-   **Reference:** [Internet Archive search -- Roland Drum Machine
    Rhythm
    Dictionary](https://archive.org/search?query=%22Roland+Drum+Machine+Rhythm+Dictionary%22)

The book is a practical rhythm-programming reference for Roland drum
machines. It covers drum-machine rhythms and programming approaches,
using written notation and machine-oriented pattern presentation. It is
included as a musical and educational reference, not as a source of
material reproduced wholesale in the extensions.

The title refers to Roland drum machines; the publication is credited to
Alfred Publishing and authored by Sandy Feldstein.

## 3. Technical references

### 3.1 Ableton Extensions SDK

-   **Publisher:** Ableton
-   **Documentation:** [Ableton Extensions
    SDK](https://ableton.github.io/extensions-sdk/)

The official SDK documentation is the primary technical reference for
building, packaging, and developing Ableton Extensions.

### 3.2 Ableton Live Extensions

-   **Publisher:** Ableton
-   **Reference:** [Ableton Live --
    Extensions](https://www.ableton.com/en/live/extensions/)

Official overview of the Extensions environment and its role in Ableton
Live.

### 3.3 Ableton Extensions FAQ

-   **Publisher:** Ableton
-   **Reference:** [Ableton Help -- Extensions
    FAQ](https://help.ableton.com/hc/en-us/articles/27303428331420-Ableton-Extensions-FAQ)

Official support information about Ableton Extensions.

### 3.4 Node.js

-   **Publisher:** OpenJS Foundation
-   **Reference:** [Node.js](https://nodejs.org/)

Node.js is used as part of the JavaScript-based development and build
environment.

### 3.5 TypeScript

-   **Publisher:** Microsoft
-   **Reference:** [TypeScript
    documentation](https://www.typescriptlang.org/docs/)

TypeScript documentation is a technical reference for typed JavaScript
development.

### 3.6 Project licence reference

-   **Licence text:** [PolyForm Noncommercial License
    1.0.0](https://polyformproject.org/licenses/noncommercial/1.0.0/)

A project development record for Genre Remap 1.0.1 identifies PolyForm
Noncommercial License 1.0.0. The licence actually included in each
published source archive must be checked for that release; this source
document does not replace or modify a release's `LICENSE` file.

## 4. Original visual design and logo

The HGT project logo and associated visual identity are original project
creations.

The visual concept takes inspiration from **Piet Mondrian's geometric
visual language**, particularly the use of geometric divisions, straight
lines, and areas of contrasting colour. The logo itself was
independently designed for the HGT extensions. It is not a reproduction,
scan, or reuse of a Mondrian painting, and no Mondrian artwork is
incorporated as the logo asset.

**Attribution:** Original visual design by HGT, inspired by the
geometric art approach associated with Piet Mondrian.

This description identifies an artistic influence; it does not imply
endorsement, sponsorship, or collaboration by the Mondrian estate or any
related rights holder.

## 5. Audio assets and sound sample production

The ten MP3 audio assets used in the documented preview-audio workflow
were created by HGT from performances of a virtual drum instrument.

-   **Virtual instrument:** Toontrack EZdrummer (VST instrument)
-   **Drum library / kit:** Jazz Kit
-   **Preset:** `tightprog`
-   **Recording and processing environment:** Ableton Live
-   **Production process:** The instrument output was recorded in
    Ableton Live, processed, and rendered/exported as WAV audio files.
-   **Recorded asset format:** converted as MP3, 320 kbit/s for the documented asset
    set.

These files are project-produced audio renderings of EZdrummer playback.
They are not represented as original dry samples supplied independently
by Toontrack, nor as recordings of a physical drum kit.

The underlying virtual instrument, Jazz Kit content, and preset remain
Toontrack products. The rights and permitted uses of the instrument
content and rendered output are governed by the applicable Toontrack
licence and terms. This document records the production provenance; it
does not make a legal determination about redistribution rights.

Where an extension package contains these MP3 files, the package's
accompanying third-party notices and the applicable Toontrack terms
should be considered together.

## 6. MIDI material and pattern-development references

The development history includes MIDI files used for analysis, testing,
comparison, and musical experimentation. One documented Genre Remap
development record refers to a file named `093 Chicken A.mid`, described
as a four-bar MIDI reference at approximately 93 BPM.

The development environment also contains MIDI pattern collections
identified by names such as `Instant Drum Patterns`,
`200 Patterns Type 0`, and `260 Patterns Type 0`.

These names identify material encountered in the development and testing
workflow. They do not, by themselves, establish the original author,
copyright owner, licence, or redistribution permission for every MIDI
file. MIDI files should therefore not be redistributed with a release
unless their provenance and licence have been established or the files
are confirmed to be project-created material.

Musical analysis and transformation logic developed for the extensions
are project work. The use of a MIDI file as a test input does not imply
ownership of that file.

## 7. Project-specific development references

The following internal development records document design decisions and
implementation work. They are project records rather than external
publications.

### 7.1 Genre Converter

Development records document genre-specific rhythm banks, arrangement
logic, section handling, and regression testing. A recorded verification
milestone reports valid per-lane 4/4 pattern banks across 25 requested
genres.

### 7.2 Genre Remap

Development records document MIDI loading and analysis, genre conversion
rules, preview functionality, and the use of musical references
including *260 Drum Machine Patterns* and *Roland Drum Machine Rhythm
Dictionary*. A development record also documents the use of
`093 Chicken A.mid` as a test/reference input.

### 7.3 Drum Construction Kit

Development records document the construction of drum parts, fills,
variations, drummer profiles, solo behaviour, song sections, and
preview-audio functionality. A recorded audio-preview development
milestone identifies ten MP3 assets in the `assets/mp3-320` folder. As
described in Section 5, these are project-produced renderings from
EZdrummer's Jazz Kit using the `tightprog` preset.

## 8. Third-party products and attribution summary

  -----------------------------------------------------------------------
  Item                    Role in the project     Origin / attribution
  ----------------------- ----------------------- -----------------------
  Ableton Live            Host application and    Ableton
                          recording environment   

  Ableton Extensions SDK  Extension development   Ableton
                          framework               

  Node.js                 JavaScript runtime and  OpenJS Foundation
                          build environment       

  TypeScript              Typed JavaScript        Microsoft
                          development             

  EZdrummer -- Jazz Kit,  Virtual drum instrument Toontrack
  `tightprog`             source used to create   
                          the recorded audio      
                          assets                  

  *260 Drum Machine       Musical reference       René-Pierre Bardet; Hal
  Patterns*                                       Leonard

  *Roland Drum Machine    Musical reference       Sandy Feldstein; Alfred
  Rhythm Dictionary*                              Publishing

  HGT logo / visual       Original project        Created by HGT;
  identity                artwork                 inspired by Mondrian's
                                                  geometric visual
                                                  language
  -----------------------------------------------------------------------

This table identifies products and references. It does not replace the
licence texts, notices, or terms supplied by their respective rights
holders.

## 9. Scope and accuracy

This document records the sources and asset origins identified in the
project development history and clarified by the project author. It
should be kept with the source code of each extension and updated when a
new external dependency, musical reference, visual asset, or audio asset
is introduced.

For each release, the actual source archive, dependency manifests,
included licence files, and bundled assets determine what is shipped. Do
not infer ownership or redistribution permission solely from an item
being used during development.

------------------------------------------------------------------------

**HGT -- Genre Converter · Genre Remap · Drum Construction Kit**
