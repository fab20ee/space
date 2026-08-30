---
title: "KIISU — taskusuurune tööriist raadio ja NFC jaoks"
seoDescription: "KIISU on krediitkaardisuurune plaat, mis ühildub Flipper Zero püsivaraga: Sub-GHz, NFC, RFID, IR, BLE, iButton, GPIO. Arendab RainWalker Tallinnas; prototüübid valmivad FAB20 töökojas."
---

KIISU on pangakaardisuurune seade, mis teeb sama, mida Flipper Zero, ja töötab selle püsivaraga:
Sub-GHz raadio, NFC ja RFID, infrapunaport, Bluetooth Low Energy, iButton ja väljatoodud GPIO.
Seda teeb RainWalker — sama meeskond, kes teeb FAB20 —, ja töökoda sai projekti kodulaboriks:
siin joodetakse ja silutakse prototüüpe ning testitakse raadioosa.

## Mis on sees

Kaks mikrokontrollerit — STM32WB55 (raadio ja BLE) ja STM32G431 (170 MHz, põhiloogika). CC1101
transiiver Sub-GHz jaoks, ST25R3916 NFC jaoks, IR-vastuvõtja ja -saatja, kiirendusmõõtur
kompassiga, temperatuuri-, niiskus- ja valgusandurid; valikuliselt gaasiandur ja kaugusmõõtur.
Toide LIR2032 akult või USB Type-C kaudu.

## Kaks versiooni

KIISU V4BR — põhiplaat kaardiformaadis. KIISU SMOL — moodulvariant neile, kes tahavad
konstruktorit, mitte valmis seadet.

## Avatud

Skeemid ja püsivara on GitHubis avalikus repositooriumis. Seade on müügil ametlikus poes ja
partnerite juures USA-s, Euroopas, Poolas ja Indias.

## Kuidas töökoda aitas

Kuumaõhu-jootejaam ja BGA-jaam prototüüpide kokkupanekuks ja ümbertegemiseks, mikroskoop peene
jootmise kontrolliks, ostsilloskoop ja spektrianalüsaator toite ja raadioosa silumiseks. Kõik see
seisab hackspace'is ja on paketiga igale liikmele kättesaadav.
