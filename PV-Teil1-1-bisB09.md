pn

[index]
-------

tc: (alle)

vn: aict01

qt: Mehrfachauswahl

hl:

in:

q:

!!Herzlich willkommen zur Promovierenden- und Promoviertenbefragung „Nacaps“!!!

Je nach persönlicher Lebenssituation wird die Befragung etwa 25 bis 35 Minuten
dauern. Die Befragung ist für Smartphones geeignet, aber an einem größeren
Bildschirm bequemer und schneller auszufüllen. Sie haben jederzeit die
Möglichkeit, die Befragung zu unterbrechen und zu einem späteren Zeitpunkt
fortzuführen. Wenn Sie den Fragebogen bis zum Ende ausgefüllt haben, haben Sie
die Gelegenheit, an der Verlosung der in der Einladungs-E-Mail genannten Preise
teilzunehmen.

Für Ihre Teilnahme danken wir Ihnen bereits an dieser Stelle ganz herzlich!

Dr. Kolja Briedis, Dr. Bernd Martens und Dr. Antje Wegner

Projektleitung Nacaps

!!Hinweise zum Datenschutz!!

Ihre Teilnahme ist selbstverständlich freiwillig. Ihre Angaben werden
ausschließlich für Forschungszwecke genutzt. Sämtliche Nacaps-Daten werden nur
in anonymisierter Form publiziert und anderen Wissenschaftler(inne)n nur
anonymisiert zur Verfügung gestellt. Ihre Kontaktdaten werden getrennt von den
Befragungsdaten gespeichert und lediglich für eine erneute Kontaktaufnahme
verwendet. Keinesfalls werden Ihre Kontaktdaten an Dritte weitergegeben.

ao: 1 : : Ich habe die
\#\#URL:[Datenschutzbestimmungen](http://www.nacaps.de/datenschutz/Datenschutz.pdf)\#\#
gelesen und bin damit einverstanden.

!!Kontakt!!

Bei !!Fragen zum Datenschutz!! wenden Sie sich bitte an den
Datenschutzbeauftragten des DZHW, Herrn Martin Fuchs: Tel.: +49 511 450670-491;
E-Mail: \#\#URL:fuchs\@dzhw.eu\#\#. Weitere Informationen zum Datenschutz am
DZHW finden Sie \#\#URL:[hier](https://www.dzhw.eu/gmbh/datenschutz)\#\#.

Bei allen !!anderen Fragen und Anmerkungen!! stehen wir Ihnen gerne zur
Verfügung:

Telefonisch unter +49 30 206 417 746 oder +49 511 450 670 106 sowie per E-Mail:
\#\#URL:nacaps\@dzhw.eu\#\#

mv:

ka:

vc: SHOW fv IF aict01 = FALSE

av:

kh:

fv: (flag_index): Bitte beachten Sie, dass ohne Zustimmung zu den
Datenschutzbestimmungen eine Teilnahme an der Nacaps-Befragung leider nicht
möglich ist.

hv:

fo:

tr:

GOTO A01 IF aict01 = TRUE

GOTO cancel1 IF aict01 = FALSE AND flag_index = TRUE

hi: Hinweistext (fv) bitte in rot

pn

[A01]
-----

tc: (alle)

vn: adbi01

qt: Einfachauswahl mit vertikalen ao

hl:

q: Von Ihrer Hochschule haben wir die Information erhalten, dass Sie Anfang
Dezember 2018 offiziell als Doktorand(in) registriert waren. In der Zwischenzeit
kann sich daran etwas geändert haben.

Bitte geben Sie an, was aktuell auf Sie zutrifft.

is: Ihr Promotionsverfahren gilt als abgeschlossen, wenn Sie die letzte Prüfung
(in der Regel: Disputation) erfolgreich abgelegt haben.

it:

ao1: 1 : : Ich promoviere.

ao2: 2 : : Ich habe das Promotionsverfahren abgeschlossen.

ao3: 3 : : Ich habe mein Promotionsvorhaben unterbrochen.

ao4: 4 : : Ich habe mein Promotionsvorhaben abgebrochen.

mv:

ka:

vc:

av:

kh:

fv: (flag_A01): Für den weiteren Verlauf der Befragung ist diese Frage wichtig.
Ohne eine Angabe würden Sie Fragen erhalten, die nicht auf Ihre Situation
zutreffen. Beantworten Sie deshalb bitte diese Frage, um fortfahren zu können.
(IF adbi01 = SYSMISS)

