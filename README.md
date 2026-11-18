# Miventia Social Media

Bildablage für die Social-Media-Beiträge von **Miventia** (DJ-Service, Eventmanagement und Technikverleih aus Bochum).

Claude erstellt die Grafiken nach dem Miventia-Designsystem, legt sie hier ab und übergibt sie über den direkten Bild-Link als Entwurf an **Buffer** (Instagram, Facebook, LinkedIn). Veröffentlicht wird erst nach Freigabe durch Mika in Buffer.

> **Wichtig: Dieses Repository ist öffentlich.**
> Hier liegen ausschließlich Bilder, die ohnehin veröffentlicht werden sollen. Keine Kundendaten, keine Rechnungen, keine Zugangsdaten, keine unveröffentlichten privaten Fotos.

## Ablauf

1. Claude erstellt die Grafik(en) im Format 1080 × 1350 px (4:5).
2. Claude legt sie im passenden Ordner ab und pusht auf `main`.
3. Claude legt in Buffer pro Kanal einen Entwurf an und verlinkt das Bild über die Raw-Adresse.
4. Mika prüft die Entwürfe in Buffer und gibt frei, ändert oder löscht.

## Ordnerstruktur

```
posts/        Regelmäßige Wochenbeiträge
  2026/
    kw48/
      2026-11-24_tipp-buchungsvorlauf/
        01.png
        02.png        (weitere Slides bei Karussells)
anlaesse/     Feste Anlässe außerhalb des Wochenrhythmus (Weihnachten, Neujahr …)
  2026/
    2026-12-24_weihnachten/
      01.png
recaps/       Event-Recaps mit Fotos und Infos von Mika
  2026/
    2026-11-07_60-geburtstag-bermuda-lounge/
      01.png
tests/        Testläufe der Automatisierung
```

## Benennung

- Ordner pro Beitrag: `JJJJ-MM-TT_kurzes-thema` (Datum = geplanter Posting-Tag, Thema in Kleinbuchstaben mit Bindestrichen, ohne Umlaute).
- Bilder pro Beitrag: `01.png`, `02.png`, … in der Reihenfolge der Slides.
- Ein Bild wird für Instagram, Facebook und LinkedIn gemeinsam genutzt (4:5 funktioniert auf allen drei Plattformen).

## Bild-Adresse für Buffer

```
https://raw.githubusercontent.com/mim05/miventia-social-media/main/<pfad-zur-datei>
```

Beispiel:

```
https://raw.githubusercontent.com/mim05/miventia-social-media/main/tests/2026-11-18_pipeline-test/01.png
```

## Regeln

- Dateien nach dem Hochladen **nicht umbenennen, verschieben oder löschen**, solange der Beitrag in Buffer noch geplant ist. Sonst findet Buffer das Bild nicht mehr.
- Bereits veröffentlichte Beiträge bleiben als Archiv liegen.
- Keine KI-Motive als echte Events, Kunden oder Gäste ausgeben (siehe Designsystem).
