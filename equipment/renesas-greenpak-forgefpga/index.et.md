---
title: "Renesase plaadid: GreenPAK ja ForgeFPGA"
seoDescription: "Renesase plaatide konteiner Tallinna hackspace'is: GreenPAK Lite Dev Board koos DIP-korpuses kiipide komplektiga ja ForgeFPGA Evaluation Board 1120 LUT-iga."
specs:
  - { label: "GreenPAK",     value: "GreenPAK Lite Dev. Board Rev 1.1 koos laienduskomplektiga: SLG46537V-DIP ja teised" }
  - { label: "ForgeFPGA",    value: "ForgeFPGA Evaluation Board, kiip SLG47910" }
  - { label: "ForgeFPGA sees", value: "1120 kuue sisendiga LUT-i, 1120 klahvlülitit, 32 kbit BRAM, 50 MHz ostsillaator, PLL, 19 GPIO-d" }
  - { label: "Tarkvara",     value: "Go Configure Software Hub, tasuta" }
  - { label: "Koosseis",     value: "muutub ja täieneb; loend kehtib 19. oktoobri 2026 seisuga" }
---

Kaks plaati ühest ja samast asjast: kuidas saada plaadilt ära peotäis väikest loogikat, asendades
selle ühe kiibiga, mille sa ise seadistasid.

## GreenPAK

GreenPAK on kiip, mille sees on loogikaelemendid, komparaatorid, loendurid, taimerid, DAC ja veidi
analoogosa, ühendatud programmeeritava maatriksiga. Sa joonistad skeemi redaktoris, programmeerid
selle kiipi — ja edasi on see tavaline väike mikroskeem, mis töötab ilma protsessori ja tavapärases
mõttes püsivarata.

Ta katab täpselt selle kihi, mis tavaliselt plaadil ruumi sööb: sisselülitusviide, lihtne riiv, paar
loogikaelementi, pingemonitor, impulsikujundaja. Viie korpuse asemel üks, SOT-i suurune.

**GreenPAK Lite Dev. Board Rev 1.1** on programmaator ja katsestend: kiip pannakse pessa, tarkvara
laeb sinna konfiguratsiooni ja lubab seda emuleerida ilma programmeerimata. Kõrval on
laienduskomplekt DIP-korpuses kiipidega — **SLG46537V-DIP** ja teised. DIP-korpus on selleks, et
kiibi saaks maketeerimislauale torgata ja selle ümber käsitsi skeemi ehitada.

## ForgeFPGA

**ForgeFPGA Evaluation Board** kannab kiipi **SLG47910**, väikest ja odavat FPGA-d. Sees on 1120
kuue sisendiga LUT-i, sama palju klahvlüliteid, 32 kbit plokkmälu, 50 MHz ostsillaator ja PLL ning
19 GPIO-d.

See ei ole Xilinx ega Altera: protsessorituum siia ei mahu. Küll aga mahub see, milleks FPGA-d
väikeses seadmes tavaliselt vaja on: taktitasemel signaalitöötlus, ebatavalised liidesed, loendurid
ja dekoodrid, millega mikrokontroller kas ei jõua või mille peale kulub kogu tema aeg.

Plaat saab toite USB-st.

## Tarkvara

Mõlemad plaadid töötavad **Go Configure Software Hubiga**, Renesase tasuta keskkonnaga. GreenPAK-i
seadistatakse hiirega graafilises redaktoris, ForgeFPGA-d Verilogis.

## Milleks neid võtta

- Saada plaadilt ära loogika ja taimerite puistang, asendades selle ühe kiibiga
- Teha pingemonitor, viide või riiv ilma mikrokontrollerita
- Proovida FPGA-d, ostmata mitmesaja eurost arendusplaati
- Võtta mikrokontrollerilt ära see, mis nõuab ranget ajastust
- Lihtsalt vaadata, kuidas see käib: mõlemad keskkonnad on tasuta ja DIP-kiibid lähevad otse
  maketeerimislauale

## Koosseis muutub

Loend kehtib **19. oktoobri 2026 seisuga**. Plaate lisandub ja mõni läheb projekti. Kui midagi
kohal ei ole, küsi meilt.

Ja kui sinu projekt vajab plaati, mida meil ei ole, kirjuta: oleme tavaliselt valmis juurde ostma.

## Ligipääs

Konteiner asub hackspace'i ruumis, seega on vaja hackspace'i ligipääsuga paketti. Instruktaaži ei
ole vaja.