hv:

fo: Antwortoptionen (Zebramuster)

tr:

GOTO A02 IF adbi01 = 3

GOTO A03 IF adbi01 = 4

GOTO A05 IF adbi01 = 1

GOTO A06 IF adbi01 = 2

GOTO cancel2 IF adbi01 = SYSMISS AND flag_A01 = TRUE

hi: Bitte hier Icon 1 für Modul A einfügen (oben rechts) und durchgängig
einblenden bis das Modul B beginnt.

Hinweistext (fv) bitte in rot

pn

[A02]
-----

tc: IF adbi01 = 3

(wenn A01 „Promotionsstatus“= 3 „unterbrochen“)

vn: adid01

qt: offene Frage (string)

hl:

in:

q: Aus welchen Gründen haben Sie das Promotionsvorhaben unterbrochen?

is:

it:

ao: [string] 8 cm; 4 Zeilen

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO A04

hi: großes Textfeld

pn

[A03]
-----

tc: IF adbi01 = 4

(wenn A01 „Promotionsstatus“= 4 „abgebrochen“)

vn: adid02

qt: offene Frage (string)

hl:

in:

q: Aus welchen Gründen haben Sie das Promotionsvorhaben abgebrochen?

is:

it:

ao: [string] 8 cm; 4 Zeilen

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO A06

hi: großes Textfeld

pn

[A04]
-----

tc: IF adbi01 = 3

(wenn A01 „Promotionsstatus“ = 3 „unterbrochen“)

vn: adid03

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Handelt es sich um eine offiziell der Hochschule gemeldete Unterbrechung?

is:

it:

ao1: 1 : : Ja

ao2: 2 : : Nein

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: Antwortoptionen (Zebramuster)

tr:

GOTO A05

hi:

pn

[A05]
-----

tc: IF adbi01 = 1

(wenn A01 „Promotionsstatus“ = 1 „promoviere“)

vn:
adtc01(adtc01a/adtc01b/adtc01c/adtc01d/adtc01e/adtc01f/adtc01g/adtc01h/adtc01i)

qt: Matrix mit horizontaler Einfachauswahl

hl:

in:

q: Warum haben Sie die Promotion begonnen?

is:

it1: (adtc01a): Weil mich die Fragestellung interessiert

it2: (adtc01b): Weil ich zum wissenschaftlichen Fortschritt beitragen möchte

it3: (adtc01c): Weil es in meinem Fach üblich ist

it4: (adtc01d): Weil mein persönliches Umfeld es erwartet

it5: (adtc01e): Weil sich nichts Anderes ergeben hat

it6: (adtc01f): Weil ich dauerhaft wissenschaftlich arbeiten möchte

it7: (adtc01g): Weil ich zur Lösung dringender gesellschaftlicher Probleme
beitragen möchte

it8: (adtc01h): Weil ich mein Ansehen steigern möchte

it9: (adtc01i): Weil ich meine Berufschancen auf dem außerakademischen
Arbeitsmarkt verbessern möchte

ao1: 1 : 1 : trifft gar nicht zu

ao2: 2 : 2 :

ao3: 3 : 3 :

ao4: 4 : 4 :

ao5: 5 : 5 : trifft völlig zu

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: Items (Zebramuster)

tr:

GOTO A06

hi:

pn

[A06]
-----

tc: (alle)

vn: adbi02a/adbi02b

qt: Einfachauswahlmatrix mit drop-down Menü

hl:

in:

q: Wann haben Sie mit der inhaltlichen Arbeit an Ihrer Promotion begonnen?

is: Beziehen Sie hierbei bitte auch die Vorbereitungs- und Orientierungsphase
mit ein (z. B. Erstellung des Exposés, Literaturrecherche, Laborversuche usw.).

it1: (adbi02a): Monat:

it2: (adbi02b): Jahr:

ao1: (adbi02a): Januar, Februar, März, April, Mai, Juni, Juli, August,
September, Oktober, November, Dezember

ao2: (adbi02b): 2019, 2018, 2017, 2016, 2015, 2014, 2013, 2012, 2011, 2010,
2009, 2008, 2007, 2006, 2005, 2004, 2003, 2002, 2001, 2000, vor 2000

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO A07 IF adbi02a = SYSMISS AND adbi02b \<\> SYSMISS

GOTO A08 IF adbi02a \<\> SYSMISS OR adbi02b = SYSMISS

hi:

pn

[A07]
-----

