# Oscilloscope virtuel — Vierkanal-Oszilloskop zum Üben (1GIGF · ELETE)

Interaktives **virtuelles Oszilloskop mit vier Kanälen** (französisch) für den Elektrotechnik-Unterricht:
Die Lehrkraft gibt Spannungen und Ströme vor (Scheitelwert, Frequenz, Phasenlage, Kurvenform), die Schülerinnen und
Schüler bedienen das Gerät wie ein echtes Oszilloskop und bestimmen **Scheitelwert, Spitze-Spitze-Wert, Effektivwert,
Periode, Frequenz** und die **Phasenverschiebung** φ = Δt/T · 360° zwischen zwei Signalen. Antworten lassen sich prüfen,
die vollständige Lösung ist aufklappbar. Ergänzung zum Kurs *ELETE 1GIG* (Kapitel „Grandeurs alternatives“) und zum
Aufgabenblatt *Lecture d'oscillogrammes*.

🔗 **Live:** https://temmchen.github.io/oscilloscope-virtuel/

<img src="qr-code.png" alt="QR-Code zum Oszilloskop" width="180">

`qr-code.png` / `qr-code.svg` = derselbe QR-Code wie in der Seite (Taste **Q**), zum Ausdrucken oder für Folien.

## Was die Seite bietet

- **Oszilloskop OV-4**: Bildschirm 10 × 8 DIV mit Feinteilung, vier Kanäle mit Drehschaltern **VOLTS/DIV** (5 mV … 20 V,
  bei Stromkanälen mA/A) und gemeinsamer Zeitbasis **TIME/DIV** (1 µs … 0,5 s), Y-POS, X-POS, **INV**, Kopplung **AC/DC/GND**,
  Triggerquelle und -flanke, Cursor (Ablesung in DIV, auf Wunsch Δt und ΔU), Repères 0 V, Tastkopf 10:1.
  Die Einstellungen liest man am Knopf ab, wie am echten Gerät – nicht als Klartext auf dem Schirm.
- **Enseignant** (Taste **E**): je Kanal Spannung oder Strom, Name, Kurvenform (Sinus, Dreieck, Rechteck), Scheitelwert,
  Phase, Gleichanteil, Tastkopf; Frequenz; Kanalpaar für den Phasenwinkel. Zehn Szenarien (Widerstand, Kondensator, Spule,
  RC- und RL-Reihenschaltung mit vier Kanälen, Netz 230 V, zwei Tensions, Drehstrom, Kurvenformen, Mischgröße) und
  **„Exercice aléatoire“** mit Zufallswerten, die auf glatte Zehntel-DIV fallen. „Copier le lien élève“ erzeugt eine Adresse
  mit den eingestellten Signalen.
- **Mission** mit Formelkasten, **Vos réponses** mit Selbstkontrolle (grün/rot) und **Solution détaillée** (Taste **L**):
  Schalterstellungen, Ablesung in DIV, Rechenweg, Richtung der Phasenverschiebung (en avance / en retard), Zeitgleichungen,
  Hinweise bei übersteuertem Signal, ungeeigneter Zeitbasis und der INV-Falle; Einzeichnungen û, T, Δt auf dem Schirm.
- **Automatische Anpassung** an Mac/PC (alles auf einer Seite), iPad und iPhone (Reiter, fixierter Schirm, große Tasten);
  Hilfe mit Taste **?**. Alles läuft offline in einer einzigen HTML-Datei, ohne Abhängigkeiten, ohne Datenübertragung.

## Bedienung

| Taste | Wirkung |
| --- | --- |
| **E** | Lehrer-Panel ein/aus |
| **L** | Lösung auf-/zuklappen |
| **C** | Cursor ein/aus |
| **R** | Oszilloskop zurücksetzen |
| **Q** | QR-Code bildschirmfüllend (für den Beamer) |
| **F** · **?** · Esc | Vollbild · Hilfe · schließen |
| Drehschalter | ziehen, Mausrad, Pfeiltasten, Klick auf eine Stellung oder − / + |

Adressen: `#mode=eleve` startet ohne Lehrer-Panel, `#ui=phone|tablet|desktop` erzwingt ein Layout, `#taille=large` die große
Darstellung für den Beamer.

## Technik

Eine `index.html` (Vanilla JS, Canvas, SVG), keine Abhängigkeiten. Quellcode des Dashboards (Vorlage, CSS, JS-Teile, Bauskript,
Testsuite) liegt beim Autor; diese Seite ist die gebaute Fassung. Lizenz: MIT (© 2026 Tom Bleyer).

---

## Section française

**Oscilloscope virtuel à quatre voies** pour la classe 1GIGF (ELETE, LTEtt). L'enseignant règle les signaux (valeur de crête,
fréquence, phase, forme d'onde) ; les élèves manipulent l'appareil comme un vrai oscilloscope – calibres VOLTS/DIV et TIME/DIV,
Y-POS, X-POS, INV, couplage AC/DC/GND, déclenchement, curseurs – et déterminent la **valeur de crête**, la **valeur crête à crête**,
la **valeur efficace**, la **période**, la **fréquence** et le **déphasage** φ = Δt/T · 360° entre deux signaux
(φ > 0 : en avance, φ < 0 : en retard). Les réponses se vérifient dans le tableau ; la solution détaillée se déplie en bas
(touche **L**) avec les lectures en divisions, les calculs et les équations horaires.

- **E** : réglages de l'enseignant (signaux, scénarios, exercice aléatoire, lien élève) · **C** : curseurs · **R** : réinitialiser ·
  **Q** : QR-code · **?** : aide.
- La page s'adapte automatiquement à l'ordinateur, à l'iPad et à l'iPhone ; elle fonctionne hors ligne, aucune donnée ne quitte l'appareil.
