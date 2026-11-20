# Glückspalast (Testversion v0.2)

Idle-Glücksspiel zum Selberspielen, nur mit Spielgeld. Man würfelt, dreht, rubbelt und pokert selbst und baut daraus ein riesiges Glücksspiel-Konstrukt.
Alle Maschinen stehen gleichzeitig auf einem Feld und sind über Röhren verbunden: Gewinne rollen von Maschine zu Maschine und lösen Kettenreaktionen aus.
Alles steckt in **einer Datei**: `index.html` im Browser öffnen, funktioniert auch auf iPad und Handy.

## Die 8 Maschinen
| Maschine | Freischalten | Röhre zur nächsten Maschine |
|---|---|---|
| 🎲 Würfeltisch | Start | Zwei Paare und mehr → Münzen (Freispiele) in den Automaten, Straße → Bonus-Los |
| 🎰 Spielautomat | 2.500 | 3+ gleiche → Kugeln ins Plinko |
| 🎟️ Rubbellos-Drucker | 600 Tsd. | Gewinn → Kugel ins Plinko, 💎 → 3 Kugeln |
| ⚪ Plinko | 500 Mio. | Randfächer → Dreh am Glücksrad |
| 🎡 Glücksrad | 100 Mrd., ab Meilenstein 1 | 🔴-Feld → Chips ins Roulette, 🪙 Freispiele, 💰 Jackpot |
| 🔴 Roulette | 200 Bio., ab Meilenstein 3 | Volltreffer auf Lieblingszahl → Karte zum Pokertisch |
| 🃏 Kartentisch (Poker) | 500 Brd., ab Meilenstein 5 | ab Drilling → Gold in den Tresor |
| 🏦 Jackpot-Tresor | 10 Trd., ab Meilenstein 8 | wird von Ketten und Poker gefüllt und springt dann auf |

- Jede Maschine hat 2–9 Upgrades und einen Helfer-Roboter.
- **Material-Stufen:** Alle 8 Upgrades wechselt das Gehäuse sein Material: Holz → Chrom → Gold → Neon → Kristall → Regenbogen.
- **Spezialwürfel** (ab Meilenstein 2 im Stern-Shop): Glas (×20, zerbricht manchmal), Joker (passt sich der besten Kombi an), Splitter (teilt sich bei einer 6), Feuer (×3 in Kombis).

## Fortschritt
- **Glücksstaub und Talentbaum:** 24 Talente in 4 Ästen (Würfel, Automaten, Glück, Röhren). Staub gibt es nur für seltene Treffer.
- **♻️ Bankrott (Ebene 1):** Ab 50 Mrd. in einer Runde gibt man alles ab und bekommt Glückssterne. Jede Zehnerpotenz mehr bringt deutlich mehr Sterne.
  - Die Sterne gibt man im **Stern-Shop** aus: 14 Upgrades, zum Beispiel Startvorteile, Spezialwürfel, Münzspeicher und VIP-Gäste.
  - Alle je verdienten Sterne geben zusätzlich einen dauerhaften Bonus.
- **🏁 Meilensteine nach verdienten Sternen:**

  | Sterne | schaltet frei |
  |---|---|
  | 1 | Stern-Shop und Glücksrad |
  | 5 | Spezialwürfel, Röhren-Talente, Highroller |
  | 15 | Roulette |
  | 40 | Herausforderungen |
  | 100 | Kartentisch |
  | 400 | Freispiel-Sturm |
  | 1.000 | Jackpot-Tresor |
  | 6.000 | Casino-Umzug |

- **🎯 Herausforderungen:** 6 Runden mit Einschränkung (z. B. „Nur ein Würfel“, „Ohne Plinko“). Wer sie schafft, bekommt eine dauerhafte Belohnung.
- **🏆 Erfolge:** 35 Stück, jeder gibt +2 % auf alles.
- **🏛️ Casino-Umzug (Ebene 2):** Man gibt Sterne, Stern-Shop und Meilensteine ab und bekommt Casino-Lizenzen.
  - Lizenz-Shop: Imperium (×3 auf alles), Bankrott-Automat, Erinnerung und mehr.
  - Jedes Casino sieht anders aus und hat eine Sonderregel: Hinterhof → Riviera → Las Vegas → Macau → Unterwasser-Kuppel → Mondbasis → Neon-Galaxie → endlos „Sektor N“.
- **Ereignisse:**
  - Goldene Chips: Heiße Hand ×7, Goldregen, Sternschnuppe oder Freispiel-Sturm.
  - Glücksphasen (×3).
  - Highroller, die eine Wette anbieten.
  - Große Gewinne mit BIG / MEGA / EPIC WIN.
- **Offline-Gewinn:** bis 12 Stunden (mit Stern-Shop bis 36 Stunden).

Laut Simulation mit einem Computer-Spieler, der ununterbrochen spielt:
- erster Bankrott nach knapp 1 Stunde
- Meilenstein 10 (Casino-Umzug) nach etwa 3 Stunden

Echte Spieler brauchen ungefähr doppelt so lang. Danach geht es mit den Casinos endlos weiter.

## Steuerung
- Maschine antippen: würfeln, drehen, Kugel werfen, Karten geben. ⚙️ an jeder Maschine öffnet ihre Upgrades.
- Lose mit dem Finger oder der Maus freirubbeln.
- Ziehen verschiebt das Feld, zwei Finger oder das Mausrad zoomen, ⤢ zeigt die Übersicht.
- Leertaste würfelt.
- Untere Leiste: Maschinen, Talente, Sterne, Bankrott, Ziele, Casino.

Der Spielstand liegt im Browser (localStorage). Der frühere Dungeon-Prototyp steckt in der Git-Geschichte dieses Repos, die aktuelle Dungeon-Version läuft im Game Hub (`dungeon.html`).
