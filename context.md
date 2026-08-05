# context.md — domain background for the Lourdes chronology

Read together with `AGENTS.md` (operating rules) and `KEYWORDS.md` (naming
variants). This file is background for agents and contributors; it is not
rendered on the site.

## The subject in one paragraph

Between 11 February and 16 July 1858, Bernadette Soubirous, a fourteen-year-old
miller's daughter, reported 18 apparitions of "a Lady" at the Massabielle
grotto outside Lourdes, in the diocese of Tarbes (France). The reported series
includes the uncovering of a spring (25 February), a request for processions
and a chapel (2 March), and — on 25 March, asked her name — the answer in
Gascon Occitan reported as "Que soy era Immaculada Concepciou" ("I am the
Immaculate Conception"). The civil authorities interrogated Bernadette
(commissioner Jacomet, 21 February) and boarded up the grotto; the Church
investigated through a commission opened by Bishop Bertrand-Sévère Laurence
of Tarbes on 28 July 1858, whose decree of 18 January 1862 judged the
apparitions real and authorized the cult. Lourdes became one of the largest
Catholic pilgrimage sites; its Medical Bureau (1883) examines claimed cures,
the International Medical Committee (1954) judges whether they are unexplained,
and diocesan bishops have declared 72 of them miraculous per the Sanctuary's
count (as of 2025). Four churches were built at the grotto between 1866 and
1958, and the volunteer Hospitality dates from 1885.

## The datable spine

| Date | Event | Status |
|---|---|---|
| 1854-12-08 | Pius IX, *Ineffabilis Deus*, defines the Immaculate Conception | verified (vatican.va) |
| 1858-02-11 → 1858-07-16 | 18 reported apparitions | verified (Sanctuary site) |
| 1858-02-21 | Jacomet interrogation | verified (Sanctuary site) |
| 1858-02-25 | spring uncovered (9th reported apparition) | verified |
| 1858-03-25 | "Immaculate Conception" statement, reported in Gascon | verified (as a report) |
| 1858-06 | civil authorities close the grotto; reopened 5 Oct 1858 | **unverified** — 7 vs 15 June, reopening tertiary-sourced (see dateNote) |
| 1858-07-28 | episcopal commission opened | verified |
| 1862-01-18 | Laurence decree — THE approval document | verified; decree text quoted on the Sanctuary's recognition page |
| 1862-01-18 | the SAME decree recognizes the first seven cures | verified (Sanctuary's list of recognized cures) |
| 1866-05-19 | crypt opened — the first church at the grotto | verified (Lourdes Tourist Office; Sanctuary keeps the anniversary) |
| 1866-07 | Bernadette to Saint-Gildard, Nevers | month verified; day NOT pinned (see dateNote) |
| 1876-07-01 | Immaculate Conception basilica consecrated; statue crowned | consecration day contested 1 vs 2 July *by the Sanctuary's own two sites* (dateNote) |
| 1879-04-16 | death of Bernadette | verified |
| 1883 | Medical Bureau founded | verified (Sanctuary site) |
| 1885 | Hospitality of Our Lady of Lourdes founded | verified (Sanctuary site) |
| 1901-10-06 | Rosary Basilica consecrated (first stone 16 July 1883) | verified (Sanctuary site) |
| 1907 | memorial inserted into the Roman calendar — a liturgical concession | year verified (Vatican City State); no day, no pope named in an official source |
| 1907–1913 | 33 of the 72 recognitions fall in these years, 20 in 1908 | verified by counting the Sanctuary's own list |
| 1925-06-14 | beatification | date NOT yet verified against a Holy See document |
| 1933-12-08 | canonization by Pius XI, deliberately on the Immaculate Conception feast | verified |
| 1954 | International Medical Committee of Lourdes (CMIL) created (1947 antecedent) | verified (Sanctuary site) |
| 1958-03-25 | Basilica of Saint Pius X consecrated, centenary year | verified (Sanctuary site) |
| 2018-02-11 | Moriau cure declared 70th recognized miracle (Bp. of Beauvais) | verified (French Bishops' Conference) |
| 2024-12-08 | Traynor cure declared 71st recognized miracle (Abp. of Liverpool) | verified (Sanctuary site) |
| 2025-04-16 | Raco cure declared 72nd recognized miracle (Bp. of Tursi-Lagonegro) | verified (Sanctuary site) |

## Reported miracles: the rule this repo models (core#71)

A miracle is a **claim**, not an event. Only two things attached to one are
datable and may enter `events[]`:

1. **The account** — that a cure was *reported*, by whom, when first attested.
2. **The recognition act** — a bishop's dated declaration, with a document.

This repo was already the family's worked example and the widening extended it
rather than diluting it. Concretely, after core#71 the dataset carries **five**
cure events and every one of them is a Church act or an attributed count:

- `1862-01-18` — the first **seven** recognitions, in the approval decree
  itself. Filed as a separate event from the apparition judgment on purpose:
  one document, two different kinds of act, and running them together is the
  exact confusion the dataset exists to prevent.
- `1907–1913` — the jubilee **wave**: 33 of the 72 recognitions, 20 of them in
  1908, five on 6 June 1908 alone, then a 33-year gap to 20 May 1946. An
  aggregate, and it is attributed to the Sanctuary's published list, which is
  where it was counted from.
- `2018-02-11`, `2024-12-08`, `2025-04-16` — three named bishops' declarations
  (Beauvais, Liverpool, Tursi-Lagonegro), each with the act's own wording.

No `title` in this dataset says "N was cured". The Medical Bureau and the CMIL
find cures *unexplained* and declare no miracle — that is stated in both
organizations' `relation` and in a disambiguation item. **Cures earn no rung on
the approval ladder**, which was not edited in this wave: no new Church act on
the *apparitions* turned up.

## Why this subject is contested terrain

Not because the approval is disputed inside the Church — Lourdes is the
textbook approved apparition — but because the epistemic registers are easy
to flatten:

- **Report vs fact.** Everything supernatural in this story enters the record
  as Bernadette's report or the Church's judgment on it. The site's own voice
  states only the documented acts.
- **Approval is an act, not an adjective.** "Approved" means: Laurence's
  decree, 18 January 1862, with quotable text. Later papal gestures (feast,
  basilicas, canonization of Bernadette) are separate dated acts.
- **Canonization ≠ apparition approval.** Bernadette's cause judged her life
  and virtues; the Sanctuary itself stresses she was canonized "not for
  having been chosen for the Apparitions".
- **Cures.** The Medical Bureau finds a cure "unexplained"; only the cured
  person's diocesan bishop declares it miraculous. The dataset records the
  recognition acts and attributes the count (72, Sanctuary, 2025; an older
  Sanctuary page still says 70).
- **The 1854 dogma predates the 1858 phrase.** *Ineffabilis Deus* is dated
  precisely because the whole significance of the 25 March statement hangs on
  that four-year gap.
- **Cult acts are not verdicts.** The crowning of the statue (1876) and the
  memorial's entry into the Roman calendar (1907) are acts of *cult* — an
  honour to an image, a devotion permitted then universalised. Both are now in
  the chronology, both are worded as concessions, and a disambiguation item
  says so. Neither may be read as Rome ruling on the apparitions: the ladder's
  Rome rung is `not-reached` and nothing added here touches it.
- **The Sanctuary disagrees with itself, and that is kept.** Not only 70 vs 72
  cures: its two sites also date the Immaculate Conception basilica's
  consecration 1 July and 2 July 1876. Both recorded, neither preferred.

## Known gaps and unverified items (as of the 2026-08-05 core#71 wave)

- **Beatification day (14 June 1925)**: only encyclopedic sources so far;
  `dateVerified: false` until a Holy See document (AAS 17, 1925) is cited.
- **July 1866 chronology** (departure 4 July / arrival 7 July / habit
  29 July): accounts subdivide the month differently; event dated `1866-07`
  with a `dateNote`.
- **Bishop Laurence's biographical dates** are not asserted (figure carries
  role only).
- **Jacomet's first name** (Dominique in most accounts) is not on the
  Sanctuary page cited — noted inline, not asserted from memory.
- **The full text of the 1862 decree** is quoted only in the fragments given
  on the Sanctuary's recognition page; a full-text primary (diocesan archive,
  Laurentin's *Lourdes. Documents authentiques*) is a follow-up.
- **~~The 2025 recognition (Antonia Raco)~~ CLOSED.** The Sanctuary's own page
  gives the act: Mgr Vincenzo Carmine Orofino, Bishop of Tursi-Lagonegro,
  16 April 2025, on the CMIL's 2024 vote. Seeded as an event.
- **~~Not yet covered: crypt, basilicas, feast, per-cure recognitions~~
  MOSTLY CLOSED.** The crypt (1866), the Immaculate Conception basilica and the
  crowning (1876), the Rosary basilica (1901), Saint Pius X (1958), the
  Hospitality (1885), the CMIL (1954), the feast (1907) and three further
  recognition acts are now events.
- **The 1858 closing of the grotto is the weakest new event.** Dated `1858-06`,
  `dateVerified: false`. The Sanctuary says access was prohibited "from 15th
  June"; French Wikipedia says the barricading was 7 June and the reopening
  5 October 1858 on Napoleon III's order. No prefectoral or municipal act, and
  no archival document, was located for either date — the reopening rests on a
  tertiary source alone. A French departmental archive would settle it.
- **The Sanctuary's list of 72 names no declaring bishop** and, for most cases,
  no date of cure. That is why only four individual recognitions are events
  (1862 ×7 collectively, 2018, 2024, 2025) and the 1907–1913 cluster is
  recorded as a *count* rather than as 33 separate rows: filling in bishops
  from devotional compilations would be exactly the failure mode core#71
  describes. The counts here were made by reading the Sanctuary's own list.
- **Still not covered, deliberately:** Pius XII's *Le pèlerinage de Lourdes*
  (1957) as an event — it is cited as a reference and quoted in the ladder, but
  no event was added because it is an encyclical *about* the centenary rather
  than an act; the papal visits (1983, 2004, 2008); the Nevers exhumations
  (1909, 1919, 1925) and the state of Bernadette's body, which is devotionally
  contested and needs its own sourcing; and the 1873 national pilgrimage.

## Glossary

No `[[term-id]]` cross-links are used yet; the pinned
`data/glossary-terms.json` has no Lourdes-specific terms. Candidates to
propose to `cronologia/glossary`: *apparition (approved)*, *constat de
supernaturalitate*, *canonization*.
