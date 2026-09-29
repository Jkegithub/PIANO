# Anleitung: Klangprobe mit MIDI-Keyboard

*Angelegt 29.09.2026. Stand damals: **kein MIDI-Keyboard vorhanden.** Diese Anleitung gilt,
sobald eines da ist.*

## Voraussetzungen

- MIDI-Keyboard oder Digitalpiano mit **USB-MIDI** (oder ein USB-MIDI-Interface)
- Browser: **Brave, Chrome, Edge oder Firefox**. Safari und iPhone/iPad haben kein Web MIDI
- Internet: Die Samples kommen beim Laden vom jsDelivr-CDN (anfangs ca. 27 MB)

## Ablauf

1. Keyboard per USB anschließen und einschalten, **bevor** der Browser die Seite öffnet.
2. Lokalen Server starten, im Ordner `300_PIANO`:
   ```
   python -m http.server 8765 --bind 127.0.0.1 --directory probe
   ```
   (oder in Claude Code: Vorschau „piano-probe“)
3. In Brave `http://localhost:8765` öffnen und auf **„Klang laden“** klicken.
4. Die Abfrage nach **MIDI-Zugriff erlauben**.
5. Im Tastenprotokoll rechts muss unter **„MIDI-Eingänge:“** das Keyboard stehen.
   Steht dort „keiner gefunden“: Keyboard aus- und wieder einschalten und die Seite neu laden.

## Was die Pianistin prüft

| Punkt | Frage |
|---|---|
| Übergänge | Gibt es hörbare Sprünge beim Crescendo über die ganze Dynamik? |
| Pianissimo | Leise genug? Klingt es noch nach Klavier? |
| Fortissimo | Genug Kraft, nicht blechern? |
| Pedal | Klingt das Nachklingen natürlich? |
| Loslassen | Dämpfer und Hammergeräusch passend? |
| Latenz | Spürbare Verzögerung zwischen Anschlag und Ton? |

**Dynamik vergleichen:** Oben lässt sich zwischen **„Neu“** und **„Alt (Probe 1)“** umschalten.
Welches Profil besser ist, entscheidet ihr Ohr.

Das Tastenprotokoll zeigt bei jedem Ton die Anschlagstärke (vel), die Sample-Stufe und die
Ziel-Lautheit. Auffällige Töne dort ablesen und notieren.