tc: IF adbi02a = SYSMISS AND adbi02b \<\> SYSMISS

(wenn bei A06 („wann mit Promotion begonnen“) ein Jahr, aber kein Monat
angegeben wurde)

vn: adbi03

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q1: Können Sie sich noch erinnern, in welchem Quartal Sie mit den Arbeiten
begonnen haben?

q2: Können Sie sich noch erinnern, in welchem Quartal Sie mit den Arbeiten
begonnen hatten?

is:

it:

ao1: 1 : : 1. Quartal

ao2: 2 : : 2. Quartal

ao3: 3 : : 3. Quartal

ao4: 4 : : 4. Quartal

mv:

ka:

vc:

SHOW q1 IF adbi01 = 1 OR adbi01 = 3

SHOW q2 IF adbi01 = 2 OR adbi01 = 4

av:

kh:

fv:

hv:

fo: Antwortoptionen (Zebramuster)

tr:

GOTO A08

hi:

pn

[A08]
-----

tc: (alle)

vn: adbi04a/adbi04b/adbi04c

qt: Einfachauswahlmatrix mit drop-down Menü und Mehrfachauswahl

hl:

in:

q: Wann wurden Sie von der Hochschule zur Promotion zugelassen?

is: D. h.: Seit wann haben Sie eine schriftliche Bestätigung über die Annahme
Ihres Promotionsvorhabens von Ihrer Hochschule?

it1: (adbi04a): Monat:

it2: (adbi04b): Jahr:

ao1: (adbi04a): Januar, Februar, März, April, Mai, Juni, Juli, August,
September, Oktober, November, Dezember

ao2: (adbi04b): 2019, 2018, 2017, 2016, 2015, 2014, 2013, 2012, 2011, 2010,
2009, 2008, 2007, 2006, 2005, 2004, 2003, 2002, 2001, 2000, vor 2000

it3: (adbi04c): Ich wurde noch nicht zugelassen./Ich habe noch keinen
Zulassungsantrag gestellt.

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: item 3 absetzen

tr:

GOTO A09 IF adbi04a = SYSMISS AND adbi04b \<\> SYSMISS

GOTO A10 IF ((adbi04a \<\> SYSMISS OR adbi04b = SYSMISS) AND (adbi01 = 2))

GOTO A11 IF ((adbi04a \<\> SYSMISS OR adbi04b = SYSMISS) AND (adbi01 = 4))

GOTO A14 IF ((adbi04a \<\> SYSMISS OR adbi04b = SYSMISS) AND (adbi01 = 1 OR
adbi01 = 3))

hi:

pn

[A09]
-----

tc: IF adbi04a = SYSMISS AND adbi04b \<\> SYSMISS

(wenn bei A08 („wann zur Promotion zugelassen“) ein Jahr, aber kein Monat
angegeben wurde)

vn: adbi05

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Können Sie sich noch erinnern, in welchem Quartal Sie zugelassen wurden?

is:

it:

ao1: 1 : : 1. Quartal

ao2: 2 : : 2. Quartal

ao3: 3 : : 3. Quartal

ao4: 4 : : 4. Quartal

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: Antwortoptionen (Zebramuster)

tr:

GOTO A10 IF adbi01 = 2

GOTO A11 IF adbi01 = 4

GOTO A14 IF adbi01 = 1 OR adbi01 = 3

hi:

pn

[A10]
-----

tc: IF adbi01 = 2

(wenn bei A01 („Promotionsstatus“) = 2 („abgeschlossen“))

vn: adbi06a/adbi06b

qt: Einfachauswahlmatrix mit horizontalem drop-down Menü

hl:

in:

q: Wann haben Sie die Promotion abgeschlossen?

is:

it1: (adbi06a): Monat:

it2: (adbi06b): Jahr:

ao1: (adbi06a): Januar, Februar, März, April, Mai, Juni, Juli, August,
September, Oktober, November, Dezember

ao2: (adbi06b): 2019, 2018, 2017, 2016, 2015, 2014, 2013, 2012, 2011, 2010,
2009, 2008, 2007, 2006, 2005, 2004, 2003, 2002, 2001, 2000, vor 2000

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO A14

hi:

pn

[A11]
-----

tc: IF adbi01 = 4

(wenn A01 („Promotionsstatus“) = 4 („abgebrochen))

vn: adbi07

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Ist Ihre Hochschule darüber informiert, dass Sie Ihre Promotion abgebrochen
haben?

