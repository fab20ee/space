---
title: "Voolutarbe mõõtja Nordic Power Profiler Kit II"
seoDescription: "Nordic PPK2 Tallinna hackspace'is: mõõdab voolu sadadest nanoampritest ühe amprini, 100 000 näidet sekundis. Patareitoitel seadmete jaoks."
specs:
  - { label: "Voolu vahemik", value: "200 nA kuni 1 A, lahutus alates 100 nA" }
  - { label: "Näidete sagedus", value: "100 000 näidet sekundis" }
  - { label: "Režiimid",     value: "ampermeeter (väline toide) ja mõõtev toiteallikas" }
  - { label: "Pinge",        value: "0,8 – 5 V allikarežiimis, kuni 1 A" }
  - { label: "Loogikasisendid", value: "8 digitaalsisendit — lihtne loogikaanalüsaator" }
  - { label: "Ühendus",      value: "USB arvutiga" }
  - { label: "Tarkvara",     value: "nRF Connect for Desktop, Power Profiler rakendus" }
---

Seade ühe küsimuse jaoks: kui palju sinu seade tegelikult tarbib ja millal?

Patareitoitel seadme puhul ongi see see küsimus. Andur, mis ärkab kord minutis, elab patarei pealt
aastaid — kui ta une ajal tarbib mikroampreid. Kui ta une ajal tarbib pool milliamprit, sest kuskil
jäi sisse mõni pull-up-takisti või LED, siis jätkub patareist kuuks. Vahet näeb ainult seadmega, mis
oskab ühes salvestuses mõõta nii mikroampreid kui ka sadu milliampreid.

PPK2 oskab: 200 nA kuni 1 A, sada tuhat näidet sekundis. Kahe millisekundi pikkuse saatepurske
näitab ta purskena, mitte keskmisena.

## Kaks režiimi

- **Ampermeeter.** Seade töötab oma toite pealt, PPK2 käib toitega jadamisi ja ainult mõõdab.
- **Mõõtev toiteallikas.** PPK2 annab ise 0,8–5 V ja mõõdab samal ajal, kui palju võetakse. Mugavam
  siis, kui tahad näha käitumist eri toitepingetel: kui palju plaat sööb 3,6 V juures ja kui palju
  2,2 V juures, kui patarei on peaaegu tühi.

Lisaks kaheksa digitaalsisendit. Need kinnitatakse oma plaadi jalgade külge ja siis on ühel graafikul
näha, mis vooluhüppe hetkel toimus: siin tõstis püsivara jala üles, siin lülitus sisse raadio, siin
on 40 mA tipp.

## Milleks see sobib

- Mõõta unevoolu ja aru saada, kas seade peab lubatud eluea vastu
- Püüda kinni see, mis ei lase seadmel magama jääda
- Arvutada ühe töötsükli tegelik kulu ja teisendada see konkreetse patarei pealt kuudeks
- Võrrelda kahte püsivara versiooni tarbimise, mitte tunde järgi
- Näha sisselülitamise käivitusvoolu

## Kuidas kasutada

1. Paigalda arvutisse **nRF Connect for Desktop** ja selle sees **Power Profiler** rakendus.
2. Ühenda PPK2 USB kaudu.
3. Vali režiim: ampermeeter, kui plaadil on oma toide, või allikas, kui toidab PPK2 ise.
4. Ühenda plaadiga komplektis olevate juhtmetega: ampermeetri režiimis käib seade toitega
   **jadamisi**, mitte rööbiti.
5. Kui tahad sündmuste märke, kinnita loogikasisendid huvipakkuvate jalgade külge.
6. Käivita salvestus, tee seadmel oma stsenaarium läbi, peata ja loe graafikut.

## Millele tähelepanu pöörata

- Ampermeetri režiimis on seade toiteahelaga jadamisi. Juhtmete äravahetamine tähendab vale asja
  mõõtmist.
- Piir on 1 A. Mootori, võimsa raadio või akulaadijaga seade siia ei sobi.
- Kõige huvitavamad arvud ei ole keskmine vool, vaid unevool ja tippude pikkus. Keskmise annab ka
  multimeeter ja see valetab tavaliselt meeldivas suunas.

## Rentimine

Seadme saab koju kaasa: vähese tarbimisega püsivara kirjutatakse seal, kus mugav on. Juhtmed ja
jõhvik käivad kaasa. Päevahind ja tähtaeg on selle lehe rendiplokis.

## Ligipääs

Seade on hackspace'i ruumis riiulil konteineris, seega on vaja hackspace'i ligipääsuga paketti.
Instruktaaži ei ole vaja.
