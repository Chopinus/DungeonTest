# Glückspalast (Testversion v0.1)

Idle-Glücksspiel zum Selberspielen, nur mit Spielgeld. Man würfelt, dreht und rubbelt selbst und baut daraus ein riesiges Glücksspiel-Konstrukt. Alle Maschinen stehen gleichzeitig auf einem Feld und sind über Röhren verbunden.
Alles steckt in **einer Datei**: `index.html` im Browser öffnen, funktioniert auch auf iPad und Handy.

## Maschinen
| Maschine | Freischalten | Was sie macht | Röhre |
|---|---|---|---|
| 🎲 Würfeltisch | Start | Würfeln, Kombis wie beim Kniffel (Pasch … Kniffel), Goldwürfel ×5 | Zwei Paare, Drilling … → Münzen (Freispiele, max. 10) in den Automaten, Straße → Bonus-Los |
| 🎰 Spielautomat | 2.500 | 3–5 Walzen, 🃏 Joker, 7️⃣7️⃣7️⃣ = Glücksstaub | 3+ gleiche → Kugeln ins Plinko |
| 🎟️ Rubbellos-Drucker | 600 Tsd. | druckt Lose, die man mit dem Finger freirubbelt | Gewinn → Kugel ins Plinko, 💎 → 3 Kugeln |
| ⚪ Plinko | 500 Mio. | Kugeln fallen durch Stifte in Gewinnfächer | Randfächer zahlen am meisten und geben manchmal Glücksstaub |

- Jede Maschine hat eigene Upgrades und einen Helfer-Roboter, der sie automatisch spielt.
- **Ketten:** Was über eine Röhre ankommt, zählt als Kettenglied. Jedes Glied gibt +5 % (mit Talent +10 %).
- **Goldener Chip:** Taucht ab und zu auf. Antippen gibt eine Heiße Hand (×7), einen Goldregen oder Glücksstaub.
- **Glücksstaub und Talentbaum:** 12 Talente in 3 Ästen. Sie bleiben auch nach dem Bankrott erhalten.
- **Bankrott (Prestige):** Ab 33 Mrd. in einer Runde (erster Stern, bei guter Spielweise nach etwa 40–90 Minuten) kann man alles abgeben und bekommt Glückssterne (+20 % auf alles pro Stern).
- **Offline-Gewinn:** bis 12 Stunden, 50 % (mit Talent 100 %).
- Der Spielstand liegt im Browser (localStorage).

## Steuerung
- Maschine antippen: würfeln, drehen oder eine Kugel werfen.
- Lose mit dem Finger oder der Maus freirubbeln.
- Ziehen verschiebt das Feld, zwei Finger oder das Mausrad zoomen, ⤢ zeigt die Übersicht.
- Leertaste würfelt.
- Untere Leiste: Upgrades pro Maschine, Talente und Bankrott.
- Im Hochformat stehen die Maschinen untereinander, im Querformat nebeneinander.

## Geplant
- **v0.2:** Röhren selbst verlegen (Weichen, Verdoppler), Glücksrad, Roulette, Glücksphasen, Herausforderungen.
- **v0.3:** Kartentisch, Jackpot-Tresor, Casinos mit Sonderregeln, Sammelbuch, Rangliste.

Der frühere Dungeon-Prototyp steckt in der Git-Geschichte dieses Repos. Die aktuelle Dungeon-Version läuft im Game Hub (`dungeon.html`).