is:

it:

ao1: 1 : : Ja

ao2: 2 : : Nein

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: Antwortoptionen (Zebramuster)

tr:

GOTO A12

hi:

pn

[A12]
-----

tc: IF adbi01 = 4 AND adbi07 = 1

(wenn A01 („Promotionsstatus“) = 4 („abgebrochen) und A11 („Hochschule
informiert“) = 1 („ja“))

vn: adbi08a/adbi08b

qt: Einfachauswahlmatrix mit drop-down Menü

hl:

in:

q: Wann haben Sie die Promotion abgebrochen?

is:

it1: (adbi08a): Monat:

it2: (adbi08b): Jahr:

ao1: (adbi08a): Januar, Februar, März, April, Mai, Juni, Juli, August,
September, Oktober, November, Dezember

ao2: (adbi08b): 2019, 2018, 2017, 2016, 2015, 2014, 2013, 2012, 2011, 2010,
2009, 2008, 2007, 2006, 2005, 2004, 2003, 2002, 2001, 2000, vor 2000

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO A13 IF adbi08a = SYSMISS AND adbi08b \<\> SYSMISS

GOTO A14 IF adbi08a \<\> SYSMISS OR adbi08b = SYSMISS

hi:

pn

[A13]
-----

tc: IF adbi08a = SYSMISS AND adbi09b \<\> SYSMISS

(wenn bei A12 („Promotionsabbruch: Zeitpunkt“) ein Jahr, aber kein Monat
angegeben wurde)

vn: adbi09

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Können Sie sich noch erinnern, in welchem Quartal Sie Ihre Promotion
abgebrochen haben?

is:

ao1: 1 : : 1. Quartal

ao2: 2 : : 2. Quartal

ao3: 3 : : 3. Quartal

ao4: 4 : : 4. Quartal

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: Antwortoptionen (Zebramuster)

tr:

GOTO A14

hi:

pn

[A14]
-----

tc: (alle)

vn: adbi10a/adbi10b

qt: offene Frage (string)

hl:

in:

q1: An welcher Hochschule promovieren Sie?

q2: An welcher Hochschule haben Sie promoviert?

q3: An welcher Hochschule wollten Sie promovieren?

is:

ao1: (adbi09a): 6 cm, Präfix [ao]: Name der Hochschule (z. B. Universität
Erlangen-Nürnberg): [string]

ao2: (adbi09b): 6 cm, Präfix [ao]: Standort der Hochschule (z. B. Nürnberg):
[string]

mv:

ka:

vc:

SHOW q1 IF adbi01 = 1 OR adbi01 = 3

SHOW q2 IF adbi01 = 2

SHOW q3 IF adbi01 = 4

av:

kh:

fv:

hv:

fo: Antwortoptionen (Zebramuster)

tr:

GOTO A15 IF ((adbi01 = 1 OR adbi01 = 3) AND (adbi10a \<\> SYSMISS))

GOTO A16 IF ((adbi01 = 1 OR adbi01 = 3) AND (adbi10a = SYSMISS))

GOTO A20 IF adbi01 = 2 OR adbi01 = 4

hi:

pn

[A15]
-----

tc: IF (adbi01 = 1 OR adbi01 = 3) AND adbi10a \<\> SYSMISS

(wenn A01 („Promotionsstatus“)= 1 („promoviere“) oder 3 („unterbrochen“) und A14
(„Hochschule Promotion“) ausgefüllt)

vn: adtc02(adtc02a/adtc02b/adtc02c/adtc02d/adtc02e/adtc02f/adtc02g/adtc02h)

qt: Mehrfachauswahl mit vertikalen ao und offener ao (string)

hl:

in:

q: Warum haben Sie sich für eine Promotion an dieser Hochschule entschieden?

is: Bitte wählen Sie alles Zutreffende aus.

it:

ao1: (adtc02a): Weil ich gerne an diesem Standort sein wollte

ao2: (adtc02b): Wegen der guten Forschungsbedingungen in meinem Fach

ao3: (adtc02c): Wegen des Betreuers/der Betreuerin

ao4: (adtc02d): Wegen des guten Rufs der Hochschule

ao5: (adtc02e): Weil es dort attraktive Serviceangebote für Promovierende gibt

ao6: (adtc02f): Es hat sich einfach so ergeben. [EK]

ao7: (adtc02g): Sonstiges, und zwar: (adtc02h): [string] 6 cm

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: Antwortoptionen (Zebramuster)

