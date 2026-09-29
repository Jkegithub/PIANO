# 300_PIANO

Ein Klavier im Browser zum Lernen und zum Spielen, für Anfänger wie für Fortgeschrittene.
Die Klangfarbe soll natürlich sein, nicht synthetisch.

**Stand:** Klangprobe (29.09.2026). Spielbar über Computertastatur, Maus, Touch oder MIDI-Keyboard.
Der Lernmodus folgt.

**Online:** https://jkegithub.github.io/PIANO/

## Bedienung

- **Klang laden** klicken; die Samples kommen vom jsDelivr-CDN (ca. 27 MB)
- Computertastatur: `A`–`Ä` weiße Tasten, `W E T Z U O P` schwarze, `C`/`X` Oktave, Leertaste = Pedal
- Handy/Tablet: Der Touch-Modus schaltet sich automatisch ein. Große Tasten, oben leise und unten laut, mehrere Finger, ◀ ▶ zum Verschieben, Pedal-Knopf. iPhone: Stummschalter aus
- MIDI-Keyboard: in Chrome, Edge, Firefox und Brave; nicht in Safari und auf iPhone/iPad
- Anleitung für den Test mit Keyboard: [probe/ANLEITUNG_Keyboardtest.md](probe/ANLEITUNG_Keyboardtest.md)

## Klangquelle

**Salamander Grand Piano V3** von Alexander Holm, lizenziert unter
[CC BY 3.0](https://creativecommons.org/licenses/by/3.0/). Aufgenommen ist ein Yamaha C5.
Verwendet wird die MP3-Fassung der npm-Pakete `@audio-samples/piano-mp3-*` (darosh).
Die Samples werden nicht in diesem Repo gespeichert, sondern zur Laufzeit geladen.
