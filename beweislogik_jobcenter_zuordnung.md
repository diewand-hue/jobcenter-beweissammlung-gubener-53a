# Beweislogik und Zuordnung für die Jobcenter-Dokumentenmappe

**Zielrepository:** [`diewand-hue/jobcenter-beweissammlung-gubener-53a`](https://github.com/diewand-hue/jobcenter-beweissammlung-gubener-53a)
**Stand:** 20. September 2026
**Status:** Arbeits- und Prüfgrundlage; keine abschließende rechtliche oder sachverständige Bewertung

> Dieses Dokument bildet die Beweislogik der Dokumentenmappe. Es trennt Originalbefund, technische Auswertung, Rechenprüfung, Schlussfolgerung und offenen Prüfbedarf. Die Begriffe „Fehler“, „Verantwortung“, „Manipulation“ und „Haftung“ werden nur als Prüfthese verwendet, solange sie nicht durch Originalunterlagen oder ein Gutachten bestätigt sind.

---

## 1. Zweck der Sammlung

Die Mappe soll dem Jobcenter eine nachvollziehbare Prüfung ermöglichen:

1. Welche Kostenposition ist für welches Jahr und welche Ebene streitig?
2. Welche Originalunterlage belegt die Position?
3. Welche Zahlen stammen aus der Wohnungseinzelabrechnung und welche aus der Gebäudeabrechnung?
4. Welche technischen oder organisatorischen Umstände sind dokumentiert?
5. Welche Kosten wurden tatsächlich vorausgezahlt, berücksichtigt oder belastend angesetzt?
6. Welche Unterlagen fehlen noch?
7. Welche konkrete Prüfung, Korrektur oder Entscheidung wird beantragt?

Die Sammlung behauptet nicht mehr, als die jeweils angegebene Quelle trägt.

---

## 2. Verbindliche Quellenhierarchie

| Rang | Quelle | Verwendung |
|---|---|---|
| 1 | unverändertes Originaldokument bzw. Originalfoto/-video | Primärnachweis |
| 2 | Originalseite mit Seitenzahl, Dateiname und Archivlink | genaue Zitierung |
| 3 | Abrechnung, Mietkonto, Ablese- oder Geräteprotokoll | Zahlen- und Messprüfung |
| 4 | CSV-/Excel-Auswertung | Register, Rechenkontrolle und Vergleich; nicht Ersatz des Originals |
| 5 | Markdown-, HTML- oder Skriptauswertung | Darstellung und Reproduzierbarkeit |
| 6 | Schlussfolgerung oder rechtliche Würdigung | getrennte Bewertung |

Eine Auswertung darf einen Originalwert nicht stillschweigend ersetzen. Bei Abweichungen werden **Wert A**, **Wert B**, Rechenprüfung, Arbeitswert und Klärungsstatus nebeneinander ausgewiesen.

---

## 3. Indexierung nach den Tabellenvorgaben

Die CSV-/Excel-Struktur ist das führende Register für die Kosten- und Nachweisindexierung. Die vorhandenen Bezeichnungen werden beibehalten.

### 3.1 Primär- und Kostenbelege

- `BK-1` – Primärabrechnungsreihe/Betriebskostenunterlagen 2009–2024
- `BK-1-2009` bis `BK-1-2024` – Jahresbezug innerhalb der Primäranlage
- `BK-5` – Mietkonto/Vorauszahlungen 2022–2024
- `BK-ANTRAG-P1` – Vorlageanträge Priorität 1
- `BK-ANTRAG-P2` – Vorlageanträge Priorität 2

### 3.2 Mediennachweise

Für Fotos und Videos wird der Tabellen- bzw. Jahresbezug vorangestellt:

- `BK-1-2024-F-001` – Foto, Abrechnungsbezug 2024
- `BK-1-2024-V-001` – Video, Abrechnungsbezug 2024
- `BK-1-2023-F-001` – Foto, Abrechnungsbezug 2023
- `BK-1-2023-V-001` – Video, Abrechnungsbezug 2023

Falls ein Medium noch keinem Jahr sicher zugeordnet werden kann, wird vorläufig `MED-YYYY-NNN` oder `MED-UNGEKLÄRT-NNN` verwendet. Eine vorläufige Zuordnung wird nicht als Aufnahmedatum ausgegeben.

### 3.3 Beweisfragen

- `B-01` – dokumentierte Mängelanzeigen und Kenntnis
- `B-02` – Heizungsausfälle, Temperatur und Nutzbarkeit
- `B-03` – eigene Zusatzheizung und Zusatzkosten
- `B-04` – Thermostat-/Stellventilereignis 2023
- `B-05` – HKV-Werte und technische Plausibilität
- `B-06` – Warmwasserposition und Zählerbeobachtungen
- `B-07` – Gebäude- gegenüber Wohnungswerten
- `B-08` – auffällige Abrechnung 2022
- `B-09` – Umlageschlüssel und Ebenentrennung
- `B-10` – Jobcenter-Akte, Prüfung und Leistungsentscheidung

Diese IDs beschreiben die **Beweisfrage**, nicht automatisch deren Beweisbarkeit.

---

## 4. Beweislogisches Grundschema

Jeder Eintrag wird in dieser Reihenfolge erstellt:

1. **Tatsache/Feststellung:** Was steht im Original oder ist unmittelbar sichtbar?
2. **Quelle:** Exakter Dateiname, Repository-Pfad, Commit/Archivstand und gegebenenfalls Seite oder Zeitstempel.
3. **Technische bzw. rechnerische Prüfung:** Welche Rechnung oder Messauswertung wurde durchgeführt?
4. **Zuordnung:** Bezug zu `BK-1`, Jahreswert, `BK-5` oder einer `B-*`-Beweisfrage.
5. **Vorläufige Schlussfolgerung:** Was spricht der Nachweis aus, ohne eine unbelegte Ursache zu behaupten?
6. **Gegenprüfung:** Welche alternative Erklärung ist möglich?
7. **Offener Nachweis:** Welche Originalunterlage oder fachkundige Prüfung fehlt?
8. **Antrag an das Jobcenter:** Welche konkrete Auskunft, Korrektur oder Prüfung wird verlangt?

### Formulierungsregel

- „Die Datei zeigt …“ = unmittelbare Feststellung.
- „Die Tabelle weist aus …“ = dokumentierter Tabellenwert.
- „Dies ist auffällig, weil …“ = Plausibilitätsbeobachtung.
- „Es besteht der Prüfbedarf, ob …“ = offene Hypothese.
- „Es ist bewiesen, dass …“ nur bei tatsächlich gesicherter Beleglage.

---

## 5. Zahlen- und Plausibilitätsregister

Jeder Geld- oder Verbrauchswert erhält mindestens diese Felder:

| Feld | Pflichtangabe |
|---|---|
| Index | z. B. `BK-1-2024` |
| Jahr/Zeitraum | Abrechnungszeitraum |
| Ebene | Gebäude / Wohnung / Jobcenter |
| Kostenart | BK / Heizung / Warmwasser / Vorauszahlung |
| Originalwert | exakt wie Quelle, einschließlich Einheit |
| Rechenwert | nachvollziehbar berechneter Vergleichswert |
| Quelle | Datei, Seite, Tabelle oder Zeile |
| Status | bestätigt / abweichend / ungeklärt |
| Prüfauftrag | erforderliche nächste Unterlage |

Die in der Tabelle dokumentierten Arbeitswerte werden nicht ohne Originalabgleich als endgültige Tatsachen verwendet. Dies betrifft insbesondere:

- 2024: `51,94 €` gegenüber `643,42 €`;
- die Summe 2022–2024: `942,77 €` gegenüber `1.534,25 €`;
- 2023: Warmwasser `0,00 €` und eine Differenz von `1,94 €`;
- die abweichenden 2022- und 2020-Werte;
- die Aufteilung von Heizung und Warmwasser 2023/2024.

Arbeitsgrundlage der Rechenkontrolle ist der Tabellenwert:

```text
2022: 2.101,54 € Gesamtkosten – 2.454,00 € Vorauszahlung = 352,46 €
2023: 2.581,63 € Gesamtkosten – 3.120,00 € Vorauszahlung = 538,37 €
2024: 3.068,06 € Gesamtkosten – 3.120,00 € Vorauszahlung = 51,94 €
Summe: 942,77 €
```

Diese Rechnung ist eine Rechenkontrolle und ersetzt nicht die Prüfung der Originalabrechnungen und des Mietkontos.

---

## 6. Vorläufige Beweismatrix

| ID | Prüfgegenstand | Primärbeleg | Ergänzender Beleg | Offene Frage |
|---|---|---|---|---|
| B-01 | Mängelanzeigen und Kenntnis | Originalschriftverkehr | Chronologie | Wann wurde wer mit welchem Inhalt informiert? |
| B-02 | Heizungsausfälle/Temperatur | Protokolle und Originalkommunikation | Fotos/Videos, Zusatzheizkosten | Welche Betriebsbedingungen lagen konkret vor? |
| B-03 | Zusatzheizung und Zusatzkosten | Rechnungen/Zahlungsbelege | Temperaturaufzeichnungen | Sind Zeitraum und Verursachungsbezug belegbar? |
| B-04 | Stellventil-/Thermostatereignis 2023 | E-Mail und Vorher-/Nachher-Aufnahmen | Arbeitsbericht/Rechnung | Welche konkrete Arbeit wurde ausgeführt? |
| B-05 | HKV-Werte | Abrechnung/Ableseprotokoll | Geräte- und Wartungsdaten | Sind Geräte, Faktoren und Ablesungen nachvollziehbar? |
| B-06 | Warmwasserabweichung | Originalabrechnung | Video/Fotoprotokoll, Zählerdaten | Liegt ein Mess-, Übertragungs- oder Zuordnungsfehler vor? |
| B-07 | Gebäude-/Wohnungsebene | vollständige Abrechnung | Umlageschlüssel/Flächen | Wurde kein Gebäudewert als Wohnungswert übernommen? |
| B-08 | Abrechnung 2022 | Originalseiten der Abrechnung | Vorjahres-/Folgejahresvergleich | Ist der Wert Original, OCR-Fehler oder Übertragungsfehler? |
| B-09 | Kostenverteilung | Einzelabrechnung und Umlageschlüssel | CSV/XLSM/Berechnung | Sind Kostenart, Zeitraum und Verteilerschlüssel identisch? |
| B-10 | Jobcenter-Entscheidung | Bescheid, Berechnungsblatt, Akte | Anträge und Schriftverkehr | Welche Werte wurden tatsächlich berücksichtigt? |

---

## 7. Medien- und Integritätsstandard

Für jedes Foto oder Video werden erfasst:

- Index und Originaldateiname;
- unveränderter Repository-Pfad und Archivstand;
- Dateityp, Dateigröße und SHA-256-Prüfsumme;
- Metadaten, soweit vorhanden;
- behaupteter Aufnahmezeitpunkt getrennt vom technisch ausgelesenen Zeitpunkt;
- dargestelltes Objekt und sachliche Beschreibung;
- Bezug zu einer `B-*`-Frage oder `BK-1`-Jahresposition;
- mögliche alternative Erklärung;
- Hinweis, ob eine technische Begutachtung erforderlich ist.

Ein Foto oder Video belegt zunächst nur die dokumentierte Beobachtung. Ursache, Messfehler, Verantwortlichkeit oder Vorsatz werden daraus nicht ohne Weiteres abgeleitet.

Primärarchiv der Medien: [`diewand-hue/Nachweise-`](https://github.com/diewand-hue/Nachweise-), insbesondere [`Fotos`](https://github.com/diewand-hue/Nachweise-/tree/main/Fotos) und [`Videos`](https://github.com/diewand-hue/Nachweise-/tree/main/Videos).

---

## 8. Dokumentenmappe und Direktverknüpfung

Die spätere Druckmappe wird in dieser Reihenfolge aufgebaut:

1. `00_Deckblatt`
2. `01_Akten_und_Sachstandsuebersicht`
3. `02_Anschreiben_und_Pruefauftrag`
4. `03_Beweisverzeichnis_und_Register`
5. `04_Technische_Fehlerkette`
6. `05_Fotos_und_Videos`
7. `06_Nachweiszuordnung_nach_BK_Index`
8. `07_Schadensausgaben_BK_WW_Heizkosten`
9. `08_Rechnungen_und_Einzelbetraege`
10. `09_Beweislogik_und_Kausalzusammenhang`
11. `10_Anlagenverzeichnis_mit_Direktlinks`
12. `11_Abschluss_und_offene_Pruefpunkte`

Jede Anlage erhält einen Eintrag im Register. Der Eintrag enthält einen direkten Link zur Originaldatei und – wenn möglich – einen commitgebundenen Link. Drucklinks und aktuelle Arbeitslinks werden getrennt ausgewiesen.

---

## 9. Konkreter Prüfauftrag an das Jobcenter

Das Jobcenter soll insbesondere mitteilen:

1. Welche Abrechnungen und Nachforderungen lagen der jeweiligen Entscheidung zugrunde?
2. Welche Wohnungswerte und welche Gebäudewerte wurden berücksichtigt?
3. Welche Beträge wurden als Unterkunfts-, Heiz- oder Warmwasserkosten angesetzt?
4. Welche Berechnungsblätter, Prüfvermerke oder Rückfragen befinden sich in der Akte?
5. Wurden Originalbelege, Ablesedaten, Umlageschlüssel und Mietkonto geprüft?
6. Welche Unterlagen fehlen aus Sicht des Jobcenters?
7. Wird die Entscheidung bis zur Klärung widersprüchlicher Abrechnungswerte überprüft oder vorläufig angepasst?
8. Kann Akteneinsicht beziehungsweise eine Kopie der entscheidungserheblichen Berechnung gewährt werden?

Der Prüfauftrag bleibt auf die Leistungsentscheidung und die konkrete Sachverhaltsaufklärung beschränkt. Eine abschließende Haftungs- oder Vorsatzbehauptung wird daraus nicht vorweggenommen.

---

## 10. Noch erforderliche Unterlagen nach Priorität

### Priorität 1 – Zahlenprüfung

- Originalabrechnungen und Einzelbelege `BK-1`, insbesondere 2022–2024;
- vollständige Heizkosten-/Warmwasseraufteilung nach Kostenart;
- HKV-Rohablesungen, Geräte-IDs, Bewertungsfaktoren und Wechselprotokolle;
- Mietkonto `BK-5` und Nachweise der Vorauszahlungen;
- Jobcenter-Bescheide, Berechnungsbögen und Aktenauszüge.

### Priorität 2 – technische Prüfung

- Wartungs-, Eich-, Kalibrier- und Serviceunterlagen;
- Arbeitsberichte zur Thermostat-/Stellventilarbeit;
- Originalfotos und Originalvideos mit Metadaten;
- Temperatur- und Ereignisprotokolle;
- nachvollziehbare Geräte- und Zählerprüfung.

### Priorität 3 – Verfahrens- und Verantwortungszuordnung

- Belegeinsichtsanfragen und Antworten;
- vollständiger Schriftverkehr mit Verwaltung, Eigentümerin und Messdienstleister;
- Korrekturabrechnungen und sämtliche Versionen;
- Zahlungs- und Nachweisunterlagen zu Zusatzkosten.

---

## 11. Qualitätskontrolle vor der Einreichung

Die Mappe ist erst abgabebereit, wenn:

- jeder Betrag auf eine Originalseite oder einen Originaldatensatz verweist;
- jedes Foto und Video eindeutig indexiert ist;
- Originale und Auswertungskopien getrennt sind;
- Rechenwege reproduzierbar sind;
- Widersprüche offen markiert sind;
- Gebäude-, Wohnungs- und Jobcenterwerte getrennt bleiben;
- keine Hypothese als bewiesener Vorsatz, Betrug oder Haftung bezeichnet wird;
- das Jobcenter einen klaren und begrenzten Prüfauftrag erhält;
- die Direktlinks und Archivstände kontrolliert wurden;
- vor einer rechtlichen Verwendung eine fachkundige Prüfung erfolgt.

## Vorläufige Zusammenfassung

Der vorhandene Bestand liefert eine strukturierte Arbeitsgrundlage aus Abrechnungen, Tabellen, Kostenvergleichen, technischen Beobachtungen, Fotos, Videos und Schriftverkehr. Die zentrale Beweisführung lautet daher nicht pauschal „Fehler ist bewiesen“, sondern:

> **Es bestehen anhand der dokumentierten Tabellenwerte, Originalunterlagen und Medien konkrete und überprüfbare Auffälligkeiten in Kosten, Messung, technischer Funktion und Zuordnung. Diese Auffälligkeiten sind anhand der bezeichneten Originalbelege, Rechenwege und fehlenden Unterlagen vollständig zu prüfen.**