tr:

GOTO A16

hi:

pn

[A16]
-----

tc: IF adbi01 = 1 OR adbi01 = 3

(wenn A01 („Promotionsstatus“) = 1 („promoviere“) oder 3 („unterbrochen“))

vn: adbi11

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Ist an Ihrem Promotionsverfahren eine Hochschule im Ausland beteiligt?

is:

it:

ao1: 1 : : Ja

ao2: 2 : : Nein

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: Antwortoptionen (Zebramuster)

tr:

GOTO A17 IF adbi11 = 1

GOTO A18 IF adbi11 = 2 OR adbi11 = SYSMISS

hi:

pn

[A17]
-----

tc: IF (adbi01 = 1 OR adbi01 = 3) AND adbi11 = 1

(wenn A01 („Promotionsstatus“) = 1 („promoviere“) oder 3 („unterbrochen“) und
A16 („Hochschule im Ausland beteiligt“) = 1 („Ja“))

vn: adbi12

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Handelt es sich dabei um einen gemeinsamen Abschluss der Hochschulen aus dem
In- und Ausland (cotutelle de thèse)?

is:

it:

ao1: 1 : : Ja

ao2: 2 : : Nein

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: Antwortoptionen (Zebramuster)

tr:

GOTO A18

hi:

pn

[A18]
-----

tc: IF adbi01 = 1 OR adbi01 = 3

(wenn A01 („Promotionsstatus“) = 1 („promoviere“) oder 3 („unterbrochen“))

vn: adbi13

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Ist an ihrem Promotionsverfahren eine Fachhochschule bzw. Hochschule für
angewandte Wissenschaften beteiligt?

is:

it:

ao1: 1 : : Ja

ao2: 2 : : Nein

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: Antwortoptionen (Zebramuster)

tr:

GOTO A19 IF adbi13 = 1

GOTO A20 IF adbi13 = 2 OR adbi13 = SYSMISS

hi:

pn

[A19]
-----

tc: IF (adbi01 = 1 OR adbi01 = 3) AND adbi13 = 1

(wenn A01 („Promotionsstatus“) = 1 („promoviere“) oder 3 („unterbrochen“)) und
A18 („Fachhochschule beteiligt“) = 1 („Ja“))

vn: adbi14(adbi14a/adbi14b/adbi14c/adbi14d/adbi14e/adbi14f/adbi14g)

qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q: Welche Aussagen treffen auf Ihr Promotionsverfahren zu?

is: Bitte wählen Sie alles Zutreffende aus.

it:

ao1: (adbi14a): Ich habe/hatte einen Arbeitsvertrag an der
Fachhochschule/Hochschule für angewandte Wissenschaften.

ao2: (adbi14b): Wesentliche Teile der Arbeit finden an der
Fachhochschule/Hochschule für angewandte Wissenschaften statt.

ao3: (adbi14c): Der/Die FH-Professor(in) ist Prüfer(in).

ao4: (adbi14d): Der/Die FH-Professor(in) ist Gutachter(in).

ao5: (adbi14e): Der/Die FH-Professor(in) ist Betreuer(in).

ao6: (adbi14f): Es gibt einen Kooperationsvertrag zwischen der Universität und
der FH.

ao7: (adbi14g): Ich habe eine Betreuungsvereinbarung, die sowohl der/die
Universitäts- als auch der/die FH-Professor(in) unterschrieben hat.

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: Antwortoptionen (Zebramuster)

tr:

GOTO A20

hi:

pn

[A20]
-----

tc: (alle)

vn: adbi15

qt: offene Frage (string)

hl:

in:

q1: In welchem Fach promovieren Sie?

q2: In welchem Fach haben Sie promoviert?

q3: In welchem Fach waren Sie eingeschrieben?

is: Bitte geben Sie eine möglichst genaue Fachbezeichnung an.

it:

ao1: [string] 8 cm, 1 Zeile

mv:

ka:

vc:

SHOW q1 IF adbi01 = 1 OR adbi01 = 3

SHOW q2 IF adbi01 = 2

SHOW q3 IF adbi01 = 4

av:

kh:

fv:

hv:

fo:

tr:

GOTO B01 IF adbi01 = 1 OR adbi01 = 2 OR adbi01 = 3

GOTO B03 IF adbi01 = 4

hi:

pn

[B01]
-----

tc: IF adbi01 = 1 OR adbi01 = 2 OR adbi01 = 3

