# HGT MIDI CC Mapping v1.0

**Architecture:** Global  
**MIDI channel:** 10 (fixed)  
**CC range:** 20–29  
**Value range:** 0–127

All assignments in this document are HGT-specific global extension controls. They are not GM percussion instrument selectors. Instrument selection is always by MIDI note number.

| CC | Stable ID | Parameter | Data type | Scope |
|---:|---|---|---|---|
| 20 | `performance_feel` | Performance Feel | Continuous | Global |
| 21 | `swing` | Swing | Continuous | Global |
| 22 | `fill_intensity` | Fill Intensity | Continuous | Global |
| 23 | `groove_variation` | Groove Variation | Continuous | Global |
| 24 | `verse_variation` | Verse Variation | Continuous | Global |
| 25 | `song_dramaturgy` | Song Dramaturgy | Continuous | Global |
| 26 | `repetition_pass` | Repetition / Pass: 0 = First Pass, 1 = Second Pass, 2 = Final Pass, 3 = Repeat/Loop; 4–127 reserved | Discrete | Global |
| 27 | `drummer_style_influence` | Drummer Style Influence | Continuous | Global |
| 28 | `preview_volume` | Preview Volume | Continuous | Global |
| 29 | `master_variation` | Master Variation | Continuous | Global |

## Rules

1. Send and receive these CCs on MIDI channel 10 only.
2. Preserve the assignment of each CC number across Genre Converter, Genre Remap, and Drum Construction Kit.
3. Do not create per-instrument interpretations of CC 20–29.
4. Continuous controls accept 0–127 and map to the receiving feature's documented native range.
5. CC 26 is a fixed discrete selector: 0 = First Pass, 1 = Second Pass, 2 = Final Pass, 3 = Repeat/Loop. Values 4–127 are reserved and must be ignored.
6. CC 28 controls preview monitoring only and must not alter generated MIDI note velocity.
7. If an extension does not implement a parameter, it may ignore that CC; it must not reuse the CC for another meaning.
8. CC 20–29 are a reserved HGT project convention for these extensions. They are not part of the GM percussion note map.
