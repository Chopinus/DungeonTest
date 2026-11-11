# Dungeon Test

Pixel-Art-Dungeon-Crawler (Top-Down, Echtzeit-Kampf) als spielbarer Prototyp.
Alles steckt in **einer Datei**: `index.html` im Browser öffnen und losspielen – auch auf dem iPad.

## Steuerung
| Aktion | Tastatur & Maus | Touch (iPad/Handy) |
|---|---|---|
| Laufen | WASD / Pfeiltasten | Joystick links (Daumen aufsetzen) |
| Angreifen | Linksklick (gedrückt halten) | ⚔-Knopf (zielt automatisch) |
| Ausweichen | Leertaste / Rechtsklick | 💨-Knopf |
| Interagieren / Wiederbeleben (halten) | E | ✋-Knopf |
| Zauber | 1–4 oder Hotbar anklicken | Hotbar antippen |
| Pause | ESC | II oben rechts |

## Inhalte
- **Lobby** mit animiertem Titel, Fackeln und deiner Party am Lagerfeuer
- **Freunde & Party**: bis zu 4 Spieler, Bereit-Status, Leader kann Mitglieder entfernen. Freunde sind simuliert (`MockSocialService`); ein echter Server kann über die Schnittstelle `SocialService` angebunden werden.
- **Ausrüstung**: Waffe, Helm, Brust, Hose, Schuhe, Schmuck, 4 Zauber-Slots, 30 Inventarplätze, Drag & Drop, Tooltips mit Vergleich
- **Waffen**: Dolch, Schwert, Axt, Kriegshammer, Bogen, Stab – jede mit eigenem Spielgefühl
- **Rüstungsklassen**: Stoff, Leder, Kette, Platte (Verteidigung gegen Tempo)
- **Seltenheiten**: Gewöhnlich, Selten, Episch, Legendär (Farbe, Glühen, Truhen-Lichtstrahl)
- **Zauber** (ca. 3 % pro Truhe): Feuerball, Heilung, Frostnova, Blitzkette, Schattenschritt
- **Dungeon-Runs**: zufällige Räume – Kampf (Wellen), Rätsel (Hebel, Kisten auf Druckplatten, Feuerschalen, Runen), Fallen (Stacheln, Feuerstrahlen), Schatzkammern, Boss mit 3 Phasen
- Minimap, HP/Mana, Hotbar, Screenshake, Partikel, Schadenszahlen, Chiptune-Sounds
- **Händler** und **Schmied** (Verbessern bis +5) in der Lobby
- Spielstand wird im Browser gespeichert (localStorage)

## Code-Aufbau (Module in `index.html`)
1. Konfiguration & Hilfsfunktionen · 2. Audio · 3. Pixel-Sprites · 4. Daten (Items, Zauber, Gegner) · 5. Item-Erzeugung · 6. Profil/Speichern · 7. Soziales (Freunde/Party) · 8. Dungeon-Generator · 9. Run (Kampf, KI, Boss, Rätsel, Fallen, Loot) · 10. Darstellung (Licht, HUD, Minimap, Lobby) · 11. Oberfläche (Menüs) · 12. Eingabe & Spielschleife

Neue Gegner, Waffen, Zauber oder Rätsel = neuer Eintrag in den Daten-Objekten (`ENEMIES`, `WEAPONS`, `SPELLS`, `PUZZLES`).