(wenn A01 („Promotionsstatus“) = 1 („promoviere“), 2 („abgeschlossen“) oder 3
(„unterbrochen“))

vn: adcd01

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q1: Ist Ihre Promotion Teil eines Forschungsprojekts, an dem auch noch andere
Personen arbeiten?

q2: War Ihre Promotion Teil eines Forschungsprojekts, an dem auch noch andere
Personen arbeite(te)n?

is:

it:

ao1: 1 : : Ja

ao2: 2 : : Nein

mv:

ka:

vc:

SHOW q1 IF adbi01 = 1 OR adbi01 = 3

SHOW q2 IF adbi01 = 2

av:

kh:

fv:

hv:

fo: Antwortoptionen (Zebramuster)

tr:

GOTO B02 IF adcd01 = 1

GOTO B03 IF (adbi01 = 1 OR adbi01 = 3) AND (adcd01 = 2 OR adcd01 = SYSMISS)

GOTO B04 IF (adbi01 = 2 AND (adcd01 = 2 OR adcd01 = SYSMISS))

hi: Bitte hier Icon 2 für Modul B einfügen (oben rechts) und durchgängig
einblenden bis das nächste Modul C beginnt.

pn

[B02]
-----

tc: IF (adbi01 = 1 OR adib01 = 2 OR adbi01 = 3) AND adcd01 = 1

(wenn {A01 („Promotionsstatus“) = 1 („promoviere“), 2 („abgeschlossen“) oder 3
(„unterbrochen“))

Und B01 {„Teil eines Forschungsprojekts“) = 1 („Ja“)})

vn: adcd02

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q1: Gibt es in dem Forschungsprojekt – außer Ihnen selbst – noch andere
Promovierende?

q2: Gab es in dem Forschungsprojekt – außer Ihnen selbst – noch andere
Promovierende?

is:

it:

ao1: 1 : : Ja

ao2: 2 : : Nein

mv:

ka:

vc:

SHOW q1 IF adbi01 = 1 OR adbi01 = 3

SHOW q2 IF adbi01 = 2

av:

kh:

fv:

hv:

fo: Antwortoptionen (Zebramuster)

tr:

GOTO B03 IF adbi01 = 1 OR adbi01 = 3

GOTO B04 IF adbi01 = 2

hi:

pn

[B03]
-----

tc: IF adbi01 = 1 OR adbi01 = 3 OR adbi01 = 4

(wenn A01 („Promotionsstatus“) = 1 („promoviere“), 3 („unterbrochen“) oder 4
(„abgebrochen“))

vn: adtc03

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q1: Haben Sie schon ein konkretes Promotionsthema?

q2: Hatten Sie schon ein konkretes Promotionsthema?

is:

it:

ao1: 1 : : Ja

ao2: 2 : : Nein

mv:

ka:

vc:

SHOW q1 IF adbi01 = 1 OR adbi01 = 3

SHOW q2 IF adbi01 = 4

av:

kh:

fv:

hv:

fo: Antwortoptionen (Zebramuster)

tr:

GOTO B04 IF ((adbi01 = 1 OR adbi01 = 3) AND (adtc03 = 1))

GOTO B05 IF ((adbi01 = 1 OR adbi01 = 3) AND (adtc03 = 2 OR adtc03 = SYSMISS))

GOTO B38 IF adbi01 = 4

hi:

pn

[B04]
-----

tc: IF (adbi01 = 1 OR adbi01 = 2 OR adbi01 = 3) AND adtc03 = 1

(wenn {(A01 („Promotionsstatus“) = 1 („promoviere“), 2 („abgeschlossen“) oder 3
(„unterbrochen“)) und („konkretes Promotionsthema“) = („Ja“)})

vn:
adtc04(adtc04a/adtc04b/adtc04c/adtc04d/adtc04e/adtc04f/adtc04g/adtc04h/adtc04i/adtc04j)

qt: Mehrfachauswahl mit vertikalen ao und offener ao (string)

hl:

in:

q1: Wie sind Sie zu Ihrem Promotionsthema gekommen?

is: Bitte wählen Sie alles Zutreffende aus.

it:

ao1a: (adtc04a): Das Thema baut auf Arbeiten meines vorangegangenen Studiums
auf.

ao2a: (adtc04b): Das Thema wurde mir von einer/einem Betreuer(in) vorgeschlagen.

ao3a: (adtc04c): Das Thema schließt an Berufserfahrungen an, die ich außerhalb
der Wissenschaft gemacht habe.

