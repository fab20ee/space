---
title: "RF-tarvikud: üleminekud, kalibreerimiskomplektid, antennid"
seoDescription: "RF-tarvikute konteiner Tallinna hackspace'is: N-, SMA- ja BNC-üleminekud, open/short/load kalibreerimiskomplektid, DC-blokk kuni 6 GHz ning 433 ja 868 MHz antennid."
specs:
  - { label: "Kalibreerimiskomplektid", value: "open / short / load, üks N-type ja üks SMA" }
  - { label: "DC-blokk",     value: "kuni 6 GHz" }
  - { label: "Üleminekud",   value: "N-type, SMA, BNC, klemmid, eri kombinatsioonides" }
  - { label: "Antennid",     value: "SMA vardantennid 433 ja 868 MHz jaoks, teleskoopantenn SMA-ga" }
  - { label: "Demoplaat",    value: "NanoVNA RF Demo Kit — filtrid ja teadaolevate väärtustega testahelad" }
  - { label: "Kaablid",      value: "SMA ja N, eri pikkustes" }
---

Eraldi konteiner kõige sellega, mis käib seadme ja antenni vahele. Ise ta midagi ei mõõda, aga ilma
temata ei tööta töökojas ükski raadioseade:
[tinySA Ultral](/et/seadmed/kaasaskantav-spektrianaluusaator-tinysa-ultra) on SMA-pistik,
[RIGOL RSA3030N-il](/et/seadmed/spektrianaluusaator-rigol-rsa3030n) N, sinu kaablil tõenäoliselt
kolmas, ja ainus asi, mis need kokku viib, on üleminek.

Seepärast ongi kogu RF-kraam ühes kohas, mitte seadmete vahel laiali.

## Kalibreerimiskomplektid

Kaks open / short / load komplekti: üks N-type pistikutega, teine SMA-ga.

Ilma selleta ei mõõda vektorvõrguanalüsaator midagi mõistlikku. Seade kalibreeritakse **sinu kaabli
otsas**, nende üleminekutega, mida kavatsed kasutada: ühendad järjest lahtise, lühistatud ja 50 Ω
koormusega mõõdu, seade jätab meelde, mida trakt ise juurde annab, ja lahutab selle edaspidi maha.
Ilma kalibreerimiseta mõõdad kaablit koos üleminekutega, mitte antenni.

Mõõdud on täppisdetailid. Maha pillata ja jõuga kinni keerata neid ei tohi.

## DC-blokk

Laseb läbi kõrgsageduse ja ei lase läbi alalispinget. Käib seadme sisendi ette siis, kui kaablis
võib olla alalispinge: fantoomtoitega aktiivantenn, mille toide käib keskjuhti mööda, nihkega
skeemiväljund, mastivõimendi.

tinySA alalispinge piir on ±5 V, RIGOLil ±50 V. DC-blokk on arvestatud kuni 6 GHz ja katab mõlema
seadme sagedusala.

## NanoVNA RF Demo Kit

Plaat pooleteise tosina testahelaga: kõrg- ja madalpääsfiltrid, ribapääs 10,7 MHz juures,
sobitatud ja sobitamata koormused, 50 ja 75 Ω. Kõik väärtused on ette teada ja plaadile peale
kirjutatud.

Ta on selleks, et õppida mõõtma millegi peal, mille vastust sa juba tead: kui demoplaat ei näita
seda, mis talle kirjutatud on, on viga sinu kalibreerimises või kaablis, mitte mõõdetavas skeemis.

## Antennid

SMA vardantennid 433 ja 868 MHz jaoks — LoRa, andurite ja muu argiraadiotelemeetria töösagedused.
Teleskoopantenn SMA-ga on lairibane, häirete otsimiseks ja vastuseks „kas signaali üldse on".

Kindla sageduse jaoks tehtud antenn on sellel sagedusel alati teleskoopantennist parem ja igal
teisel alati halvem.

## Kuidas pistikutega ümber käia

Pistikud on selle konteineri kõige kallim osa ja kõik lõhuvad neid ühtmoodi.

- Keera **mutrit, mitte kaablit ega seadet**. Keskkontakti keerutamine tapab pistiku.
- Käega. N ja SMA käivad sõrmedega kinni; momentvõtit meil igale poole ei jagu ja ülekeeramine
  rikub keerme kindla peale.
- Ära keera viltu: mutter peab esimesest keerust vabalt minema.
- SMA ja RP-SMA näevad välja ühesugused, aga nende keskkontaktid on peegelpildis. Kui „ei lähe
  sisse", siis just sellepärast — ära suru.
- Ära aja segi 50 ja 75 Ω. Takistus on märgitud plaadile ja osale üleminekutest.
- Pane korgid mõõtudele ja seadmete pistikutele tagasi.

## Mida karbis ei ole

**Sumbuteid.** tinySA, HackRF One ja RIGOLi kaardid ütlevad kõik, et saatja väljund jõuab seadmeni
ainult läbi sumbuti — ja see on õige, aga sumbutit ennast praegu konteineris ei ole. Kui sul on
vaja anda analüsaatorile midagi tugevamat kui millivatt, kirjuta meile, ära improviseeri.

## Ligipääs

Konteiner asub hackspace'i ruumis, seega on vaja hackspace'i ligipääsuga paketti. Instruktaaži ei
ole vaja. Komplekti välja ei renti — ta kuulub seadmete juurde, mis jäävad siia.
