---
title: "Ekraanid ja indikaatorid"
seoDescription: "Ekraanide konteiner Tallinna hackspace'is: TFT, OLED, 1602 sümbolekraanid, LED-maatriksid ja seitsmesegmendilised indikaatorid Arduino ja STM32 prototüüpide jaoks."
specs:
  - { label: "TFT",          value: "värviline umbes 3,5-tolline ekraan lintkaabliga" }
  - { label: "OLED",         value: "mitu monokroomset umbes tollist moodulit, plaatidel ja palja kaablina" }
  - { label: "Sümbolekraan", value: "1602 LCD — kaks rida kuueteistkümne sümboliga" }
  - { label: "Maatriksid",   value: "8 × 8 LED" }
  - { label: "Seitsmesegmendilised", value: "neljakohalised ja üksikud, lisaks ribaindikaator" }
  - { label: "Koosseis",     value: "muutub; kaart kirjeldab tüüpe, mitte konkreetseid artikleid" }
---

Karp ekraanidega prototüüpide jaoks. Iga projekt jõuab varem või hiljem küsimuseni „kuidas ma
näen, mis seal sees toimub", ja siis algab valik: näidata arvu, joonistada graafik või saada
hakkama vilkuva LED-iga.

Siin on kõik see, mille peal seda proovida, enne kui tellida ekraan oma plaadi jaoks.

## Mis siin on ja milleks

- **Umbes 3,5-tolline TFT** — värviline, taustavalgusega, ühendub lintkaabliga. Piltide,
  graafikute ja nuppudega liidese jaoks. Tahab tunduvalt rohkem jalgu ja mälu kui ülejäänud.
- **Umbes tollised OLED-moodulid** — monokroomsed, I²C või SPI kaudu, kaks kuni neli juhet. Kõige
  tavalisem valik väikese seadme jaoks: kontrastsed, taustavalgust ei vaja, lihtne ühendada. Osa on
  valmis plaatidel, osa paljad FPC-sabaga — viimased neile, kes joonistavad oma plaati.
- **Sümbolekraan 1602** — kaks rida kuueteistkümne sümboliga, paralleelliides või I²C-moodul, kui
  mõni juhtub olema. Vana, lihtne ja väga ettearvatav asi.
- **8 × 8 LED-maatriksid** — jooksev tekst, ikoonid, lihtne animatsioon.
- **Seitsmesegmendilised indikaatorid** — neljakohalised ja üksikud. Siis, kui on vaja näidata
  arvu ja ei midagi muud: kell, loendur, temperatuur.
- **Ribaindikaator** — segmentide sammas taseme või edenemise jaoks.

## Mida enne ühendamist teada

- **Pinge.** Osa mooduleid on 3,3 V, osa talub 5 V. Viie voldi andmine kolmevoldisele OLED-ile
  juhtub üks kord. Kui plaadil selget märgistust ei ole, mõõda ja vaata andmelehte.
- **Liides.** I²C on kaks juhet ja aeglane, SPI rohkem juhtmeid ja kiire, paralleelliides palju
  juhtmeid. TFT animatsiooni jaoks on see vahe oluline.
- **Paljaste ekraanide FPC-sabad on haprad.** Neid ei tohi murda ega tõmmata: rajad katkevad sees
  märkamatult ja ekraan lihtsalt ei lülitu enam sisse.
- **Teegid.** Peaaegu kõigele siin on olemas valmis teek Arduino ja STM32 jaoks. Alusta teegi
  näitest, mitte oma koodist: nii saad kohe teada, kas moodul on elus.

## Kuidas kasutada

1. Võta moodul ja vaata plaadil olevat kontrolleri markeeringut — selle järgi leiad nii teegi kui
   ka andmelehe.
2. Pane maketeerimislauale kokku ja kontrolli teegi näitega.
3. Pane moodul karpi tagasi, mitte taskusse ega oma laua sahtlisse.
4. Kui moodul ei tööta, pane ta eraldi ja anna meile teada, et järgmine inimene ei kulutaks tema
   peale õhtut.

Kokkupanekuks vajalik — ühendusjuhtmed, maketeerimislauad, traat — on
[komponendikarpides](/et/seadmed/elektroonikakomponendid-ja-kulumaterjalid).

## Ligipääs

Konteiner asub hackspace'i ruumis, seega on vaja hackspace'i ligipääsuga paketti. Instruktaaži ei
ole vaja.
