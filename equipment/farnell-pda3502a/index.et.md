---
title: "Kahekanaliline toiteplokk Farnell PDA3502A"
seoDescription: "Kahe väljundiga lineaarne laboritoiteplokk Tallinna hackspace'is. Farnell PDA3502A: kaks sõltumatut 0–35 V, 0–2 A kanalit jälgimisrežiimiga sümmeetriliste ±V analoogskeemide jaoks."
specs:
  - { label: "Väljundid",   value: "2 sõltumatut kanalit" }
  - { label: "Kanali kohta", value: "0–35 V, 0–2 A" }
  - { label: "Režiimid",    value: "sõltumatu või master/slave jälgimine" }
  - { label: "Tüüp",        value: "lineaarne, osutinäidikud" }
---

<!-- TODO: kontrolli päris seadme järgi — kalibreerimise seis, kas mõlemad kanalid on
     spetsifikatsiooni piires, klemmide seisukord. -->

Vana kooli lineaarne toiteplokk kahe väljundi ja osutinäidikutega, ja põhjus, miks see ikka laual
seisab, on lihtne: kaks kanalit. Paljud analoogskeemid — operatsioonivõimendid, heliastmed,
mõõtevõimendid — vajavad korraga positiivset ja negatiivset toitesiini. Jälgimisrežiimis järgib teine
kanal esimest, nii et üks nupp annab puhta, sümmeetrilise ±12 V või ±15 V.

Lineaarsena on sellel väga vähe lülitusmüra, mis on oluline, kui vaatad ostsilloskoobil väikeseid
signaale. Näidikutel on kirjas „ainult orienteeruvaks" — kui täpne väärtus loeb, kasuta multimeetrit.

## Milleks see sobib

- Sümmeetriline toide operatsioonivõimendi- ja heliskeemidele
- Kahe eraldi plaadi või plaadi ja selle anduri toitmine eri pingetel
- Madala müraga toide mõõtmisteks, kus impulsstoiteplokk paistaks ostsilloskoobil välja
- Kõik, mis vajab kuni 35 V — rohkem kui teised laual olevad toiteplokid annavad

## Ohutus

- Keera voolunupud enne uue skeemi ühendamist alla ja tõsta ainult nii palju, kui vaja.
- Jälgimisrežiimis on kaks kanalit seespool jadamisi ühendatud — vaata enne esimest ±V toite
  ehitamist juhendi ühendusskeemi.
- Punane on pluss, must on miinus, roheline klemm on maandus. Kaks kanalit tähendab kaks korda
  rohkem võimalusi eksida.
- Seade läheb töös soojaks; hoia õhutusavad vabad.

## Kuidas kasutada

1. Lülita sisse väljalülitatud väljunditega. Vali režiimilülitiga INDEP või TRACK.
2. Sea pinge igal kanalil (või jälgimisrežiimis master-kanalil) ja voolupiir.
3. Ühenda juhtmed, kontrolli polaarsust ja lülita väljund sisse.
4. Kui täpsus loeb, mõõda pinge multimeetriga.
5. Lõpus lülita väljundid välja, ühenda juhtmed lahti ja lülita seade välja.

## Ligipääs

Toiteplokk asub hackspace'i ruumi elektroonikalaual, seega on vaja paketti, mis sisaldab hackspace'i
ligipääsu. Ohutusinstruktaaži pole vaja.
