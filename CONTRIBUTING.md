# Mitwirken: das Gesetzgebungsverfahren

Das Mittagspointengesetz (MiPoG) ändert nur die Tischrunde, die es sich gegeben hat. Dieses Repository ist das Gesetzblatt; GitHub ist der Weg, Anträge und Entwürfe einzureichen. Alles hier ist öffentlich: keine Namen von Mitgliedern, nichts, was am Tisch gesagt wurde (§ 3a MiPoG).

## Verfahren

1. **Antrag.** Ein Issue „Antrag an den Gesetzgeber“ (Vorschrift, Antrag, Begründung) oder eine E-Mail an burow(at)borisburow.de. Label „Antrag“.
2. **Entwurf.** Ein Pull Request mit der Änderung an `gesetz/mipog.md`, nach der Vorlage „Gesetzentwurf“. Label „Entwurf“. Begründung und Anhang in derselben Datei dürfen angepasst werden.
3. **Beschluss.** Das Gesetz ändert nur die Tischrunde: mit zwei Dritteln der anwesenden Mitglieder, wenn mindestens die Hälfte aller Mitglieder anwesend ist (§ 30 Abs. 1 Satz 1). Die §§ 3a und 16a können nur einstimmig geändert werden (Satz 2); dasselbe gilt für jede Änderung, die ihren Schutz verkürzt. § 3, § 12, § 20 und § 30 Abs. 2 sind unabänderlich. Ergebnis: Label „Beschlossen“ oder „Abgelehnt“.
4. **Verkündung.** Der Punktewart merged den Pull Request. Zugleich entstehen die neue Fassung `gesetz/fassungen/JJJJ-MM-TT.md` (identisch mit `mipog.md`) und ein Eintrag in `gesetz/chronik.yml`. Commit: „MiPoG: Fassung vom …“. Webseite und PDFs auf mipog.de werden aus diesem Repository gebaut.

## Außerdem

- **Redaktionelles.** Begründung und Anhang sind nicht Teil des Gesetzes. Korrekturen dort brauchen keinen Beschluss: Label „Redaktionelles“.
- **Beitritt.** Ein Tisch, der das Gesetz übernimmt, meldet sich mit dem Issue „Beitrittserklärung“ (Name des Tisches, Ort, Datum des Beschlusses). Label „Beitritt“. Er wird in `gesetz/vertragsstaaten.yml` eingetragen.
- **Rezeption.** Wer das Gesetz für den eigenen Tisch anders haben will, forkt das Repository. Ein Fork ist ein eigener Staat; seine Änderungen binden die Ursprungsrunde nicht.

## Konventionen in gesetz/mipog.md

- `# Titel (Kurzbezeichnung – Abkürzung)`, dann `## Präambel`, danach `## Abschnitt N – Titel`
- `### § N Titel`, N auch mit Buchstabe (3a, 16a); Absätze beginnen mit `(1) `; eine nummerierte Liste gehört zum vorangehenden Absatz
- **Fett** markiert Legaldefinitionen
- `## Anlage – Punktetabelle` (Tabelle `Tatbestand | Punkte | Fundstelle`, danach ein Absatz „Beispiel: …“), `## Begründung (Auszug)` (Absätze `**Zu § N …:** Text`), `## Anhang – Juristendeutsch für Nichtjuristen`
- Verweise wie „§ 7 Absatz 1“ oder „§§ 23 bis 25“ werden auf der Webseite zu Links

## Labels

| Label | Bedeutung |
| --- | --- |
| Antrag | Antrag an den Gesetzgeber, noch nicht beraten |
| Entwurf | Pull Request mit Änderung an `gesetz/mipog.md` |
| Beschlossen | von der Tischrunde nach § 30 beschlossen |
| Abgelehnt | von der Tischrunde abgelehnt |
| Beitritt | Beitrittserklärung eines Tisches |
| Redaktionelles | ohne Beschluss, nicht Teil des Gesetzes |
