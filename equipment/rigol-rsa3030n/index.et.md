---
title: "Spektrianalüsaator RIGOL RSA3030N"
seoDescription: "Reaalaja spektrianalüsaator 9 kHz – 3 GHz koos VNA, jälgiva generaatori ja EMI-lisaga Tallinna hackspace'is. RIGOL RSA3030N, TekBoxi TEM-kamber, kalibreerimiskomplekt. Ligipääs 24/7."
specs:
  - { label: "Sagedusala",          value: "9 kHz – 3 GHz" }
  - { label: "Reaalaeg",            value: "riba 10 MHz" }
  - { label: "Režiimid",            value: "pühkiv, reaalaja, EMI, VNA (S11, S21, DTF)" }
  - { label: "Jälgiv generaator",   value: "on" }
  - { label: "Ekraan",              value: "puutetundlik 10,1\"" }
  - { label: "Liidesed",            value: "USB, LAN, HDMI" }
  - { label: "Max sisend",          value: "+30 dBm (1 W), ±50 V DC" }
  - { label: "Kõrval",              value: "TEM-kamber TekBox TBTC1, NanoVNA demoplaat, RF-üleminekud, kalibreerimiskomplekt" }
---

Spektrianalüsaator näitab, mis on eetris või kaablis: millistel sagedustel on energiat, kui
võimsalt ja kui laialt. See on seade kõige raadioga seotud jaoks: kontrollida, et LoRa- või
Wi-Fi-moodul saadab seal, kus peab, leida häirete allikas, häälestada antenn või mõõta filter.

RSA3030N-il on tavalise analüsaatori kõrval kolm asja rohkem. Reaalajarežiim püüab lühikesed
impulsid ja sagedust hüpitavad signaalid, millest pühkiv analüsaator mööda vaatab. Sisseehitatud
vektorvõrguanalüsaator mõõdab S11 ja S21, nii et antenni sobitus ja filtri karakteristik on näha
ilma eraldi seadmeta. Ostetud on EMI-lisa: CISPR-i ribad ja kvaasitipp-detektor oma plaadi
häirete hindamiseks enne sertifitseerimist.

Sellega on häälestatud projekti KIISU antennid; seade on ka projekti seadmete loendis allpool.

## Mis on kõrval

- **TEM-kamber TekBox TBTC1**: avatud kamber väikese plaadi elektromagnetiliste häirete
  eelhindamiseks, kuni 3 GHz, plaadi ruum 190 × 130 × 50 mm, komplektis koormus ja DC-blokk.
  Plaat pannakse sisse, analüsaator näitab, mida see kiirgab.
- **NanoVNA RF Demo Kit**: 18 testahelat, filtrid ja sumbutid, et õppida VNA-mõõtmisi teada
  tuntud objektidel.
- Eri tüüpi RF-üleminekute komplekt ja VNA kalibreerimiskomplekt.

Kõik see jääb seadme juurde.

## Seadme sisend

Ainus asi, mida saab sekundiga rikkuda, on sisendtrakt.

- Ära ühenda saatja väljundit otse. Sisendi piir on +30 dBm ehk 1 W; arvuta tase ja pane sumbuti.
- Ära anna sisendile alalispinget ilma DC-blokita. Piir on ±50 V, ohutu väärtus on null.
- Enne pika kaabli või antenni ühendamist puuduta pistiku korpusega seadme kere, et staatika maha
  laadida.
- N- ja SMA-pistikud keeratakse käega, ilma tööriistata ja ilma viltu ajamata.

## Kuidas kasutada

1. Lülita sisse, tasemetäpsuse jaoks lase mõni minut soojeneda.
2. Vajuta Preset, seejärel sea kesksagedus ja vaateriba või algus- ja lõppsagedus.
3. Referentstase pane veidi kõrgemale kõige tugevamast oodatavast signaalist. Lahutusriba
   vähenda, et näha detaile, suurenda, et skaneerida kiiremini.
4. Markerid ja tipuotsing on täpsemad kui võrgu lugemine silmaga.
5. Antenni jaoks lülitu VNA-režiimi, kalibreeri kalibreerimiskomplekti open-, short- ja
   load-standarditega oma kaabli otsas, siis ühenda antenn ja loe S11 või SWR.
6. Ekraanipildid salvestuvad USB-le. Lõpus võta oma üleminekud ära, pane kaablid ja komplektid
   tagasi, lülita seade välja.

## Ligipääs

Analüsaator asub hackspace'i ruumis, vaja on hackspace'i ligipääsuga paketti. Instruktaaži ei ole
vaja, aga loe sisendi osa läbi enne esimest ühendamist.
