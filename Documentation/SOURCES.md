# HGT Ableton Extensions — Sources and Third-Party Notices

**Current documented releases**
- Drum Construction Kit 0.7.0
- Genre Remap 3.3.0
- Genre Converter 9.6.2

This document records the source materials and compatibility references identified in the supplied source packages for these releases. The individual extension packages contain their own `LICENSE`, `SOUND-ASSETS` and `THIRD-PARTY-NOTICES` documents; those package files take precedence for release-specific wording.

## 1. Audio assets — Phazite Sounds

All three current extensions contain 37 embedded MP3 audio payloads derived from **Phazite Sounds**:

- Source project: https://github.com/august-byrne/phazite-sounds
- Declared sound-asset dedication: **CC0 1.0 Universal**
- CC0 deed: https://creativecommons.org/publicdomain/zero/1.0/

The sound set consists of four velocity layers each for Kick, Snare, Rim / Side Stick, Low Tom, Mid Tom, High Tom, Closed Hi-Hat, Open Hi-Hat and Ride (36 payloads), plus one dedicated long-decay Crash one-shot (1 payload). The documented MIDI velocity bands are 1–31, 32–63, 64–95 and 96–127.

The source packages include sound-asset manifests with SHA-256 hashes and byte lengths for the embedded MP3 payloads. The original WAV/FLAC recordings are not distributed as loose files in these source packages; the MP3 payloads are embedded in the application/source representation as documented by each project.

The Phazite project distinguishes its sound assets from its application code. The extensions use the sound assets only; they do not include Phazite application code. CC0 does not require attribution, but HGT provides this source credit voluntarily.

**Scope note:** The CC0 status above is the license declaration recorded by the Phazite project and the supplied HGT manifests. This document records that provenance; it is not an independent legal certification of upstream ownership.

## 2. Toontrack / EZdrummer — MIDI mapping reference only

Toontrack and EZdrummer are not sources of audio assets in the current releases. No Toontrack/EZdrummer recordings, samples, presets, software, logos or other product assets are included.

Where an extension offers a Toontrack/EZdrummer drum layout, the product name identifies a **MIDI note-mapping compatibility option only**. It describes how MIDI notes are assigned to drum instruments. It does not refer to or distribute Toontrack audio.

Toontrack and EZdrummer are product names/trademarks of their respective owner. Their mention is for compatibility identification only and does not imply endorsement, partnership or affiliation.

## 3. Other MIDI mapping references

Depending on the extension, product names such as Native Instruments Battery/Kontakt and Korg Drumlogue may appear as MIDI mapping or compatibility references. Such references identify note layouts only. They do not indicate that recordings, samples, presets, software or other product assets from those manufacturers are included.

## 4. Ableton Extensions SDK

The extensions are developed for Ableton Live using Ableton's Extensions SDK. The supplied packages include the SDK license text and describe the SDK runtime/build boundary. The SDK remains Ableton material and is not relicensed by HGT.

- Ableton: https://www.ableton.com/
- Ableton branding and trademark guidance: https://www.ableton.com/en/legal/branding-trademark-guidelines/

The applicable SDK terms are those supplied by Ableton for the SDK version used to build the respective release. Consult the `ABLETON-EXTENSIONS-SDK-LICENSE.md` or the corresponding third-party notice in each source package.

## 5. HGT artwork

The HGT logos and visual elements used in the extensions are original artwork created by HGT. Their geometric visual language is inspired by Piet Mondrian. They are not copies, reproductions or redistributed artworks by Mondrian.

## 6. HGT project licenses

Each extension has its own project-specific HGT license file. These licenses cover only original project material that HGT owns or controls. They do not relicense Phazite sound assets, Ableton SDK components, third-party software or trademarks.

The exact license title and terms are stated in each release package:
- Drum Construction Kit: `HGT License 1.0`
- Genre Remap: `HGT License 1.0`
- Genre Converter: `HGT Free Music Creator License 1.0`

These are project-specific licenses, not a single blanket license for all third-party material and not necessarily OSI-approved open-source licenses. Read the license shipped with the relevant extension.

## 7. Development tools

The supplied source packages document the use of Node.js and project build/test tooling, including TypeScript and esbuild where applicable. These are development dependencies and are not presented as bundled audio assets. Their respective upstream licenses apply.

## 8. Distribution and changes

The current release packages document:
- 37 embedded Phazite-derived MP3 payloads under the declared CC0 1.0 dedication;
- per-payload integrity hashes in `SOUND-ASSET-MANIFEST.json`;
- separate HGT project licenses and Ableton SDK notices;
- no Toontrack/EZdrummer audio content.

For exact file-level provenance, hashes, build boundaries and release-specific notices, consult the documents included in each source ZIP.

---
**HGT — Source and attribution record**
