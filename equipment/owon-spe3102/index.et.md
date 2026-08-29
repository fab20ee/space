---
title: "Programmeeritav toiteplokk OWON SPE3102"
seoDescription: "Programmeeritav laboritoiteplokk Tallinna hackspace'is. OWON SPE3102: 0–30 V, 0–10 A, 200 W, üle- pinge- ja voolukaitsega ning USB-laadimispordiga."
specs:
  - { label: "Väljund",     value: "0–30 V, 0–10 A, 200 W" }
  - { label: "Lahutusvõime", value: "1 mV / 1 mA" }
  - { label: "Kaitse",      value: "OVP, OCP, ülekuumenemine" }
  - { label: "Ekraan",      value: "2,8\" värviline LCD V/A trendigraafikuga" }
  - { label: "Lisad",       value: "5 V / 1 A USB-laadimisport, USB arvutist juhtimiseks" }
---

<!-- TODO: kontrolli päris seadme järgi — püsivara, kas arvutist juhtimine on seadistatud,
     millised juhtmed on kaasas. -->

Laua peamine toiteplokk. Programmeeritav toiteplokk annab puhta, reguleeritava alalispinge ja
voolupiiri, mille sead ise — nii et kui värskes skeemis on lühis, jääb plokk lihtsalt piirile pidama,
selle asemel et suitsu välja lasta. Saadaoleva 10 A juures toidab see ka mootoreid, LED-ribasid ja
kütteelemente, mitte ainult väikeseid loogikaplaate.

Ekraan näitab pinget ja voolu reaalajas ning joonistab trendigraafiku, mis on kasulik, kui tahad
jälgida, kui palju seade aja jooksul tegelikult tarbib.

## Milleks see sobib

- Prototüübi toitmine täpselt vajaliku pingega ja ohutu voolupiiriga
- Lühise otsimine: sea piir madalale, vaata, kuidas pinge kokku kukub, otsi soe detail
- Seadme tarbimise mõõtmine — jõudeolekus, töös, unerežiimis
- Akude laadimine või testimine järelevalve all, OVP valvurina
- Mootorite, pumpade, LED-ribade ja muude kuni 200 W koormuste toitmine

## Ohutus

- Sea voolupiir **enne** skeemi ühendamist ja nii madalale, kui skeem lubab. Just see päästab
  plaadid.
- Kontrolli polaarsust kaks korda. Punane on pluss, must on miinus; roheline klemm on maandus, mitte
  miinus.
- 10 A läbi peenikeste juhtmete või makettplaadi on tuleoht — kasuta suurte voolude jaoks
  korralikke juhtmeid.
- Ära ühenda toiteploki väljundit kunagi pinge all oleva skeemi ega teise toiteallikaga.
- Ära kasuta seda liitiumelementide jaoks ilma korraliku laadimisskeemita või inimeseta, kes teab,
  mida ta teeb.

## Kuidas kasutada

1. Lülita sisse **väljalülitatud** väljundiga. Sea pinge nupu ja V-klahviga, siis voolupiir
   I-klahviga.
2. Soovi korral sea OVP ja OCP veidi tööväärtustest kõrgemale teise valvurina.
3. Ühenda juhtmed skeemiga, kontrolli polaarsust, siis vajuta On/Off, et väljund sisse lülitada.
4. Jälgi ekraani: kui CC-indikaator põleb, on plokk voolupiiris — skeem tarbib rohkem, kui lubasid.
5. Lõpus lülita esmalt väljund välja, siis ühenda juhtmed lahti, siis lülita seade välja.

## Ligipääs

Toiteplokk asub hackspace'i ruumi elektroonikalaual, seega on vaja paketti, mis sisaldab hackspace'i
ligipääsu. Ohutusinstruktaaži pole vaja.