ao4a: (adtc04d): Das Thema wurde in enger Kooperation mit Partnern außerhalb der
Wissenschaft abgestimmt.

ao5a: (adtc04e): Ich habe das Thema selbst entwickelt.

ao6a: (adtc04f): Das Thema war vorgegeben (z. B. im Rahmen eines
Forschungsprojekts).

ao7a: (adtc04g): Der thematische Rahmen war vorgegeben.

ao8a: (adtc04h): Das Thema wurde ausgeschrieben.

ao9a: (adtc04i): Sonstiges, und zwar: (adtc04j): [string] 6 cm

q2: Wie waren Sie zu Ihrem Promotionsthema gekommen?

ao1b: (adtc04a): Das Thema baute auf Arbeiten meines vorangegangenen Studiums
auf.

ao2b: (adtc04b): Das Thema wurde mir von einer/einem Betreuer(in) vorgeschlagen.

ao3b: (adtc04c): Das Thema schloss an Berufserfahrungen an, die ich außerhalb
der Wissenschaft gemacht habe.

ao4b: (adtc04d): Das Thema wurde in enger Kooperation mit Partnern außerhalb der
Wissenschaft abgestimmt.

ao5b: (adtc04e): Ich habe das Thema selbst entwickelt.

ao6b: (adtc04f): Das Thema war vorgegeben (z. B. im Rahmen eines
Forschungsprojekts).

ao7b: (adtc04g): Der thematische Rahmen war vorgegeben.

ao8b: (adtc04h): Das Thema wurde ausgeschrieben.

ao9b: (adtc04i): Sonstiges, und zwar: (adtc04j): [string] 6 cm

mv:

ka:

vc:

SHOW q1 IF adbi01 = 1 OR adbi01 = 3

SHOW ao1a – ao9a IF adbi01 = 1 OR adbi01 = 3

SHOW q2 IF adbi01 = 2

SHOW ao1b – ao9b IF adbi01 = 2

av:

kh:

fv:

hv:

fo: Antwortoptionen (Zebramuster)

tr:

GOTO B05 IF adbi01 = 1 OR adbi01 = 3

GOTO B06 IF adbi01 = 2

hi: Gleiche Variablen werden bei den Antwortoptionen erhoben, nur der Text ist
in verschiedenen Zeitformen

pn

[B05]
-----

tc: IF adbi01 = 1 OR adbi01 = 3

(wenn A01 („Promotionsstatus“) = 1 („promoviere“) oder 3 („unterbrochen“))

vn: adcd03

qt: offene Frage (number)

hl:

in:

q: Wie weit sind Sie mit Ihrer Promotion?

is:

it:

ao1: 3 cm, Präfix [ao] Suffix: Ich habe ca. [number] % bewältigt.

mv:

ka:

vc:

av: number : \<= 3 stellig : 0 TO 100

kh: Bitte geben Sie einen Wert zwischen 0 und 100 an. (IF adcd03 \> 100)

fv:

hv:

fo:

tr:

GOTO B06

hi:

pn

[B06]
-----

tc: IF adbi01 = 1 OR adbi01 = 2 OR adbi01 = 3

(wenn A01 („Promotionsstatus“) = 1 („promoviere“), 2 („abgeschlossen“) oder 3
(„unterbrochen“))

vn: adcd04

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q1: Sind Sie derzeit Mitglied in einem strukturierten Promotionsprogramm (z. B.
Promotionsstudiengang, Promotionsprogramm, Graduiertenschule,
Graduiertenkolleg)?

q2: Waren Sie Mitglied in einem strukturierten Promotionsprogramm (z. B.
Promotionsstudiengang, Promotionsprogramm, Graduiertenschule,
Graduiertenkolleg)?

is:

it:

ao1: 1 : : Ja, als ordentliches Mitglied.

ao2: 2 : : Ja, als assoziiertes Mitglied.

ao3: 3 : : Nein.

mv:

ka:

vc:

SHOW q1 IF adbi01 = 1 OR adbi01 = 3

SHOW q2 IF adbi01 = 2

av:

kh:

fv:

hv:

fo: Antwortoptionen (Zebramuster)

tr:

GOTO B07 IF adcd04 = 1 OR adcd04 = 2

GOTO B10 IF ((adbi01 = 1 OR adbi01 = 3) AND (adcd04 = 3 OR adcd04 = SYSMISS))

