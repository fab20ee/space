---
title: "Infrapuna BGA-remondijaam IR6500"
seoDescription: "Infrapuna BGA-remondijaam Tallinna hackspace'is. IR6500 üla- ja alakütteelemendiga reballing'uks ning GPU-de, kiibistike ja muude BGA-kiipide vahetamiseks sülearvuti- ja telefoniplaatidel."
specs:
  - { label: "Tüüp",            value: "infrapuna, üla- ja alaküte" }
  - { label: "Ülaküte",         value: "IR, tume kiirgur, reguleeritav kõrgus" }
  - { label: "Alumine eelsoojendus", value: "IR, kogu plaadi eelsoojendus" }
  - { label: "Juhtimine",       value: "kaks PID-kontrollerit K-tüüpi termopaaridega" }
  - { label: "Plaadihoidik",    value: "reguleeritavad siinid, plaat kuni u 350 × 400 mm" }
---

<!-- TODO: kontrolli päris jaama järgi — kütteelementide võimsused, maksimaalne plaadi suurus,
     millised termopaarid ja šabloonid on laual, kas profiil on häälestatud. -->

Infrapuna-remondijaam on viis vahetada kiipi, millel pole jalgu. BGA-korpused — GPU-d, kiibistikud,
mälu, enamik telefoniprotsessoreid — on joodetud sadade kuulikestega alt, nii et jootekolb nende
juurde ei pääse. IR6500 kuumutab kogu plaati õrnalt alt ja üht kiipi tugevalt ülalt, järgides
temperatuuriprofiili, kuni kuulikesed sulavad ja kiibi saab üles tõsta või see vajub paika.

See on elektroonikalaua kõige nõudlikum tööriist. Vale profiil küpsetab plaadi läbi või jätab pooled
kuulikesed jootmata, seetõttu on enne esimest tööd nõutav ohutusinstruktaaž.

## Milleks see sobib

- BGA-kiipide eemaldamine ja tagasipanek: GPU-d, kiibistikud, mälu, telefonide SoC-id
- Kiibi reballing šablooni ja uute tinakuulikestega
- Kahtlase kiibi ülessulatamine, mille jootekohad on pragunenud
- Plaadi eelsoojendus kuumaõhutööks, et vask kogu kuumust ära ei viiks

## Ohutus

- Mõlemad kütteelemendid töötavad võrgutoitel ja lähevad jootekolvist palju kuumemaks. Plaat,
  hoidiku siinid ja kiip püsivad pärast tsükli lõppu veel minuteid ohtlikult kuumad.
- Ära vaata sisselülitatud ülemisse IR-kiirgurisse.
- Ära jäta töötavat tsüklit kunagi maha. Püsi jaama juures ja jälgi termopaaride näite.
- Lase plaadil hoidikus jahtuda — sulanud kuulikestega plaadi liigutamine rikub töö.
- Ülessulatamisel on räbustiaure palju; kasuta suitsuimurit.

## Kuidas kasutada

1. Eemalda plaadilt akud, plastkatted, kleebised ja kõik, mis sulab. Kata lähedal asuvad
   plastpistikud alumiiniumteibi või metallkatetega.
2. Kinnita plaat siinidesse loodis, sihtkiip ülakütte all. Sea kütteelemendi kõrgus juhendi järgi.
3. Teibi termopaar kiibi kõrvale (mitte peale) ja kontrolli, et see näitab toatemperatuuri.
4. Kanna kiibi ümber räbustit ja vali või sisesta kasutatava tina temperatuuriprofiil — pliivaba
   vajab kõrgemat tippu kui pliiga tina.
5. Käivita tsükkel ja jälgi näite. Kui tipp on saavutatud ja tina on nähtavalt sulanud, tõsta kiip
   vaakumpintsetiga ära või lase sel paika vajuda, kui teed ülessulatamist.
6. Lase kõigel enne plaadi puutumist täielikult jahtuda. Puhasta räbusti maha.

## Ligipääs

Jaam asub hackspace'i ruumis, seega on vaja paketti, mis sisaldab hackspace'i ligipääsu.
**Ohutusinstruktaaž on enne esimest tööd kohustuslik** — see hõlmab kütteelementide seadistust,
termopaari paigutust, profiile ja seda, mida teha, kui plaat hakkab suitsema.
