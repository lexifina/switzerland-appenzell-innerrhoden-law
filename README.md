# Appenzell Innerrhoden: law history in git

The law of the canton of Appenzell Innerrhoden (Kanton Appenzell Innerrhoden, Switzerland) as a git history: one file per article, one commit per amending act on the day it took effect, and the amending act as the commit's author. `git blame` names the act behind every paragraph; `git log` lists every change to an article; checking out a date gives the text in force that day.

It follows the shared design of [lexifina/global-law](https://github.com/lexifina/global-law), which places it at `ch-ai/`. The federal law is in [lexifina/switzerland-law](https://github.com/lexifina/switzerland-law).

The text is in German, the canton's official language, exactly as the canton publishes it.

## What this repository holds

183 acts with 302 versions so far: the cantonal constitution, the cantonal laws (Gesetze) in force and 119 Verordnungen and Reglemente in force, in the order of the systematic collection, added in parts. Other decrees and decisions, intercantonal agreements and repealed acts are not included yet.

| Folder | Act | Versions | History |
| --- | --- | ---: | --- |
| `101-000/` | Verfassung für den Eidgenössischen Stand Appenzell I. Rh. (GS 101.000) | 3 | oldest version available, then each consolidated version: 1 May 2018 to 1 May 2022 |
| `142-500-integrationsgesetz-intg/` | Gesetz über die Einführung der Integrationsbestimmungen des Bundesgesetzes über die Ausländerinnen und Ausländer (GS 142.500) | 1 | as enacted, 19 October 2009 |
| `172-600-verwvg/` | Verwaltungsverfahrensgesetz (GS 172.600) | 1 | one version (the oldest available), 1 June 2018 |
| `172-700-frig/` | Gesetz über den Fristenlauf (GS 172.700) | 2 | oldest version available, then each consolidated version: 27 April 2003 to 1 May 2025 |
| `172-800-diag/` | Datenschutz-, Informations- und Archivgesetz (GS 172.800) | 2 | oldest version available, then each consolidated version: 24 April 2016 to 1 January 2020 |
| `173-000-gog/` | Gerichtsorganisationsgesetz (GS 173.000) | 5 | oldest version available, then each consolidated version: 1 August 2014 to 1 January 2024 |
| `173-400-verwgg/` | Verwaltungsgerichtsgesetz (GS 173.400) | 2 | oldest version available, then each consolidated version: 27 April 2014 to 1 May 2025 |
| `175-600-fusionsgesetz-fusg/` | Gesetz über die Fusion von Bezirken und Schulgemeinden (GS 175.600) | 1 | one version (the oldest available), 23 October 2017 |
| `177-000-anwg/` | Anwaltsgesetz (GS 177.000) | 1 | one version (the oldest available), 29 April 2007 |
| `211-000-eg-zgb/` | Einführungsgesetz zum Schweizerischen Zivilgesetzbuch (GS 211.000) | 2 | oldest version available, then each consolidated version: 1 May 2018 to 1 June 2024 |
| `211-400-zeddelgesetz-zeg/` | Gesetz über die Verpfändung der Liegenschaften (GS 211.400) | 1 | one version (the oldest available), 26 April 2015 |
| `211-500-eg-bewg/` | Einführungsgesetz zum Bundesgesetz über den Erwerb von Grundstücken durch Personen im Ausland (GS 211.500) | 1 | one version (the oldest available), 1 January 2011 |
| `211-600-geodg/` | Geodatengesetz (GS 211.600) | 2 | as enacted, then each consolidated version: 1 July 2011 to 1 January 2020 |
| `280-100-eg-schkg/` | Einführungsgesetz zum Bundesgesetz über Schuldbetreibung und Konkurs (GS 280.100) | 4 | oldest version available, then each consolidated version: 26 April 2015 to 1 June 2024 |
| `311-000-uestg/` | Übertretungsstrafgesetz (GS 311.000) | 1 | one version (the oldest available), 26 April 2015 |
| `411-000-schg/` | Schulgesetz (GS 411.000) | 1 | one version (the oldest available), 23 October 2017 |
| `413-000-eg-bbg/` | Einführungsgesetz zum Bundesgesetz über die Berufsbildung (GS 413.000) | 1 | one version (the oldest available), 1 January 2011 |
| `414-100/` | Gesetz über Kostenbeiträge an kantonale Hochschulen (GS 414.100) | 1 | one version (the oldest available), 30 April 2006 |
| `415-000-sportg/` | Sportgesetz (GS 415.000) | 1 | one version (the oldest available), 30 April 2017 |
| `416-000-ausbg/` | Gesetz über Ausbildungsbeiträge (GS 416.000) | 2 | oldest version available, then each consolidated version: 1 August 2014 to 1 August 2021 |
| `442-000/` | Gesetz über die Errichtung einer Stiftung «Pro Innerrhoden» (GS 442.000) | 2 | oldest version available, then each consolidated version: 30 April 2006 to 1 January 2021 |
| `442-100/` | Gesetz über die Errichtung einer Innerrhoder Kunststiftung (GS 442.100) | 2 | oldest version available, then each consolidated version: 30 April 2006 to 1 January 2021 |
| `446-000/` | Kulturgesetz (GS 446.000) | 1 | one version (the oldest available), 30 April 2006 |
| `520-000-eg-bzg/` | Einführungsgesetz zum Bundesgesetz über den Bevölkerungsschutz und den Zivilschutz sowie zum Bundesgesetz über den Schutz der Kulturgüter bei bewaffneten Konflikten (GS 520.000) | 1 | one version (the oldest available), 26 April 2015 |
| `550-000-polg/` | Polizeigesetz (GS 550.000) | 2 | oldest version available, then each consolidated version: 5 September 2017 to 1 January 2020 |
| `560-100-hug/` | Hundegesetz (GS 560.100) | 1 | one version (the oldest available), 1 January 2011 |
| `613-000-fag/` | Finanzausgleichsgesetz (GS 613.000) | 1 | one version (the oldest available), 1 January 2011 |
| `640-000-stg/` | Steuergesetz (GS 640.000) | 3 | oldest version available, then each consolidated version: 23 October 2017 to 1 January 2024 |
| `685-000-gnu/` | Gesetz über die Nutzung des Untergrundes (GS 685.000) | 1 | as enacted, 1 January 2019 |
| `688-000/` | Gesetz über die Versorgung mit Radio- und Fernsehprogrammen (GS 688.000) | 1 | one version (the oldest available), 25 April 2004 |
| `700-000-baug/` | Baugesetz (GS 700.000) | 3 | oldest version available, then each consolidated version: 1 May 2017 to 1 April 2026 |
| `710-000-entg/` | Enteignungsgesetz (GS 710.000) | 2 | oldest version available, then each consolidated version: 25 April 2004 to 1 June 2024 |
| `721-000-wbaug/` | Wasserbaugesetz (GS 721.000) | 1 | one version (the oldest available), 1 May 2018 |
| `725-000-strg/` | Strassengesetz (GS 725.000) | 2 | oldest version available, then each consolidated version: 26 April 2015 to 1 August 2021 |
| `725-300-eg-fwg/` | Einführungsgesetz zum Bundesgesetz über Fuss- und Wanderwege (GS 725.300) | 1 | one version (the oldest available), 1 January 2011 |
| `726-100-egob/` | Einführungsgesetz über das öffentliche Beschaffungswesen (GS 726.100) | 1 | as enacted, 1 November 2022 |
| `730-000-energ/` | Energiegesetz (GS 730.000) | 3 | oldest version available, then each consolidated version: 1 January 2011 to 9 May 2021 |
| `740-300-gov/` | Gesetz über den öffentlichen Verkehr (GS 740.300) | 1 | as enacted, 1 January 2017 |
| `741-000-eg-svg/` | Einführungsgesetz zum Strassenverkehrsgesetz (GS 741.000) | 2 | oldest version available, then each consolidated version: 1 January 2011 to 1 May 2019 |
| `800-000-gesg/` | Gesundheitsgesetz (GS 800.000) | 1 | one version (the oldest available), 1 June 2018 |
| `801-300-altershilfegesetz-ahig/` | Gesetz über die öffentliche Altershilfe (GS 801.300) | 1 | one version (the oldest available), 24 April 2005 |
| `810-000-ggz/` | Gesetz über das Gesundheitszentrum Appenzell (GS 810.000) | 2 | as enacted, then each consolidated version: 27 April 2003 to 1 January 2019 |
| `814-000-eg-usg/` | Einführungsgesetz zum Bundesgesetz über den Umweltschutz (GS 814.000) | 1 | one version (the oldest available), 1 January 2011 |
| `814-300-eg-gschg/` | Einführungsgesetz zum Bundesgesetz über den Schutz der Gewässer (GS 814.300) | 1 | one version (the oldest available), 26 April 2015 |
| `822-200-ruhetagsgesetz/` | Gesetz über die öffentlichen Ruhetage (GS 822.200) | 1 | one version (the oldest available), 1 January 2011 |
| `831-200-gel/` | Gesetz über Ergänzungsleistungen zur Alters-, Hinterlassenen- und Invalidenversicherung (GS 831.200) | 1 | as enacted, 27 April 2008 |
| `836-000-fzg/` | Gesetz über die Familienzulagen (GS 836.000) | 1 | one version (the oldest available), 1 January 2013 |
| `837-000-avalg/` | Gesetz über die Arbeitsvermittlung und die Arbeitslosenversicherung (GS 837.000) | 1 | one version (the oldest available), 1 January 2011 |
| `844-000-wsg/` | Gesetz über die Unterstützung von Wohnbausanierungen (GS 844.000) | 1 | as enacted, 15 June 2009 |
| `850-000-sozialhilfegesetz-shig/` | Gesetz über die öffentliche Sozialhilfe (GS 850.000) | 1 | one version (the oldest available), 1 August 2014 |
| `900-000-wirtschaftsforderungsgesetz-wfg/` | Gesetz über die Förderung der Wirtschaft (GS 900.000) | 1 | one version (the oldest available), 24 April 2005 |
| `910-000-lag/` | Landwirtschaftsgesetz (GS 910.000) | 2 | oldest version available, then each consolidated version: 26 April 2015 to 1 May 2024 |
| `911-000/` | Einführungsgesetz zum Bundesgesetz über das bäuerliche Bodenrecht (GS 911.000) | 2 | oldest version available, then each consolidated version: 26 April 2015 to 1 June 2024 |
| `913-000/` | Gesetz über die Flurgenossenschaften (GS 913.000) | 1 | one version (the oldest available), 1 May 2007 |
| `916-500/` | Alpgesetz (GS 916.500) | 1 | one version (the oldest available), 26 April 2015 |
| `921-000-eg-wag/` | Einführungsgesetz zum Bundesgesetz über den Wald (GS 921.000) | 1 | one version (the oldest available), 1 January 2013 |
| `922-000-jag/` | Jagdgesetz (GS 922.000) | 2 | oldest version available, then each consolidated version: 1 January 2011 to 1 July 2025 |
| `923-000-fischg/` | Fischereigesetz (GS 923.000) | 1 | one version (the oldest available), 1 January 2011 |
| `930-000-hgpg/` | Gesetz über die Handels- und Gewerbepolizei (GS 930.000) | 1 | one version (the oldest available), 1 January 2011 |
| `935-100-tfg/` | Tourismusförderungsgesetz (GS 935.100) | 2 | oldest version available, then each consolidated version: 25 April 2004 to 1 January 2020 |
| `935-300-gastgewerbegesetz-gag/` | Gesetz über das Gastgewerbe und den Handel mit alkoholischen Getränken (GS 935.300) | 2 | oldest version available, then each consolidated version: 1 January 2011 to 1 January 2021 |
| `935-500-eg-bgs/` | Einführungsgesetz zum Bundesgesetz über Geldspiele (GS 935.500) | 2 | as enacted, then each consolidated version: 27 April 2008 to 1 January 2021 |
| `951-000-kbg/` | Gesetz über die Appenzeller Kantonalbank (GS 951.000) | 2 | oldest version available, then each consolidated version: 1 January 2007 to 1 January 2019 |
| `963-100-feuerschutzgesetz-fsg/` | Gesetz über den Feuerschutz (GS 963.100) | 1 | one version (the oldest available), 1 January 2007 |
| `141-010-vlg/` | Verordnung über das Landrecht und das Gemeindebürgerrecht (GS 141.010) | 2 | oldest version available, then each consolidated version: 1 January 2018 to 1 January 2020 |
| `142-110-auslanderverordnung-ausv/` | Vollzugsverordnung zum Bundesgesetz über Ausländerinnen und Ausländer (GS 142.110) | 1 | as enacted, 23 March 2009 |
| `142-210-asylv/` | Verordnung über das Asylwesen (GS 142.210) | 1 | as enacted, 23 March 2009 |
| `142-510-integrationsverordnung-intv/` | Verordnung zum Integrationsgesetz (GS 142.510) | 1 | as enacted, 19 October 2009 |
| `160-010-vua/` | Verordnung über die Urnenabstimmungen (GS 160.010) | 3 | as enacted, then each consolidated version: 1 January 2018 to 1 October 2024 |
| `160-020-vau/` | Verordnung über ausserordentliche Urnenabstimmungen (GS 160.020) | 2 | as enacted, then each consolidated version: 8 February 2021 to 25 October 2021 |
| `160-110-viv/` | Verordnung über das Initiativverfahren (GS 160.110) | 2 | as enacted, then each consolidated version: 1 January 2018 to 8 February 2021 |
| `160-410-vlgv/` | Verordnung über die Landsgemeinde und die Gemeindeversammlungen (GS 160.410) | 1 | one version (the oldest available), 1 January 2018 |
| `170-010-behv/` | Behördenverordnung (GS 170.010) | 5 | oldest version available, then each consolidated version: 1 December 2014 to 1 June 2024 |
| `171-210-grgr/` | Geschäftsreglement des Grossen Rates (GS 171.210) | 3 | oldest version available, then each consolidated version: 1 December 2014 to 1 January 2021 |
| `172-110-depv/` | Verordnung über die Departemente (GS 172.110) | 3 | oldest version available, then each consolidated version: 1 December 2014 to 1 May 2025 |
| `172-113-gr-stk/` | Geschäftsreglement der Standeskommission (GS 172.113) | 2 | as enacted, then each consolidated version: 1 January 2022 to 17 June 2025 |
| `172-310-pev/` | Personalverordnung (GS 172.310) | 6 | oldest version available, then each consolidated version: 1 January 2017 to 1 January 2027 |
| `172-316-spesenreglement/` | Reglement über Spesen und weitere Vergütungen (GS 172.316) | 6 | as enacted, then each consolidated version: 1 January 2018 to 1 August 2025 |
| `172-317/` | Reglement über die Aus- und Weiterbildung (GS 172.317) | 2 | as enacted, then each consolidated version: 1 January 2018 to 1 May 2026 |
| `172-410/` | Verordnung über die Kantonale Versicherungskasse (GS 172.410) | 2 | as enacted, then each consolidated version: 1 January 2014 to 1 January 2027 |
| `172-510-gebv/` | Gebührenverordnung (GS 172.510) | 2 | as enacted, then each consolidated version: 1 January 2020 to 1 November 2021 |
| `172-910-regv/` | Verordnung zum Bundesgesetz über die Harmonisierung der Einwohnerregister und anderer amtlicher Personenregister (GS 172.910) | 1 | as enacted, 16 June 2008 |
| `173-001/` | Reglement über die Gerichtsberichterstattung (GS 173.001) | 3 | oldest version available, then each consolidated version: 13 November 2009 to 11 February 2026 |
| `173-510-vab/` | Verordnung über die Anstellung des Bezirksgerichtspräsidenten (GS 173.510) | 2 | oldest version available, then each consolidated version: 3 February 2014 to 1 January 2021 |
| `173-810-ggv/` | Verordnung über die Gebühren der Gerichte (GS 173.810) | 2 | oldest version available, then each consolidated version: 1 December 2014 to 1 January 2024 |
| `175-210/` | Verordnung über die Grenzen der Bezirke, der Schul- und Kirchgemeinden sowie der Feuerschaugemeinde Appenzell (GS 175.210) | 3 | as enacted, then each consolidated version: 22 October 2007 to 1 May 2022 |
| `175-610-fusv/` | Fusionsverordnung (GS 175.610) | 1 | as enacted, 1 January 2020 |
| `177-301/` | Reglement über die Prüfungen für die Zulassung zum Anwaltsberuf (GS 177.301) | 1 | one version (the oldest available), 11 November 2013 |
| `177-310/` | Verordnung über die Gebühren der Anwaltskammer (GS 177.310) | 1 | one version (the oldest available), 1 December 2014 |
| `177-410-anwhv/` | Verordnung über die Honorare der Anwälte (GS 177.410) | 2 | oldest version available, then each consolidated version: 1 December 2014 to 1 January 2024 |
| `178-710/` | Verordnung über die öffentliche Beurkundung (GS 178.710) | 3 | oldest version available, then each consolidated version: 1 December 2014 to 1 June 2024 |
| `211-110-ziv/` | Zivilstandsverordnung (GS 211.110) | 2 | oldest version available, then each consolidated version: 1 July 2017 to 1 July 2024 |
| `211-430-vvp/` | Verordnung über die Viehverpfändung (GS 211.430) | 3 | oldest version available, then each consolidated version: 1 December 2014 to 1 June 2024 |
| `211-450/` | Verordnung über die Schätzung von Grundstücken (GS 211.450) | 4 | oldest version available, then each consolidated version: 1 December 2014 to 1 June 2024 |
| `211-460-veu/` | Verordnung über die elektronische Überwachung im Zivilrecht (GS 211.460) | 1 | as enacted, 1 April 2024 |
| `211-620-vgb/` | Verordnung über das Grundbuch (GS 211.620) | 4 | oldest version available, then each consolidated version: 1 December 2014 to 1 June 2024 |
| `211-640/` | Verordnung über das Alpregister im Grundbuch (GS 211.640) | 3 | oldest version available, then each consolidated version: 1 December 2014 to 1 June 2024 |
| `211-914/` | Gebührenreglement der BVG- und Stiftungsaufsicht der Kantone Zürich, Glarus, Schaffhausen, Appenzell Ausserrhoden, Appenzell Innerrhoden, St. Gallen, Graubünden, Thurgau und Tessin (GS 211.914) | 1 | as enacted, 1 January 2026 |
| `221-310-vlp/` | Verordnung zum Bundesgesetz über die landwirtschaftliche Pacht (GS 221.310) | 2 | oldest version available, then each consolidated version: 1 December 2014 to 1 January 2022 |
| `311-010-vob/` | Verordnung über die Ordnungsbussen (GS 311.010) | 3 | oldest version available, then each consolidated version: 1 December 2014 to 1 August 2023 |
| `312-410-voh/` | Verordnung zum Bundesgesetz über die Opferhilfe (GS 312.410) | 2 | oldest version available, then each consolidated version: 1 December 2014 to 1 January 2025 |
| `411-010-schv/` | Schulverordnung (GS 411.010) | 3 | oldest version available, then each consolidated version: 23 October 2017 to 1 August 2022 |
| `411-510-vgd/` | Verordnung über die gesundheitlichen Dienste in den Schulen (GS 411.510) | 3 | oldest version available, then each consolidated version: 5 December 2016 to 1 August 2024 |
| `412-010-gymv/` | Gymnasialverordnung (GS 412.010) | 1 | one version (the oldest available), 1 February 2016 |
| `413-010-veg-bbg/` | Verordnung zum Einführungsgesetz zum Bundesgesetz über die Berufsbildung (GS 413.010) | 1 | one version (the oldest available), 1 January 2011 |
| `415-010-sportv/` | Sportverordnung (GS 415.010) | 1 | one version (the oldest available), 23 October 2017 |
| `416-010-ausbv/` | Verordnung über Ausbildungsbeiträge (GS 416.010) | 2 | oldest version available, then each consolidated version: 1 May 2017 to 1 August 2021 |
| `417-410/` | Verordnung über die Erwachsenenbildung (GS 417.410) | 1 | one version (the oldest available), 1 December 2014 |
| `445-010-archv/` | Archäologieverordnung (GS 445.010) | 1 | as enacted, 1 January 2013 |
| `446-010/` | Verordnung zum Kulturgesetz (GS 446.010) | 1 | one version (the oldest available), 23 October 2006 |
| `450-010-vnh/` | Verordnung über den Natur- und Heimatschutz (GS 450.010) | 2 | oldest version available, then each consolidated version: 1 January 2017 to 1 April 2026 |
| `502-010-ev-wg/` | Einführungsverordnung zum Bundesgesetz über Waffen, Waffenzubehör und Munition (GS 502.010) | 1 | one version (the oldest available), 1 December 2014 |
| `520-010-schutzplatzersatzverordnung-spev/` | Verordnung über die Schutzplatzersatzbeiträge (GS 520.010) | 2 | oldest version available, then each consolidated version: 1 December 2014 to 1 January 2020 |
| `520-020/` | Verordnung über die Schutzdienstpflichtverlängerung (GS 520.020) | 1 | as enacted, 1 January 2021 |
| `530-010/` | Verordnung über die wirtschaftliche Landesversorgung (GS 530.010) | 1 | one version (the oldest available), 1 December 2014 |
| `550-010-polv/` | Verordnung zum Polizeigesetz (GS 550.010) | 1 | one version (the oldest available), 23 October 2006 |
| `550-720/` | Verordnung über Massnahmen gegen Gewalt anlässlich von Sportveranstaltungen (GS 550.720) | 1 | as enacted, 1 January 2013 |
| `560-110-huv/` | Verordnung zum Hundegesetz (GS 560.110) | 3 | oldest version available, then each consolidated version: 12 September 2006 to 1 January 2025 |
| `600-010/` | Verordnung über das fakultative Finanzreferendum (GS 600.010) | 1 | as enacted, 20 October 2014 |
| `613-010-fav/` | Finanzausgleichsverordnung (GS 613.010) | 1 | one version (the oldest available), 23 October 2017 |
| `614-010-vfg/` | Verordnung über die Finanzprüfung und die Geschäftsüberwachung (GS 614.010) | 1 | one version (the oldest available), 31 March 2014 |
| `640-010-stv/` | Steuerverordnung (GS 640.010) | 5 | oldest version available, then each consolidated version: 23 October 2017 to 1 June 2024 |
| `658-010-v-dbg/` | Verordnung zum Bundesgesetz über die direkte Bundessteuer (GS 658.010) | 1 | as enacted, 31 March 2014 |
| `660-010-ev-wpeg/` | Einführungsverordnung zum Bundesgesetz über die Wehrpflichtersatzabgabe (GS 660.010) | 1 | one version (the oldest available), 1 July 2017 |
| `685-010-vnu/` | Verordnung über die Nutzung des Untergrundes (GS 685.010) | 1 | as enacted, 1 January 2019 |
| `700-010-bauv/` | Verordnung zum Baugesetz (GS 700.010) | 3 | oldest version available, then each consolidated version: 23 October 2017 to 1 April 2026 |
| `702-010-ev-zwg/` | Einführungsverordnung zum Bundesgesetz über Zweitwohnungen (GS 702.010) | 2 | as enacted, then each consolidated version: 20 June 2016 to 1 November 2021 |
| `721-010-wbauv/` | Wasserbauverordnung (GS 721.010) | 1 | one version (the oldest available), 22 November 2004 |
| `725-010-strv/` | Strassenverordnung (GS 725.010) | 1 | one version (the oldest available), 1 January 2013 |
| `725-020/` | Verordnung über Beiträge an die Sanierung bestehender Bahnübergänge (GS 725.020) | 1 | as enacted, 26 June 2006 |
| `725-310-veg-fwg/` | Verordnung zum Einführungsgesetz zum Bundesgesetz über Fuss- und Wanderwege (GS 725.310) | 1 | one version (the oldest available), 1 January 2011 |
| `726-110-vegob/` | Verordnung zum Einführungsgesetz über das öffentliche Beschaffungswesen (GS 726.110) | 1 | as enacted, 1 November 2022 |
| `730-010-enerv/` | Energieverordnung (GS 730.010) | 2 | oldest version available, then each consolidated version: 11 March 2014 to 1 April 2020 |
| `741-010-veg-svg/` | Verordnung zum Einführungsgesetz zum Strassenverkehrsgesetz (GS 741.010) | 2 | oldest version available, then each consolidated version: 1 December 2014 to 20 June 2022 |
| `746-010-ev-rlg/` | Einführungsverordnung zum eidgenössischen Rohrleitungsgesetz (GS 746.010) | 1 | as enacted, 6 December 2010 |
| `748-010/` | Verordnung zur Bundesgesetzgebung über die Luftfahrt (GS 748.010) | 1 | one version (the oldest available), 1 December 2014 |
| `800-010-v-gesg/` | Verordnung zum Gesundheitsgesetz (GS 800.010) | 2 | oldest version available, then each consolidated version: 1 June 2018 to 1 January 2024 |
| `810-010-vgz/` | Verordnung über das Gesundheitszentrum Appenzell (GS 810.010) | 2 | oldest version available, then each consolidated version: 1 January 2017 to 1 January 2019 |
| `810-014/` | Arbeitszeitreglement (GS 810.014) | 2 | as enacted, then each consolidated version: 1 January 2021 to 1 July 2024 |
| `814-010-veg-usg/` | Verordnung zum Einführungsgesetz zum Bundesgesetz über den Umweltschutz (GS 814.010) | 2 | oldest version available, then each consolidated version: 1 January 2011 to 1 February 2022 |
| `814-310-veg-gschg/` | Verordnung zum Einführungsgesetz zum Bundesgesetz über den Schutz der Gewässer (GS 814.310) | 1 | one version (the oldest available), 1 January 2013 |
| `814-710/` | Einführungsverordnung zur Bundesgesetzgebung über den Schutz vor Gefährdungen durch nichtionisierende Strahlung und Schall (GS 814.710) | 1 | as enacted, 24 October 2022 |
| `817-010-ev-lmg/` | Einführungsverordnung zum Lebensmittelgesetz (GS 817.010) | 2 | oldest version available, then each consolidated version: 1 December 2014 to 1 January 2024 |
| `818-210/` | Einführungsverordnung zur Bundesgesetzgebung über Tabakprodukte und elektronische Zigaretten (GS 818.210) | 1 | as enacted, 1 July 2026 |
| `818-410/` | Verordnung über das Bestattungswesen (GS 818.410) | 1 | one version (the oldest available), 16 February 2004 |
| `822-010/` | Vollziehungsverordnung zum Arbeitsgesetz (GS 822.010) | 1 | one version (the oldest available), 1 December 2014 |
| `822-020/` | Verordnung zum Bundesgesetz über die Heimarbeit (GS 822.020) | 1 | as enacted, 22 June 2015 |
| `822-210/` | Verordnung über die Öffnung von Verkaufsgeschäften an öffentlichen Ruhetagen (GS 822.210) | 1 | one version (the oldest available), 30 March 2015 |
| `823-210/` | Verordnung über die Errichtung von Einigungsstellen (GS 823.210) | 1 | one version (the oldest available), 1 December 2014 |
| `831-010/` | Verordnung zum Bundesgesetz über die Alters- und Hinterlassenenversicherung (GS 831.010) | 2 | oldest version available, then each consolidated version: 31 October 2005 to 1 July 2024 |
| `831-020/` | Verordnung zum Bundesgesetz über die Invalidenversicherung (GS 831.020) | 1 | one version (the oldest available), 1 December 2014 |
| `832-010-vkvg/` | Verordnung zum Bundesgesetz über die Krankenversicherung (GS 832.010) | 1 | one version (the oldest available), 31 October 2005 |
| `836-010-fzv/` | Verordnung über die Familienzulagen (GS 836.010) | 2 | as enacted, then each consolidated version: 1 January 2009 to 1 January 2020 |
| `844-010-wsv/` | Verordnung über die Unterstützung von Wohnbausanierungen (GS 844.010) | 1 | as enacted, 15 June 2009 |
| `845-010/` | Verordnung über Wohnbau- und Eigentumsförderung (GS 845.010) | 1 | one version (the oldest available), 31 October 2005 |
| `850-010-shiv/` | Verordnung über die öffentliche Sozialhilfe (GS 850.010) | 1 | one version (the oldest available), 24 June 2013 |
| `850-350-ibv/` | Verordnung über die Inkassohilfe und Bevorschussung von Unterhaltsbeiträgen (GS 850.350) | 1 | one version (the oldest available), 1 January 2007 |
| `900-010-wirtschaftsforderungsverordnung-wifov/` | Verordnung über die Förderung der Wirtschaft (GS 900.010) | 1 | as enacted, 24 October 2016 |
| `900-020-nrp-verordnung/` | Verordnung über Regionalpolitik (GS 900.020) | 1 | as enacted, 24 October 2016 |
| `910-210/` | Verordnung über Qualität und Vernetzung von ökologischen Ausgleichsflächen in der Landwirtschaft (GS 910.210) | 1 | one version (the oldest available), 1 December 2014 |
| `913-010-vsv/` | Verordnung über Strukturverbesserungen und soziale Begleitmassnahmen in der Landwirtschaft (GS 913.010) | 1 | one version (the oldest available), 1 December 2014 |
| `913-020-beitragsverordnung-unterhalt-bvu/` | Verordnung über Beiträge an den Unterhalt von Strassen und Seilbahnen (GS 913.020) | 2 | oldest version available, then each consolidated version: 1 December 2014 to 1 January 2021 |
| `916-130/` | Verordnung über die Bekämpfung gefährlicher Pflanzenkrankheiten (GS 916.130) | 1 | one version (the oldest available), 1 December 2014 |
| `916-310/` | Verordnung über die Viehzucht, den Viehabsatz und die Unterstützung von Viehversicherungen (GS 916.310) | 1 | one version (the oldest available), 31 October 2005 |
| `916-350-qmv/` | Verordnung über die Qualitätssicherung, die Qualitätskontrolle und die Unterstützung des Absatzes von Milch und Milchprodukten (GS 916.350) | 1 | one version (the oldest available), 1 December 2014 |
| `916-420-tgv/` | Tiergesundheitsverordnung (GS 916.420) | 1 | as enacted, 1 January 2025 |
| `916-510-alpverordnung/` | Verordnung zum Alpgesetz (GS 916.510) | 1 | one version (the oldest available), 1 December 2014 |
| `916-520-alpbuchlein/` | Verordnung über die Gemeinen Alpen (GS 916.520) | 1 | one version (the oldest available), 1 January 2007 |
| `916-610-weinv/` | Weinverordnung (GS 916.610) | 1 | as enacted, 1 August 2022 |
| `921-010-vegwag/` | Verordnung zum Einführungsgesetz zum Bundesgesetz über den Wald (GS 921.010) | 2 | oldest version available, then each consolidated version: 31 October 2005 to 1 January 2020 |
| `922-010-jav/` | Verordnung zum Jagdgesetz (GS 922.010) | 4 | oldest version available, then each consolidated version: 1 February 2016 to 1 January 2025 |
| `922-012-wrv/` | Wildruheverordnung (GS 922.012) | 1 | as enacted, 1 July 2025 |
| `923-010-fischv/` | Fischereiverordnung (GS 923.010) | 1 | one version (the oldest available), 1 March 2014 |
| `930-010-hgpv/` | Verordnung zum Gesetz über die Handels- und Gewerbepolizei (GS 930.010) | 1 | one version (the oldest available), 23 October 2006 |
| `935-110-tfv/` | Tourismusförderungsverordnung (GS 935.110) | 2 | oldest version available, then each consolidated version: 1 January 2017 to 1 January 2020 |
| `935-210/` | Verordnung über das Bergführerwesen (GS 935.210) | 1 | one version (the oldest available), 31 October 2005 |
| `935-310-gastgewerbeverordnung-gav/` | Verordnung über das Gastgewerbe und den Handel mit alkoholischen Getränken (GS 935.310) | 1 | one version (the oldest available), 14 June 2010 |
| `935-610/` | Campingverordnung (GS 935.610) | 1 | one version (the oldest available), 1 January 2013 |
| `941-210/` | Verordnung über das Eichwesen (GS 941.210) | 2 | oldest version available, then each consolidated version: 20 March 2007 to 1 January 2020 |
| `941-410-ev-sprstg/` | Einführungsverordnung zum Bundesgesetz über explosionsgefährliche Stoffe (GS 941.410) | 1 | one version (the oldest available), 23 October 2006 |
| `942-010/` | Verordnung über die Bekanntgabe von Preisen (GS 942.010) | 2 | oldest version available, then each consolidated version: 1 December 2014 to 1 January 2021 |
| `944-010-ev-kkg/` | Einführungsverordnung zum Bundesgesetz über den Konsumkredit (GS 944.010) | 1 | one version (the oldest available), 23 October 2006 |
| `963-110-feuerschutzverordnung-fsv/` | Verordnung zum Gesetz über den Feuerschutz (GS 963.110) | 1 | one version (the oldest available), 1 January 2013 |

## Source

The GS (systematic collection) of the canton, published by the canton at <https://ai.clex.ch/>. For each act it gives every consolidated version it holds, with the day each version took effect, and a change table listing each amendment: its decision date, the day it took effect, the provision it touched and its entry in the chronological collection (cGS). Annexes the collection publishes only as separate PDF files are not included.

## Dates

- Each commit is dated at **noon, Europe/Zurich, on the day the version took effect**, as the collection gives it ("in Kraft seit / von"). The decision date of each amending act is the `Enacted:` trailer.
- An act's first commit is its oldest version in the collection. It is credited to the act as enacted only when the change table shows no amendment in force before it; otherwise it is the "oldest version available", naming the earlier amendments.
- Versions that take effect after the retrieval day are on the `zukunft` branch, never merged into `main`.
- `--before="YYYY-MM-DD"` alone uses your clock's time of day; use `T23:59:59Z` or `tools/on.py`.

## Files

`<act>/art-005.md` is Art. 5 (or § 5), `art-005a.md` Art. 5a; `ingress.md` holds the title, date and preamble; `gliederung.md` the section headings; `schluss.md` the closing formula and signatures. One paragraph or list item per line. Amendment markers (`*`), footnote numbers and the "Stand" date are left out.

## How it is checked

- Every version of every act is read back from git on the day it took effect and on the day before (`tools/check_repo.py`); both must match `corpus.json`.
- The letters and digits of every version equal those of the canton's own text of that version, and every article's text appears in it in order.
- Health checks: no merge commits, commit dates never go backwards, nothing dated in the future, and every commit's trailers parse.

## What "author" means

The author of a commit is the amending act, named by its entry in the chronological collection (cGS), with an e-mail address that cannot exist (`<act key>@ai.clex.ch.invalid`). Where one version holds changes by several amending acts and the change table does not say which provision each one touched, the commit names them all. The committer is always Lexifina.

## Limits

This is not an official publication. The binding text is the one the canton publishes as binding (its chronological collection, or its systematic collection where cantonal law makes that binding). The history starts with the oldest consolidated version the collection holds for each act, which for many acts is later than the act's enactment. Only the acts listed above are included.
