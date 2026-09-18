---
title: "Aku sisetakistuse tester FNIRSI HRM-10"
seoDescription: "FNIRSI HRM-10 Tallinna hackspace'is: aku sisetakistuse mõõtja nelja juhtme Kelvini klambritega, näitab korraga takistust ja pinget. Millioommeeter taskus."
specs:
  - { label: "Mõõdab",         value: "sisetakistust ja pinget korraga" }
  - { label: "Takistus",       value: "kuni 200 Ω; millioomide piirkonnas eristab millioomi sajandikke" }
  - { label: "Pinge",          value: "kuni 100 V alalispinget" }
  - { label: "Meetod",         value: "nelja juhtmega (Kelvin), juhtmete ja kontaktide takistus jääb välja" }
  - { label: "Mälu",           value: "mõõtmiste ajalugu, kaheksa pinge ja takistuse paari ekraanil, eksport tabelina" }
  - { label: "Ekraan",         value: "värviline TFT" }
  - { label: "Komplektis",     value: "nelja kontaktiga Kelvini klambrid" }
---

Aku mahtuvus ütleb, kui palju on sinna salvestatud. Sisetakistus ütleb, kui kiiresti ta selle
tagasi anda suudab — ja kas element on üldse elus. 18650 võib näidata ausat 4,1 V ja ikkagi koormuse
all väljalülituspiirini vajuda, sest tema sisetakistus on 30 mΩ asemel 300.

HRM-10 mõõdab mõlemat korraga: panid klambrid külge ja näed pinget ning takistust. Millioome
tavalise multimeetriga mõõta ei ole mõtet — tema enda juhtmete takistus on suurem kui see, mida sa
mõõta püüad.

## Miks neli juhet

Klambrid ei ole tavalised, vaid Kelvini klambrid: igal lõual on kaks eraldi kontaktplaati. Üks
juhtmepaar kannab voolu, teine mõõdab pinget otse aku klemmil. Juhtmete, klambrite ja klemmil oleva
oksiidi takistus tulemusse ei jõua. Just seepärast näeb see seade millioomi kümnendikke ja
multimeeter mitte.

## Milleks see sobib

- Kasutatud 18650 ja 21700 elementide praakimine: surnud elemendi sisetakistus on kordades suurem
  kui elusal, isegi kui mõlemal on pinge normaalne
- Elementide sobitamine pakiks: rööbiti ja jadamisi pannakse lähedase takistusega elemendid, muidu
  teeb üks neist kõigi eest tööd ja kuumeneb
- Nikkelriba keevituskohtade kontroll pakis — halb keevitus paistab välja lisamillioomidena
- Kontaktide, pistikute, kaitsmete ja radade kontroll: see on ka lihtsalt millioommeeter
- Pliiaku diagnoosimine ilma seda autost välja võtmata

## Kuidas kasutada

1. Lülita sisse ja veendu, et mõõdad alalispinget. **Vahelduvpinget ei tohi anda mitte mingil
   juhul**, alalispinge piir on 100 V.
2. Pane klambrid nii, et mõlemad plaadid igal lõual puutuksid metalli. Kui üks plaat jääb õhku,
   muutub nelja juhtme meetod vaikselt kahe juhtme omaks ja näit läheb paigast ära.
3. Lase näidul paika loksuda ja loe mõlemad väärtused.
4. Elementide sortimisel mõõda neid ühesugustes tingimustes: sama laetus, sama temperatuur, sama
   koht klemmil. Ainult nii on võrdlus midagi väärt.
5. Vajalikud tulemused salvesta mällu ja ekspordi hiljem tabelina.

## Mida mitte teha

- Ära ühenda seda võrku ega üldse vahelduvpingega.
- Ära mõõda takistust ahelas, kus midagi töötab: seade annab oma voolu.
- Ära ühenda klambritega aku mõlemat klemmi pingerežiimis kokku — see ei ole mõõtmine, vaid lühis
  läbi klambri.

## Rentimine

Selle seadme saab koju kaasa: tavaline põhjus on kasutatud 18650 elementide karp läbi vaadata ja
aru saada, millised neist veel midagi väärt on. Päevahind ja tähtaeg on selle lehe rendiplokis.

## Ligipääs

Seade on hackspace'i ruumis riiulil konteineris, seega on vaja hackspace'i ligipääsuga paketti.
Instruktaaži ei ole vaja.
