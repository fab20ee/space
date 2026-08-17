---
title: "Ostsilloskoop Micsig TO3004"
seoDescription: "300 MHz neljakanaliline tahvel-ostsilloskoop Tallinna hackspace'is. Silu manussüsteeme, siine ja toiteallikaid korraliku seadmega."
specs:
  - { label: "Ribalaius",   value: "300 MHz" }
  - { label: "Kanalid",     value: "4" }
  - { label: "Vorm",        value: "tahvel, puuteekraan, akutoide" }
  - { label: "Liidesed",    value: "USB, LAN" }
---

<!-- TODO: kontrolli päris seadme järgi — diskreetimissagedus, mälu sügavus, millised sondid ja
     tarvikud on olemas, kas jadasiinide dekodeerimise litsents on aktiveeritud. -->

Ostsilloskoop näitab, mida signaal tegelikult ajas teeb, mitte seda, mida andmelehel lubatakse.
300 MHz ribalaius ja neli kanalit katavad enamiku manussüsteemide tööst: taktid, resetid, PWM,
lülitustoiteallikad ja jadasiinid kõrvuti samal ajaskaalal.

Tahvelformaat on praktikas oluline — seade töötab akuga ja seda saab kaasa võtta sellele pingile
või masina juurde, mida parajasti silud.

## Milleks sobib

- Välja selgitada, miks mikrokontroller resetib või siin lõpetab vastamise
- Mõõta tõusuaegu, värinat, pulsatsiooni ja müra
- Võrrelda nelja signaali korraga — näiteks takt, chip select ja mõlemad andmeliinid
- Kontrollida lülitustoiteallikaid koormuse all
- Püüda harvu tõrkeid päästiku abil, mitte ekraani jõllitades

## Ohutus

- Maanda sond enne skeemi puudutamist korralikult; hõljuv maandus muudab mõõtmised väljamõeldiseks
  ja võib seadme rikkuda.
- Ära kunagi ühenda sondi maandust pingestatud võrgujuhiga. Võrgupingega töö vajab
  eraldustrafot või diferentsiaalsondi — küsi enne alustamist.
- Järgi sondi pingetaluvust, arvestades ka jaguri seadet (×1 ja ×10 erinevad).
- Ära ava korpust. Kui seadmega on midagi valesti, teata sellest.

## Kuidas kasutada

1. Lülita sisse, kontrolli akut ja sea sondi jagur ekraanil oleva seadega samaks.
2. Kompenseeri sond kalibreerimisväljundil enne täpseid mõõtmisi.
3. Ühenda maandusklamber võimalikult mõõtmispunkti lähedale.
4. Sea ajaskaala ja vertikaalne skaala umbkaudu paika; kasuta auto-set'i vaid lähtepunktina.
5. Kasuta päästikut teadlikult — serva perioodilistele signaalidele, pulsilaiust või jadasiini
   tõrgete püüdmiseks.
6. Lõpetades salvesta ekraanipildid USB-pulgale, puhasta sondid ja pane kõik tagasi.

## Ligipääs

Seade asub hackspace'i ruumis, seega on vaja paketti, mis sisaldab hackspace'i ligipääsu.
Seade jääb kohapeale — koju kaasa võtta ei saa.
