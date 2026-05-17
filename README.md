# 🔍 Sherlock – Logikrätsel

Ein browserbasiertes Logikrätsel, inspiriert vom klassischen DOS-Spiel **Sherlock – The Game of Logic** (Everett Kaser Software, 1991).

## Spielprinzip

Auf einem N×N-Raster (4×4, 5×5 oder 6×6) muss jedes Symbol genau einer Spalte zugeordnet werden. Hinweise beschreiben die Lagebeziehungen zwischen Symbolen und ermöglichen es, die korrekte Lösung durch logisches Schlussfolgern zu ermitteln.

## Steuerung

| Aktion | Beschreibung |
|---|---|
| **Linksklick** auf ein Symbol | Symbol ausschließen / Ausschluss rückgängig machen |
| **Rechtsklick** auf ein Symbol | Symbol als korrekt markieren / Markierung aufheben |
| **Klick auf bestätigte Zelle** | Zelle zurücksetzen |
| **Klick auf Hinweiskarte** | Hinweis als „verwendet" abhaken |
| **Drag & Drop** auf Hinweiskarte | Hinweise umsortieren |

## Buttons

| Button | Funktion |
|---|---|
| 🔄 Neues Spiel | Generiert ein neues, eindeutig lösbares Rätsel |
| ↺ Zurücksetzen | Setzt alle Markierungen zurück |
| 💡 Tipp | Schließt ein falsches Symbol automatisch aus und erklärt warum |
| ✓ Prüfen | Überprüft die bisherigen Markierungen auf Fehler |
| 👁 Lösung | Zeigt die vollständige Lösung an |

## Hinweistypen

| Symbol | Bedeutung |
|---|---|
| ↕ (gestapelt) | Beide Symbole stehen in derselben Spalte |
| ≠↕ | Beide Symbole stehen **nicht** in derselben Spalte |
| ↔ | Beide Symbole stehen direkt nebeneinander |
| ↮ | Beide Symbole stehen **nicht** direkt nebeneinander |
| … | Linkes Symbol befindet sich irgendwo links vom rechten |
| ‹ A › | A liegt direkt zwischen den beiden äußeren Symbolen |
| ·\|· | Genau eine Spalte Abstand zwischen beiden Symbolen |

## Schwierigkeitsgrade

| Modus | Raster | Beschreibung |
|---|---|---|
| Leicht | 4×4 | 4 Kategorien, wenige Hinweise |
| Mittel | 5×5 | 5 Kategorien, mittlere Komplexität |
| Schwer | 6×6 | 6 Kategorien, maximale Herausforderung |

## Kategorien

Das Spiel verwendet 6 Symbol-Kategorien: **Zahlen**, **Buchstaben**, **Tiere**, **Früchte**, **Formen** und **Wetter**.

## Technisches

- Reine Client-Side-Anwendung: eine einzige HTML-Datei, keine Abhängigkeiten
- Puzzle-Generator mit Constraint-Solver stellt eindeutige Lösbarkeit sicher
- Vollständig responsives Layout

## Starten

Einfach `sherlock.html` im Browser öffnen – kein Server oder Installation nötig.
