---
title: "Kaasaskantav toiteplokk FNIRSI DPS-150"
seoDescription: "FNIRSI DPS-150 Tallinna hackspace'is: taskusuurune laboritoiteplokk kuni 30 V ja 5 A, toide USB-C PD laadijast. Saab rentida ja kaasa võtta."
specs:
  - { label: "Väljund",        value: "0 – 30 V, 0 – 5 A, kuni 150 W" }
  - { label: "Seadistussamm",  value: "10 mV pinge, 1 mA voolu jaoks" }
  - { label: "Pulsatsioon",    value: "alla 20 mV" }
  - { label: "Toide",          value: "USB-C PD või QC toega, või DC-pesa 5 – 30 V" }
  - { label: "Režiimid",       value: "CV ja CC, kuus mälupesa M1 – M6" }
  - { label: "Kaitsed",        value: "üle pinge, voolu, võimsuse, temperatuuri, lühise ja pooluste vahetuse vastu" }
  - { label: "Ekraan",         value: "2,8\" IPS, pöördub 90°" }
  - { label: "Arvestus",       value: "ampertunnid, vatt-tunnid, aeg koormuse all" }
  - { label: "Mõõdud",         value: "106 × 76 × 28 mm, 178 g" }
  - { label: "Komplektis",     value: "krokodillklambritega juhtmed" }
---

Laboritoiteplokk kaardipaki suurusega. Annab nullist kuni 30 V ja kuni 5 A, piirab voolu, loeb
antud ampertunde ja vatt-tunde — kõik see, mida teeb suur lauatoiteplokk, ainult et mahub taskusse
ja töötab tavalisest sülearvuti laadijast.

Tõsise töö jaoks on hackspace'is [OWON SPE3102](/et/seadmed/toiteplokk-owon-spe3102): kaks kanalit,
võrgutoide, ausad näitajad. DPS-150 on teise olukorra jaoks — kui toide peab tulema sinna, kus sa
töötad, või koju kaasa minema.

## Toide ja üks tõeline piirang

Ta töötab USB-C pealt PD-ga — sobib ükskõik milline sülearvuti laadija hackspace'is — või
tavalisest plokist ümara pistikuga, 5 kuni 30 V. Mõlemat korraga sisse panna ei tohi, see on
korpusele kirjutatud.

Ja nüüd oluline: **DPS-150 on pinget alandav muundur**. Väljundpinge on alati sisendpingest
madalam. PD-laadijast võtab ta kõige rohkem 20 V, seega väljundis saad veidi alla kahekümne. Kui
tahad kolmekümne lähedale, on vaja eraldi 24–30 V plokki ümarasse pesasse. Üle 30 V sisendisse anda
ei tohi, see tapab seadme.

Sama lugu on võimsusega: 150 W tuleb ainult allikast, mis seda anda suudab. 65 W laadija annab
umbes 65 W, ja see on normaalne — lihtsalt tea, miks.

## Milleks see sobib

- Toita prototüüpi või plaati voolupiiranguga, et skeemiviga ei muutuks ilutulestikuks
- Seada pinge 10 mV täpsusega ja vaadata, kuidas seade oma vahemiku piiril käitub
- Laadida või tühjendada midagi kontrolli all ja näha, mitu ampertundi kulus
- Viia toide seadme juurde, mida ei saa lauale tuua
- Töötada kodus, kui töökoht on seal

## Kuidas kasutada

1. Võta seade ja krokodillklambritega juhtmed riiulil olevast konteinerist ning laadijaks ükskõik
   milline vaba PD-laadija hackspace'is.
2. Pane toide sisse. Ekraanile ilmub sisendpinge, nii et näed kohe, mida laadija andis ja millele
   loota.
3. **Enne koormuse ühendamist** sea Vset ja Iset. Voolupiirang ei ole formaalsus, vaid ainus asi,
   mis su plaadi vea korral päästab.
4. Ühenda krokodillid õigetpidi ja lülita väljund sisse.
5. CV või CC märk näitab, millesse seade on kinni jooksnud: seatud pingesse või seatud voolu. Ootamatu
   üleminek CC-sse tähendab, et koormus võtab rohkem, kui sa lubasid, ja see on põhjus väljund välja
   lülitada ning uurida, miks.
6. Sageli kasutatavad seaded pane mälupesadesse M1 – M6.
7. Lõpus lülita väljund välja, ühenda koormus lahti ja pane seade koos juhtmetega konteinerisse
   tagasi.

## Rentimine

Selle seadme saab koju kaasa. **Laadija rendikomplekti ei kuulu** — võta oma sülearvuti või telefoni
laadija, peaasi et see oskaks PD-d. Päevahind ja tähtaeg on selle lehe rendiplokis.

## Ligipääs

Konteiner asub hackspace'i ruumis, seega on vaja hackspace'i ligipääsuga paketti. Instruktaaži ei
ole vaja.
