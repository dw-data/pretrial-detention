# Abuse of pretrial detention in Germany and Europe

One in five people jailed in the EU haven't been convicted —  including 12,000 in Germany alone. Studies suggest that pretrial detention is unnecessary in most cases.

*In this repository, you will find the methodology, data and code behind
the story that came out of this analysis.*

Story by: [Kira
Schacht](https://www.twitter.com/daten_drang)


This project is part of a collaboration within the [European Data Journalism Network](https://www.europeandatajournalism.eu/).

Project lead: Civio

Collaborators: Deutsche Welle, Divergente, El Confidencial, EUrologus, OBCT, VoxEurop

**Read the full article on DW.com:** [English](https://www.dw.com/a-61983097) |
[German](https://www.dw.com/a-61983111)

**Main story by Civio:** [English](https://civio.es/2022/05/10/use-and-abuse-of-preventive-detention-in-the-european-union/) | [Spanish](https://civio.es/2022/05/10/uso-y-abuso-de-la-prision-provisional-en-la-union-europea/)

# Files

| Name                 | Content                                                                           |
| -------------------- | --------------------------------------------------------------------------------- |
| `pretrial detention in Germany data.xlsx`         | The Excel file containing the data used in this analysis |

# Data sources

## SPACE: Council of Europe Annual Penal Statistics 2021

Source: Council of Europe / University of Lausanne. [Link](https://wp.unil.ch/space/space-i/annual-reports/)

Annual reports on prison populations in European countries.

This analysis uses data from the 2021 annual report for European comparisons, which refers to data from 31st January 2021 unless otherwise stated. Namely, we used the following variables:

- `Table 3`: Number of inmates and prison population rates (adjusted and non-adjusted)
  - `3A`: Population of the country on 1st January 2021
  - `3B`: Total number of inmates (including pre-trial detainees) [Stock]
- `Table 8`: Prison population by legal status
  - `8A`: Total number of inmates not serving a final sentence
- `Table 16`: Prison capacity and prison density
  - `16A`: Total capacity of penal institutions

## German Federal Statistical Office: Prison population statistics 2019-2021
 
"Bestand der Gefangenen und Verwahrten in den deutschen Justizvollzugsanstalten nach ihrer Unterbringung auf Haftplätzen des geschlossenen und offenen Vollzugs" [Link](https://www.statistischebibliothek.de/mir/receive/DESerie_mods_00002496)

Monthly number of inmates in German jails and prisons, 2019-2021. We used the following variables:
- capacity ("`Belegungsfähigkeit am letzten Tag des Monats 24.00 Uhr insgesamt`")
- stock ("`Belegung am letzten Tag des Monats 24.00 Uhr insgesamt`")
- of which in remand detention ("`Untersuchungshaftvollzug insgesamt brutto`")

## German Federal Statistical Office: Prosecution statistics 2020

"Strafverfolgung – Fachserie 10 Reihe 3 – 2020" [Link](https://www.statistischebibliothek.de/mir/receive/DESerie_mods_00000107)

Annual reports on activities of criminal prosecution in Germany. Included is every person charged with a crime during that year.

For this analysis, we used the following variables:

- `6`: In der Strafverfolgungsstatistik 2020 erfasste Personen mit Untersuchungshaft
  - `6.1`:	Nach Grund und Dauer der Untersuchungshaft – Kurzfassung
    - type of crime (`Art der Straftat`)
    - registered persons total (`Erfasste Personen	insgesamt`)
    - of which with pretrial detention (`darunter mit Untersuchungshaft`)
    - because of flight risk (`Haftgründe (auch mehrere nebeneinander) > "flüchtig oder Fluchtgefahr (§ 112 Abs. 2 Nr.1,2 StPO)"`)
    - length of pretrial detention (`Dauer der Untersuchungshaft`)
  - `6.2`:	Nach Art der (späteren) Entscheidung – Kurzfassung
    - all variables, but only for row "all crimes" (`Straftaten insgesamt`)

## German Federal Statistical Office: People in pretrial detention by nationality

"Statistisches Bundesamt (Destatis), 2021 Sonderauswertung Strafverfolgungsstatistik Berichtsjahr 2019" [Link](https://www.destatis.de/DE/Themen/Staat/Justiz-Rechtspflege/Tabellen/sonderauswertung-untersuchungshaft.html;jsessionid=8BF2529706786B5019F12CD7ABF84CFE.live731)

Number of people in pretrial detention in 2019, brakdown by German / non-German nationality.

## Studies on flight risk as a cause for pretrial detention in Germany

- Wolf, Lara: Die Fluchtprognose im U-Haft-Recht, 1. Auflage 2017, Baden-Baden. [Link](https://doi.org/10.5771/9783845286891)
  - 169 cases between 2000 and 2015
  - criteria: flight risk assumed by court, but defendant released for procedural reasons, e.g. missed deadlines
  - results: 14 fled, 155 (92%) did not flee
- Lind, Detlef: „Der Strafverteidiger“, 2019, Seite 118 bis 132 [Link](https://www.liebert-roeth.de/de/rechtsgebiete/strafrecht/216-missbrauch-der-untersuchungshaft)
  - 65 cases between 2009-2016
  - criteria: flight risk assumed, but defendant released anyway
  - results: 1 fled, 64	did not flee

# Interviews

- [Christine Morgenstern](https://www.jura.fu-berlin.de/fachbereich/einrichtungen/strafrecht/lehrende/morgensternc/index.html),	professor of criminal law and gender studies at the Free University of Berlin, who researched pretrial detention in Europe in her [postdoctoral thesis](https://www.irks.at/detour/publications.html).
- [Thomas Röth](https://www.liebert-roeth.de/de/team/rechtsanwalt-thomas-roeth),	Lawyer in Berlin, [writes about](https://www.liebert-roeth.de/de/rechtsgebiete/strafrecht/216-missbrauch-der-untersuchungshaft) pretrial detention in Germany.
- [Lara Wolf](https://www.strafrechtskanzlei.de/dr-lara-wolf/), criminal defense laywer, wrote [dissertation](https://doi.org/10.5771/9783845286891) about the use of flight risk as a cause for pretrial detention in Germany.