---
title: "Reaalaja spektrianalüsaator RIGOL RSA3030N"
seoDescription: "9 kHz – 3 GHz reaalaja spektrianalüsaator vektor-võrguanalüüsiga Tallinna hackspace'is. RIGOL RSA3030N antennide häälestamiseks, RF-silumiseks, häirete otsimiseks ja filtrite mõõtmiseks."
specs:
  - { label: "Sagedusvahemik",   value: "9 kHz – 3 GHz" }
  - { label: "Reaalaja ribalaius", value: "kuni 40 MHz" }
  - { label: "Režiimid",         value: "pühkiv SA, reaalaja SA, VNA (S11, S21), jälgiv generaator" }
  - { label: "Ekraan",           value: "10,1\" puuteekraan" }
  - { label: "Liidesed",         value: "USB, LAN, HDMI" }
  - { label: "Max sisend",       value: "+30 dBm (1 W), ±50 V DC — mitte kunagi ületada" }
---

<!-- TODO: kontrolli päris seadme järgi — millised valikud on litsentsitud (RTSA ribalaius, EMI,
     VNA), millised kaablid, adapterid ja kalibreerimiskomplekt on riiulil. -->

Spektrianalüsaator näitab, mis on eetris või kaablil, sageduse järgi: kus energia on, kui tugev ja
kui lai. See on instrument kõige raadioga seotu jaoks — kontrollida, et LoRa- või Wi-Fi-moodul
saadab seal ja nii tugevalt, kus ja kuidas peab, leida häirete allikas, häälestada antenni või
mõõta filtrit.

RSA3030N lisab kaks asja, mida lihtsal analüsaatoril pole. Reaalaja režiim püüab lühikesi impulsse
ja sagedushüplevaid signaale, millest pühkiv analüsaator mööda vaataks. Ja sisseehitatud
vektor-võrguanalüsaator mõõdab S11 ja S21, nii et antenni sobitust (SWR) või filtri
sageduskarakteristikut näed otse, eraldi instrumendita.

## Milleks see sobib

- Raadiomooduli saatesageduse, võimsuse ja harmooniliste kontrollimine
- Antennide häälestamine: tagasipeegeldus, SWR ja resonants VNA-ga
- Filtrite, sumbutite ja kaablite mõõtmine jälgiva generaatoriga
- EMI ja häirete otsimine plaadil või ruumis
- Bluetoothi, Wi-Fi ja muude hüplevate signaalide jälgimine reaalajas
- Vastuvõtja sisendastme ja impulsstoiteploki spektri kontrollimine

## Ohutus

- **Sisend on õrn koht.** Ära ühenda saatja väljundit kunagi otse — juba 1 W hävitab sisendastme.
  Kasuta sumbutit ja arvuta tase enne paberil läbi.
- Ära anna sisendile kunagi alalispinget ilma DC-blokita; ±50 V on absoluutne piir ja ohutu vastus
  on null.
- Lae kaablid ja antennid enne ühendamist maha: puuduta esmalt pistiku kestaga korpust. Pika antenni
  staatikast piisab sisendi tapmiseks.
- Ära pinguta pistikuid jõuga. N ja SMA keeratakse käega; viltu keeratud keere on jäädav.
- Instrument jääb kohapeale ning selle kaablid ja adapterid jäävad selle juurde.

## Kuidas kasutada

1. Lülita sisse ja lase mõni minut soojeneda, kui taseme täpsus on oluline.
2. Vajuta Preset, et jõuda teada olevasse seisu, siis sea kesksagedus ja vaateriba — või algus- ja
   lõppsagedus — huvipakkuva signaali järgi.
3. Sea referentstase veidi kõrgemale tugevaimast oodatavast signaalist; vähenda lahutusribalaiust
   detailide nägemiseks, suurenda kiiremaks pühkimiseks.
4. Kasuta markereid ja tipuotsingut, ära loe võrku silma järgi.
5. Antennitööks lülitu VNA-režiimi, kalibreeri oma kaabli otsas open/short/load etalonidega, siis
   ühenda antenn ja loe S11 või SWR.
6. Salvesta ekraanipildid USB-le, eemalda oma adapterid, pane kaablid tagasi, lülita välja.

## Ligipääs

Analüsaator asub hackspace'i ruumis, seega on vaja paketti, mis sisaldab hackspace'i ligipääsu.
**Ohutusinstruktaaž on enne esimest kasutamist kohustuslik** — see on lühike ja räägib peamiselt
sellest, kuidas sisendit mitte hävitada.
