# Dungeon Test

Pixel-Art-Dungeon-Crawler (Top-Down, Echtzeit-Kampf) als spielbarer Prototyp.
Alles steckt in **einer Datei**: `index.html` im Browser öffnen und losspielen – auch auf dem iPad.

## Steuerung
| Aktion | Tastatur & Maus | Touch (iPad/Handy) |
|---|---|---|
| Laufen | WASD / Pfeiltasten | Joystick links (Daumen aufsetzen) |
| Angreifen | Linksklick (gedrückt halten) | ⚔-Knopf: antippen = automatisch zielen, ziehen = selbst zielen (Zielanzeige), loslassen = Angriff, halten = Dauerangriff |
| Ausweichen | Leertaste / Rechtsklick | 💨-Knopf |
| Interagieren / Wiederbeleben (halten) | E | ✋-Knopf |
| Zauber | 1–4 oder Hotbar anklicken | Zauber-Knöpfe im Bogen um den Angriffsknopf |
| Helden-Fähigkeit | Q | ✨-Knopf neben dem Angriffsknopf |
| Heiltrank | R | Trank-Knopf oben im Bogen |
| Pause | ESC | II oben rechts |

## Inhalte
- **Freischaltungen nach Konto-Level**: Start mit Ritter, Krypta, Ausrüstung, Händler, Schmied. Lv 2 Helden-Fähigkeit · Lv 3 Moosige Kerker, Zerlegen · Lv 5 Artefakte & antike Räume · Lv 6 Glutschlund, Tägliche Herausforderung · Lv 7 Verzaubern · Lv 8 Helden-Auswahl + Bogenschütze · Lv 9 Frostgewölbe · Lv 10 Assassine · Lv 12 Magier · Lv 14 Berserker. Schwierigkeit II ab Lv 6, III ab 10, IV ab 14, V ab 18 (zusätzlich zum Boss-Sieg). Langsamer Fortschritt: XP pro Level = 150 · Level^1,6
- **Ausrüstungsstufen 1–20** (zusätzlich zur Seltenheit): Schwierigkeit I gibt Stufe 1–4 (alle 2 Stages eine Stufe höher), II = 5–8, III = 9–12, IV = 13–16, V = 17–20. Gegnerstärke hängt an Schwierigkeit + Stage (Stage 10 auf I ist leichter als Stage 1 auf II). Pro zusätzlichem Spieler: Gegner +55 % Leben, +10 % Schaden (Bosse +70 % Leben).
- **Antike Räume**: einer pro Stage (meist am Ende eines Nebenwegs). Optional: Relikt berühren → 3 Elite-Wellen oder ein Mini-Boss (Grabritter, Brutmutter, Magmakoloss, Eisjägerin) → antike Truhe mit garantiertem Artefakt.
- **Dungeon-Auswahl**: 4 Dungeons (Krypta, Moosige Kerker, Glutschlund, Frostgewölbe) mit je 5 Stufen (I–V). Jeder Dungeon hat eigene Gegner, einen eigenen Boss (Knochenkönig, Moosgolem, Glutwyrm, Frostkönigin) und ein eigenes Artefakt-Set. Sieg über den Boss schaltet die nächste Stufe frei.
- **Artefakte** (wie in Genshin): 5 Plätze (Blüte, Feder, Sanduhr, Kelch, Krone), 2★–5★ je nach Stufe, Hauptwert + bis zu 4 Nebenwerte, Set-Boni für 2 und 4 Teile, aufwerten mit Essenz (2★ bis +8 … 5★ bis +20). 6 Sets: Knochenkrone, Wildwuchs, Glutherz, Frostschwur, Goldene Gier (Ultra-Schatzkammer), Sturmläufer (Tagesbelohnung)
- **Helden-Fähigkeiten**: Schildstoß, Pfeilhagel, Schattenschleier, Meteor, Raserei
- **Heiltränke**, **Schreine** (Segen oder Pakt für den ganzen Run), **Händler im Dungeon**, **Mimics**
- **Elite-Gegner** (Flink, Explosiv, Gepanzert, Vampir, Eisig) und neue Gegner: Skelettschütze, Höhlenspinne, Steinwächter, Irrlicht
- **Schmied**: Verbessern, Zerlegen (→ Essenz), Verzaubern (Passiv neu würfeln), Artefakte aufwerten
- **Tägliche Herausforderung**: fester Dungeon für alle, wechselnde Tagesregel, einmal täglich ein Sturmläufer-Artefakt
- **Lobby** mit animiertem Titel, Fackeln und deiner Party am Lagerfeuer
- **Freunde & Party**: bis zu 4 Spieler, Bereit-Status, Leader kann Mitglieder entfernen. Freunde sind simuliert (`MockSocialService`); ein echter Server kann über die Schnittstelle `SocialService` angebunden werden.
- **Ausrüstung**: Waffe, Helm, Brust, Hose, Schuhe, Schmuck, 4 Zauber-Slots, 30 Inventarplätze, Drag & Drop, Tooltips mit Vergleich
- **Helden**: Ritter von Anfang an (kleiner Bonus mit jeder Waffe). Ab Konto-Level 4 Bogenschütze (großer Bonus nur mit Bögen), ab 7 Assassine (Dolche), ab 10 Magier (Stäbe), ab 13 Berserker (Äxte/Hämmer). Jeder Held levelt einzeln bis Level 20.
- **Sets**: 8 Sets (Ritterorden, Schattenklinge, Waldläufer, Erzmagier, Blutrausch, Bergkönig, Glücksritter, Frostwacht) mit Boni für 2/4/6 Teile
- **Passive Boni**: Seltene Teile haben 1, epische 2, legendäre 3 zufällige Passive (Schaden, Angriffstempo, Crit, Lebensraub, Dornen, Gold …)
- **Waffen**: Dolch, Schwert, Axt, Kriegshammer, Bogen, Stab – jede mit eigenem Spielgefühl
- **Rüstungsklassen**: Stoff, Leder, Kette, Platte (Verteidigung gegen Tempo)
- **Seltenheiten**: Gewöhnlich, Selten, Episch, Legendär (Farbe, Glühen, Truhen-Lichtstrahl)
- **Zauber** (ca. 3 % pro Truhe): Feuerball, Heilung, Frostnova, Blitzkette, Schattenschritt
- **Stages**: Nach dem Boss erscheinen zwei Portale – grün = Dungeon verlassen und Beute sichern, lila = tiefer hinab in die nächste Stage (größer, stärkere Gegner, besserer Loot, neues Thema: Krypta, Moosige Kerker, Glutschlund, Frostgewölbe). Wer fällt, verliert die Hälfte des Golds.
- **Ultra-Schatzkammer** nach jeder 5. Stage: Goldberge, Statuen, 5 Truhen (meist episch/legendär) und mit 50 % eine Zauber-Schriftrolle
- **Raumgestaltung**: Kampfräume mit 6 Layouts (Säulen, Kistenlager, Mauerreste, Säulenhalle), Rätselräume mit Bücherregalen und Runenkreis, Fallenräume mit Blutflecken, Schatzkammern golden
- **Dungeon-Runs**: zufällige Räume – Kampf (Wellen), Rätsel (Hebel, Kisten auf Druckplatten, Feuerschalen, Runen), Fallen (Stacheln, Feuerstrahlen), Schatzkammern, Boss mit 3 Phasen
- Minimap, HP/Mana, Hotbar, Screenshake, Partikel, Schadenszahlen, Chiptune-Sounds
- **Händler** und **Schmied** (Verbessern bis +5) in der Lobby
- Spielstand wird im Browser gespeichert (localStorage)

## Code-Aufbau (Module in `index.html`)
1. Konfiguration & Hilfsfunktionen · 2. Audio · 3. Pixel-Sprites · 4. Daten (Items, Zauber, Gegner) · 5. Item-Erzeugung · 6. Profil/Speichern · 7. Soziales (Freunde/Party) · 8. Dungeon-Generator · 9. Run (Kampf, KI, Boss, Rätsel, Fallen, Loot) · 10. Darstellung (Licht, HUD, Minimap, Lobby) · 11. Oberfläche (Menüs) · 12. Eingabe & Spielschleife

Neue Gegner, Waffen, Zauber oder Rätsel = neuer Eintrag in den Daten-Objekten (`ENEMIES`, `WEAPONS`, `SPELLS`, `PUZZLES`).