GOTO B18 IF ((adbi01 = 2) AND (adcd04 = 3 OR adcd04 = SYSMISS))

hi:

pn

[B07]
-----

tc: IF (adbi01 = 1 OR adbi01 = 2 OR adbi01 = 3) AND (adcd04 = 1 OR adcd04 = 2)

(wenn A01 („Promotionsstatus“) = 1 („promoviere“), 2 („abgeschlossen“) oder 3
(„unterbrochen“)) und

B06 („Mitglied Promotionsprogramm“) = 1 („ordentliches Mitglied“) oder 2
(„assoziiertes Mitglied“))

vn:
adcd05(adcd05a/adcd05b/adcd05c/adcd05d/adcd05e/adcd05f/adcd05g/adcd05h/adcd05i/adcd05j/adcd05k)

qt: Mehrfachauswahl mit vertikalen ao und offener ao (string)

hl:

in:

q1: In welcher Art von Promotionsprogramm(en) sind Sie Mitglied?

q2: In welcher Art von Promotionsprogramm(en) waren Sie Mitglied?

is: Bitte wählen Sie alles Zutreffende aus.

it:

ao1: (adcd05a): Graduiertenkolleg (DFG)

ao2: (adcd05b): Integriertes Graduiertenkolleg (innerhalb eines SFB)

ao3: (adcd05c): Graduiertenschule der Exzellenzinitiative (DFG)

ao4: (adcd05d): Promotionsprogramm der Universität ohne Förderung durch die DFG

ao5: (adcd05e): Promotionsprogramm der Universität mit Förderung durch die DFG

ao6: (adcd05f): International Max Planck Research School (IMPRS)

ao7: (adcd05g): Programm der Helmholtz Gemeinschaft

ao8: (adcd05h): Leibniz Graduate School

ao9: (adcd05i): Promotionsstudiengang

ao10: (adcd05j): Sonstiges Programm, und zwar: (adcd05k): [string] 6 cm

mv:

ka:

vc:

SHOW q1 IF adbi01 = 1 OR adbi01 = 3

SHOW q2 IF adbi01 = 2

av:

kh:

fv:

hv:

fo: Antwortoptionen (Zebramuster)

tr: GOTO B08

hi:

pn

[B08]
-----

tc: IF (adbi01 = 1 OR adbi01 = 2 OR adbi01 = 3) AND (adcd04 = 1 OR adcd04 = 2)

(wenn A01 („Promotionsstatus“) = 1 („promoviere“), 2 („abgeschlossen“) oder 3
(„unterbrochen“)) und B06 („Mitglied Promotionsprogramm“) = 1 („ordentliches
Mitglied“) oder 2 („assoziiertes Mitglied“))

vn: adcd06(adcd06a/adcd06b/adcd06c)

qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q: Was trifft für Ihre Mitgliedschaft in dem/den Promotionsprogramm(en) zu?

is: Bitte wählen Sie alles Zutreffende aus.

it:

ao1: (adcd06a): Ich muss an einem verbindlichen Kurs- und
Lehrveranstaltungsprogramm teilnehmen.

ao2: (adcd06b): Ich werde von mehreren Hochschullehrer(inne)n betreut.

ao3: (adcd06c): Ich habe ein wettbewerbliches Auswahlverfahren mit Ausschreibung
durchlaufen.

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: Antwortoptionen (Zebramuster)

tr:

GOTO B09

hi:

pn

[B09]
-----

tc: IF (adbi01 = 1 OR adbi01 = 2 OR adbi01 = 3) AND (adcd04 = 1 OR adcd04 = 2)

(wenn A01 („Promotionsstatus“) = 1 („promoviere“), 2 („abgeschlossen“) oder 3
(„unterbrochen“)) und B06 („Mitglied Promotionsprogramm“) = 1 („ordentliches
Mitglied“) oder 2 („assoziiertes Mitglied“))

vn: adcd07(adcd07a/adcd07b/adcd07c)

qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q: Bekamen Sie im Rahmen des Programms/der Programme ein Stipendium oder eine
Stelle?

is: Bitte wählen Sie alles Zutreffende aus.

it:

ao1: (acdc07a): Ja, ein Stipendium.

ao2: (adcd07b): Ja, eine Stelle.

ao3: (adcd07c): Nein. [EK]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: Antwortoptionen (Zebramuster)

tr:

GOTO B10 IF adbi01 = 1 OR adbi01 = 3

GOTO B18 IF adbi01 = 2

hi:
