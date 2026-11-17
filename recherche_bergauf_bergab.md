# Bergauf und bergab: Recherche für den Laufzeit-Rechner

Stand: 17.11.2026. Kennzeichnung: **[Sicher]** = im Original gelesen, **[Wahrscheinlich]** = Abstract oder Sekundärquelle, **[Vermutung]** = eigene Rechnung oder Synthese.

## Kurzfazit

1. **Energie:** Die Laufkosten am Hang sind gut vermessen. Minetti et al. 2002 ist im Bereich −10 % bis +10 % durch drei neuere Laborstudien bestätigt. Bergab spart man eher etwas weniger, als Minetti angibt. [Sicher]
2. **Tatsächliches Tempo:** Läufer nutzen Gefälle viel weniger aus, als die Energie erlauben würde. Das höchste Tempo liegt im Gelände bei etwa −8 %, die geringsten Kosten erst bei −14 bis −20 %. [Sicher/Wahrscheinlich]
3. **Rundkurs:** Die Faustregel der App („2 % langsamer je 100 Hm auf 10 km“) ist als Mittelwert für Straßenkurse mit 4–6 % Steigung gedeckt. Vertretbar ist ein Band von 1–3 %, je nach Steilheit. [Vermutung, aus mehreren Quellen abgeleitet]
4. **Watt:** Stryd-„Watt“ am Hang sind keine gemessene Mechanik, sondern ein an den Sauerstoffverbrauch geeichtes Modell. Polar und Golden Cheetah bauen Minetti sogar direkt ein. Für die App bringen Watt gegenüber einer direkt gewählten Kostenkurve keine zusätzliche Information. [Sicher/Wahrscheinlich]

---

## 1. Energiekosten im Labor

Minetti et al. 2002 (n = 10, Laufband, −45 % bis +45 %), Kosten je Meter in J/kg mit i als Dezimalbruch:
`C(i) = 155,4·i⁵ − 30,4·i⁴ − 43,3·i³ + 46,3·i² + 19,5·i + 3,6`. Das Minimum liegt bei −18 bis −20 %. [Sicher]
Hinweis: Das Polynom liefert in der Ebene 3,6, gemessen wurden 3,40. Verhältnisse deshalb immer mit 3,6 als Bezug bilden.

**Kosten gegenüber flach (Faktor)**

| Steigung | Minetti 2002 | Lemire 2021 (12 km/h, n = 29) | Lemire 2023 (10 km/h, n = 19) | Whiting 2022 (13 km/h, n = 16) | Breiner 2019 (n = 19) |
|---|---|---|---|---|---|
| −20 % | 0,50 | 0,59 | – | – | – |
| −10 % | 0,60 | 0,66 | 0,66 | – | – |
| −5 % | 0,76 | 0,80 | – | 0,76 (−5,24 %) | 0,82 |
| −2 % | 0,90 | 0,91 | – | – | – |
| +2 % | 1,11 | 1,10 | – | – | – |
| +5 % | 1,30 | 1,27 | – | 1,38 (+5,24 %) | – |
| +7,5 % | 1,47 | 1,44 | – | – | 1,46 |
| +10 % | 1,66 | 1,62 | 1,60 | – | – |

Lemire 2021 (Formel und optimales Gefälle −17,3 ± 2,3 %) habe ich im Original nachgeprüft [Sicher]. Breiner 2019 stammt aus dem Abstract [Wahrscheinlich].

## 2. Tatsächliches Tempo im Gelände

| Quelle | Daten | Ergebnis |
|---|---|---|
| Townshend et al. 2010 | Geländelauf, n = 8 | bergauf 23 % langsamer, bergab nur 13,8 % schneller; bergab sank die Sauerstoffaufnahme auf 79 % der Schwelle [Wahrscheinlich] |
| Staab et al. 1992 | Laufband-Rennen über 30 min, n = 11, Abschnitte mit ±5 % | Hügelkurs 2,4–2,8 % langsamer als flach [Wahrscheinlich] |
| Jidovtseff & De Cock 2026 | 517 Läufer, 20 Trailrennen, GPS | Höchsttempo bei etwa −8 %; ab etwa −15 % langsamer als flach; bei 3 m/s: +5 % → −14 %, −5 % → +9 % Tempo [Sicher] |
| Strava GAP | Herzfrequenzdaten sehr vieler Läufe | größter Bergab-Bonus bei etwa −10 %, bei etwa −18 % wieder wie flach [Sicher für die Hilfeseite, Wahrscheinlich für das Patent] |
| Daniels-Faustregel | Boston-Zwischenzeiten | bergauf 12–15 s/Meile je 1 %, bergab etwa 8 s/Meile je 1 % [Wahrscheinlich bzw. Vermutung für bergab] |

**Ab welchem Gefälle gebremst wird:** Das höchste Tempo liegt bei −8 bis −10 %, die geringsten Kosten bei −14 bis −20 %. Läufer bremsen also lange bevor es energetisch nötig wäre (Technik, Stoßbelastung, Muskelschutz). [Wahrscheinlich]

**Ermüdung bergab:** Nach längerem Bergablaufen ist die Laufökonomie in der Ebene 3–18 % schlechter, die Oberschenkelkraft 14–55 % niedriger (Bontemps 2020, Review mit typisch −12 % über 40 min) [Sicher]. Eine belegte Formel für den Zusatzverlust am Ende langer Rennen gibt es nicht.

## 3. Zeitverlust auf dem Rundkurs (100 Hm rauf und runter auf 10 km)

**Herleitung [Vermutung, eigene Rechnung]:** Bei konstanter Stoffwechselleistung hebt sich der lineare Term auf. Übrig bleibt
`Δt/t₀ ≈ 2·b·ḡ·H/D` mit dem quadratischen Kostenterm b (Minetti: 46,3/3,6 = 12,9) und der mittleren Steigung ḡ.
Der Verlust hängt also nicht nur von den Höhenmetern ab, sondern auch davon, wie steil sie sind.

| Modell | 2 % | 5 % | 8 % | 10 % |
|---|---|---|---|---|
| Minetti (Energie) | 0,5 % | 1,3 % | 2,1 % | 2,6 % |
| Lemire 2021 (Energie, 12 km/h) | 0,6 % | 1,4 % | 2,3 % | 2,8 % |
| Gelände-Tempo (Jidovtseff, 3 m/s) | 0,7 % | 1,7 % | 2,7 % | 3,5 % |
| Daniels | 1,1–1,9 % | gleich | gleich | gleich |
| Staab (±5 %, Laufband-Rennen) | – | etwa 3 % | – | – |

Mit derselben Zahl in der Schreibweise der App (Δt/t₀ = k·H/D in Prozent je 100 Hm auf 10 km):
- reine Energie bei 2–5 % Steigung: k ≈ 0,5–1,4
- Daniels: k ≈ 1,1–1,9
- Whiting bei 5,2 %: k ≈ 2,7–2,9
- Townshend: k ≈ 2,2–3,6
- Staab: k ≈ 3
- steiles Berg- oder Traillaufen (Scarf, ITRA): k ≈ 4–10

## 4. Watt bergauf und bergab (Stryd, Garmin, Coros, Polar)

- **Stryd:**
  - Steigung im Freien kommt aus dem Barometer, auf dem Laufband muss sie von Hand eingegeben werden [Sicher].
  - Die Hangleistung ist laut Stryd an Sauerstoffmessungen auf dem geneigten Laufband „rückwärts geeicht“, damit die angezeigten Watt in festem Verhältnis zum Energieumsatz stehen. Die Formel ist nicht veröffentlicht [Wahrscheinlich, über Outside 2018 und 2020].
- **Validierung gegen Sauerstoffaufnahme (Laufband, Steigung von Hand eingegeben):**
  - Gravina-Cognetti 2025, n = 15, −7 % bis +7 % [Sicher]:
    - Stryd-Leistung relativ zu flach: 0,73 (−7 %), 0,79 (−5 %), 1,26 (+5 %), 1,38 (+7 %).
    - Sauerstoffaufnahme relativ zu flach: 0,78, 0,83, 1,27, 1,36.
    - Bergab senkt Stryd die Watt also etwas stärker, als die Kosten sinken: bei −7 % etwa 4–7 % zu niedrig (eigene Rechnung).
  - van Rassel 2026 (0–8 %): Stryd unterschätzt bei steileren Steigungen um etwa 2–4 % [Wahrscheinlich].
  - Adejuwon 2026 (0/5/10 %): kein Unterschied im Verhältnis Sauerstoff zu Watt [Wahrscheinlich].
- **Steiler als −7 %** gibt es keine unabhängige Prüfung, für keinen Hersteller. Stryd rät selbst, ab −5 % die Leistung zu senken und auf steilen, technischen Abstiegen ganz zu ignorieren [Sicher].
- **Marken nicht vergleichbar:** Garmin liegt 25–30 % bzw. 100–150 W über Stryd. Auf einem Trail mit 195 Hm stimmten Garmin und Stryd bergauf schlecht überein (ICC 0,44) [Sicher].
- **Polar und GOVSS** (Golden Cheetah, Runalyze ohne Sensor) verwenden Minettis Kurve direkt [Sicher].
- **Modell van Dijk und van Megen** („The Secret of Running“): gedruckte Formel und eigene Tabelle widersprechen sich (quadratisch gegen linear) [Sicher]. Ihre Hangtests vergleichen Stryd mit dem eigenen Modell, nicht mit Sauerstoffmessung.

**Folgerung [Vermutung]:** Konstante Watt plus Hangmodell ist mathematisch dasselbe wie eine Kostenkurve C(i). Für die App reicht deshalb eine Kostenkurve. Watt würden nur nützen, wenn Nutzer eigene Stryd-Daten einspielen.

## 5. Empfehlung für die App [Vermutung]

1. **Ohne Angabe der Steilheit:** 2 % je 100 Hm auf 10 km beibehalten. Das ist gedeckt.
2. **Mit wählbarer Steilheit** (z. B. „wellig ≈ 2 %“, „hügelig ≈ 5 %“, „steil ≈ 10 %“): k steigungsabhängig wählen, etwa `k ≈ 1 + 20·ḡ` (2 % → 1,4; 5 % → 2,0; 10 % → 3,0). Diese Zwischenformel ist nicht validiert. Sie liegt aber zwischen reiner Energetik und den Feldmessungen.
3. **Mit Höhenprofil (Abschnitte):**
   - Bergauf: Zeitfaktor = C(i)/C(0) nach Lemire oder Minetti.
   - Bergab: nur einen Teil der Ersparnis gutschreiben und das Tempo begrenzen. Höchster Vorteil bei etwa −8 bis −10 %, ab etwa −15 % kein Vorteil mehr.
4. **Strecken mit Netto-Gefälle** (Punkt zu Punkt) gesondert behandeln: etwa 1–2 m Flachstrecke Gutschrift je Meter Netto-Gefälle (Daniels, Boston-Regel).

## 6. Lücken und Widersprüche

- **Keine direkte Studie:** Keine peer-reviewte Studie misst direkt „Zeitverlust je 100 Hm auf einem Rundkurs“. Staab 1992 kommt dem am nächsten.
- **Kleine Stichproben:** Laborstudien haben n = 8–29, meist trainierte Männer, auf dem Laufband mit Belastungen von 4–5 Minuten.
- **Felddaten:** Sie sind beobachtend und durch Technik und GPS-Höhenrauschen verzerrt.
- **Energieminimum:** Die Angaben schwanken zwischen −10 % (Margaria, Dewolf) und −17 bis −20 % (Minetti 2002, Lemire).
- **Nicht zugänglich:** Die Volltexte von Townshend, Kay, Scarf, Staab und der Strava-Technikblog 2017 waren gesperrt. Die Umrechnungen aus diesen Quellen sind Schätzungen.

## Quellen

**Energiekosten im Labor**
- Minetti et al. 2002: https://iris.unibs.it/retrieve/ddc633e4-3c03-4e2e-e053-3705fe0a4c80/Minetti%20JAP%202002.pdf
- Lemire et al. 2021: https://www.frontiersin.org/journals/physiology/articles/10.3389/fphys.2021.697315/full
- Lemire et al. 2023: https://www.nature.com/articles/s41598-023-38328-x
- Whiting, Hoogkamer & Kram 2022: https://pmc.ncbi.nlm.nih.gov/articles/PMC9189710/
- Breiner, Ortiz & Kram 2019: https://pubmed.ncbi.nlm.nih.gov/30357515/
- Hoogkamer, Taboga & Kram 2014: https://doi.org/10.7717/peerj.482
- Vernillo et al. 2017 (Review): https://pubmed.ncbi.nlm.nih.gov/27501719/
- Dewolf & Willems 2019: https://pubmed.ncbi.nlm.nih.gov/30611540/

**Tempo im Gelände und im Wettkampf**
- Townshend et al. 2010: https://pubmed.ncbi.nlm.nih.gov/20010117/
- Staab et al. 1992: https://pubmed.ncbi.nlm.nih.gov/1548986/
- Jidovtseff & De Cock 2026: https://doi.org/10.1080/24748668.2026.2651537
- Kay 2012: https://doi.org/10.1515/1559-0410.1456
- Scarf 2007: https://pubmed.ncbi.nlm.nih.gov/17454539/
- Strava GAP (Hilfeseite): https://support.strava.com/hc/en-us/articles/216917067-Grade-Adjusted-Pace-GAP
- Strava (Patent): https://patents.google.com/patent/US11623121B1/en
- Boston Marathon, Qualifikationsregeln: https://www.baa.org/races/boston-marathon/qualify
- World Athletics, Ranglistenregeln Straße: https://worldathletics.org/world-ranking-rules/road-running-2025

**Ermüdung bergab**
- Bontemps et al. 2020 (Review): https://pmc.ncbi.nlm.nih.gov/articles/PMC7674385/

**Watt am Hang: Validierungsstudien**
- Gravina-Cognetti et al. 2025: https://pmc.ncbi.nlm.nih.gov/articles/PMC12473670/
- van Rassel et al. 2026: https://doi.org/10.1123/ijspp.2025-0382
- Adejuwon et al. 2026: https://doi.org/10.1123/ijspp.2025-0579
- Berzosa et al. 2024: https://pmc.ncbi.nlm.nih.gov/articles/PMC11175203/

**Watt am Hang: Herstellerangaben und Berichte**
- Stryd-Hilfe, Trails und Hügel: https://help.stryd.com/en/articles/6879476-can-i-use-stryd-for-trails-and-hills
- Stryd-Hilfe, Laufband: https://help.stryd.com/en/articles/7971005-using-stryd-on-the-treadmill
- Stryd-Blog, Downhill-Modell 2017: https://blog.stryd.com/2017/05/24/power-up-and-attack-the-downhill-2/
- Outside 2018, „What Is Running Power, Anyway?“: https://www.outsideonline.com/health/what-running-power-anyway/?scope=anon
- Outside 2020, Stryd-Forschung: https://www.outsideonline.com/health/training-performance/running-power-stryd-research-2020?scope=anon
- Polar-Whitepaper: https://www.polar.com/img/static/whitepapers/pdf/polar-running-power-white-paper.pdf
- Golden Cheetah, GOVSS-Quellcode: https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/src/Metrics/GOVSS.cpp
- van Dijk & van Megen, Kosten am Hang: https://hetgeheimvanhardlopen.nl/wp-content/uploads/2017/02/17.-The-Energy-Cost-of-Running-on-hills.pdf
- the5krunner, Garmin Running Power: https://the5krunner.com/2026/10/25/garmin-running-power-guide/
