---
title: "Kaasaskantav spektrianalüsaator tinySA Ultra"
seoDescription: "Taskus mahtuv spektrianalüsaator 100 kHz – 5,3 GHz Tallinna hackspace'is: tinySA Ultra sisseehitatud signaaligeneraatoriga. Töötab akult, saab ka rentida."
specs:
  - { label: "Sisendi sagedusala", value: "100 kHz – 800 MHz, Ultra-režiimis kuni 5,3 GHz" }
  - { label: "Lahutusfiltrid",     value: "0,2 / 1 / 3 / 10 / 30 / 100 / 300 / 600 / 850 kHz" }
  - { label: "Generaator",         value: "siinus 100 kHz – 800 MHz, −115…−19 dBm 1 dB sammuga; meander kuni 4,4 GHz" }
  - { label: "Max sisend",         value: "+6 dBm 0 dB sumbutusel, ±5 V alalispinget" }
  - { label: "Ekraan",             value: "puutetundlik 4\", 480 × 320" }
  - { label: "Toide",              value: "sisemine aku, umbes 2 tundi; laeb USB-C kaudu" }
  - { label: "Mälu",               value: "microSD-kaart seadmes, ekraanipildid salvestuvad sinna" }
  - { label: "Komplektis",         value: "teleskoopantenn SMA-pistikuga, randmepael" }
---

Spektrianalüsaator näitab, millistel sagedustel on energiat ja kui palju. tinySA Ultra teeb seda
vahemikus 100 kHz – 5,3 GHz, mahub jopetaskusse ja töötab oma akult. Sellega kontrollitakse, kas
moodul saadab ja millisel sagedusel, ja otsitakse, kust müra tuleb — seal, kus küsimus tekkis,
mitte töölaua taga.

Meil on juba [RIGOL RSA3030N](/et/seadmed/spektrianaluusaator-rigol-rsa3030n): suur, täpne, VNA ja
EMI-lisaga. RIGOL seisab laual ja mõõdab korralikult, tinySA saab kaasa võtta. Häired korteris,
raadiomooduli kiire kontroll kohapeal, analüsaator objektile kaasa — see on tinySA. Ausad tasemed,
dünaamiline ulatus ja sertifitseerimiseelsed mõõtmised — see on RIGOL.

Sees on ka signaaligeneraator, nii et seade töötab ka teistpidi: annad signaali ja vaatad, mida
filter, kaabel, sumbuti või vastuvõtja sellega teeb.

## Milleks see sobib

- Kontrollida, et 433/868 MHz, Wi-Fi või BLE moodul saadab seal, kus peab, mitte kõrvalkanalil
- Vaadata oma saatja harmoonikuid ja otsustada, kas filtrit on vaja
- Leida häirete allikas: impulsstoiteplokk, laadija, LED-riba draiver
- Võrrelda kahte antenni ja näha, kumb on vajalikul sagedusel parem
- Kontrollida kaablit, üleminekut või sumbutit sisseehitatud generaatoriga
- Vaadata enne oma raadio ülespanekut, kui hõivatud sagedusala on

## Generaator

Alla 800 MHz annab seade siinuse tasemega −115 kuni −19 dBm 1 dB sammuga — sellest piisab, et anda
vastuvõtjale kontrollitud nõrk signaal ja leida selle tundlikkuse piir.

Üle 800 MHz ja kuni 4,4 GHz on väljund meander. Meander on harmoonikute poolest rikas, seega
tasemeetalonina see ei kõlba; kontrollimiseks, kas signaal läbi tuleb, piisab sellest.

Signaal väljub sama RF-pistiku kaudu, mis on ka sisend. Eraldi CAL-pistik on seadme enesekontrolli
jaoks mõeldud 30 MHz referentssignaal, mitte teine väljund.

## Kuidas sisendit mitte ära põletada

Korpusele pistiku kõrvale on trükitud „+6 dBm RF, 5 VDC Max".

- +6 dBm on absoluutne maksimum nulli sumbutusel. Saatja väljund, ka väikese võimsusega, läheb
  sisse ainult läbi sumbuti.
- Alalispinge sisendil peab jääma alla ±5 V, ohutu väärtus on null. Kaabel, mille keskjuhis kannab
  toidet (mastivõimendi, aktiivne GPS-antenn), vajab DC-blokki.
- Enne pika kaabli või antenni ühendamist puuduta pistiku korpusega seadme kere, et staatika maha
  laadida.
- SMA keeratakse sõrmedega — ilma võtmeta ja ilma viltu ajamata.

Sumbutid, DC-blokid, üleminekud ja kaablid on eraldi RF-konteineris, millel on oma kaart ja oma
kleebis.

## Kuidas kasutada

1. Seade on plastkonteineris riiulil. Konteineri koht riiulil kannab sama kleebist M05 — sinna ta
   tagasi käibki.
2. Lülita sisse ja vaata aku olekut. Laeb USB-C kaudu, täis akuga töötab umbes kaks tundi.
3. Sea algus- ja lõppsagedus või kesksagedus koos vaateribaga.
4. Ultra-režiim on sellel seadmel juba avatud, nii et üle 800 MHz vaatab ta kohe. Kui pärast
   püsivara uuendust jääb pühkimine 800 MHz peale seisma, lülita see uuesti sisse: CONFIG → MORE
   → ENABLE ULTRA, kood 4321.
5. Lahutusriba vähenda, et näha kitsaid signaale, suurenda, et kiiremini skaneerida. 0,2 kHz juures
   võtab täisriba pühkimine väga kaua, seega kasuta kitsaid filtreid kitsal ribal.
6. Marker ja tipuotsing loevad sagedust ja taset paremini kui silm võrgustikku. Ekraanipildid
   salvestuvad microSD-kaardile.
7. Teleskoopantenn sobib häirete otsimiseks ja vastuseks „signaal on / ei ole". Taseme mõõtmiseks
   on vaja kaablit ja selle sumbuvuse arvestamist.
8. Lülita välja, lükka antenn kokku, pane seade konteinerisse ja konteiner oma kohale tagasi.

## Rentimine

Selle seadme saab koju kaasa: broneerid saidil ja võtad kleebisel oleva koodi järgi ükskõik mis
kellaajal. Enamasti võetakse see selleks, et leida, mis kodus või töökojas müra teeb, või
objektile, kuhu raadiot paigaldatakse. Päevahind ja tähtaeg on selle lehe rendiplokis.

## Ligipääs

Konteiner asub hackspace'i ruumis, seega on vaja hackspace'i ligipääsuga paketti. Instruktaaži ei
ole vaja, aga loe sisendi osa läbi enne, kui sellega midagi ühendad.
