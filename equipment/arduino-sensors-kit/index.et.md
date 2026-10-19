---
title: "Arduino andurite komplekt, 37 ühes"
seoDescription: "37-osaline andurite ja moodulite komplekt Arduino jaoks Tallinna hackspace'is: temperatuur, valgus, liikumine, heli, Hall ja IR, sahtlikarbis märgistatud pesadega."
specs:
  - { label: "Mooduleid",    value: "37, igaüks omas pesas" }
  - { label: "Mis sees on",  value: "temperatuur ja niiskus, valgus, Hall, kalle, löök, heli, IR vastuvõtt ja saatmine, nupud, enkooder, sumistid, LED-moodulid" }
  - { label: "Liides",       value: "enamasti kolm või neli jalga: toide, maa, signaal" }
  - { label: "Vaheleht",     value: "leht kõigi moodulite piltide ja nimedega" }
---

Sahtlikarp, kus iga pesa on eraldi moodul väikesel plaadil: andur, nupp, sumisti, LED.
Kolmkümmend seitse tükki ja nende juurde vaheleht piltidega, mille järgi saab aru, mis on mis.

See on komplekt esimese sammu jaoks. Küsimus „kuidas ma üldse mikrokontrolleriga temperatuuri
mõõdan" saab siin kümne minutiga vastuse: võtad mooduli, kolm juhet, teegi näite — ja arv on
ekraanil. Mida edasi teha, saab selgeks juba elusa riistvara peal, mitte teoorias.

## Mis seal on

Täpne koosseis on vahelehel, aga üldjoontes:

- **Keskkond**: temperatuur ja niiskus, analoogtemperatuuriandur, valgus
- **Asend ja liikumine**: kalle, löök ja vibratsioon, Halli andur, roopalüliti
- **Inimene**: nupud, pöördenkooder, puuteandur, pulsiandur
- **Valgus ja IR**: eri värvi LED-moodulid, IR-saatja ja -vastuvõtja, lasermoodul
- **Heli**: mikrofon, aktiivne ja passiivne sumisti

Peaaegu kõik ühendub ühtmoodi: toide, maa ja üks signaalijalg, analoog- või digitaalne.

## Mida sellelt oodata ei tasu

See on õppekomplekt, mitte mõõteriistad. Siinsed andurid annavad suurusjärgu ja sündmuse fakti —
„läks soojemaks", „koputati", „pandi valgus põlema". Kui on vaja päris täpsust, võta korralik andur
ja vaata tema andmelehte, mitte seda sahtlikarpi.

Ja moodulid on tehtud Arduino 5 V loogika jaoks. Kolmevoldise plaadiga osa neist töötab, osa mitte,
ja osa annab signaalijalale viis volti ning rikub sisendi ära. Kontrolli enne ühendamist.

## Kuidas kasutada

1. Leia moodul vahelehe järgi ja võta pesast välja.
2. Tee kindlaks, mis kiip plaadil on, ja leia näide: enamikul neist moodulitest on valmis teek.
3. Pane maketeerimislaual kokku. Ühendusjuhtmed ja maketeerimislauad on
   [komponendikarpides](/et/seadmed/elektroonikakomponendid-ja-kulumaterjalid).
4. **Pane moodul samasse pessa tagasi.** Komplekt, kus kõik on segamini, lakkab olemast komplekt:
   sealt otsimine võtab kauem kui uue tellimine.

## Ligipääs

Sahtlikarp asub hackspace'i ruumis, seega on vaja hackspace'i ligipääsuga paketti. Instruktaaži ei
ole vaja.
