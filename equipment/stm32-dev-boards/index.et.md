---
title: "STM32 arendusplaadid"
seoDescription: "STM32 arendusplaatide konteiner Tallinna hackspace'is: Nucleo H7, G4, U0 ja U5, ST-LINK V3 programmaatorid, sealhulgas V3-PWR voolutarbe mõõtmisega."
specs:
  - { label: "Nucleo plaadid", value: "NUCLEO-H7S3L8, NUCLEO-U031R8 (kaks), NUCLEO-G431RB, NUCLEO-U545RE-Q" }
  - { label: "Programmaatorid", value: "ST-LINK V3-PWR ja mitu kompaktset ST-LINK V3" }
  - { label: "Kaablid",      value: "lintkaablid ST-LINK-ide jaoks" }
  - { label: "Üleminekud",   value: "STDC14 → CatCon, RW plaatide pistik" }
  - { label: "Koosseis",     value: "muutub ja täieneb; loend kehtib 19. oktoobri 2026 seisuga" }
---

Konteiner plaatidega, mille peal saab STM32 projekti alustada ilma midagi jootmata ja trükkplaati
joonistamata. Iga Nucleo on kontaktidele välja toodud mikrokontroller, mille peal on juba
programmaator: paned USB otsa ja kirjutad koodi.

Plaadid on meelega erinevad — STM32-l on mitu perekonda ja need on eri asjade jaoks:

- **NUCLEO-H7S3L8** — Cortex-M7, kuni 600 MHz. Karbi kõige võimsam: graafika, signaalitöötlus,
  kõik see, mille jaoks tavalisest kontrollerist jääb väheks.
- **NUCLEO-G431RB** — Cortex-M4 matemaatikakiirendiga. Perekond mootorite juhtimiseks ja
  digitaalseks toiteks.
- **NUCLEO-U031R8** — Cortex-M0+, ülimadal tarbimine. Selle jaoks, mis elab patarei pealt aastaid.
  Neid plaate on kaks — mugav, kui on vaja kahe seadme vahel ühendust üles ehitada.
- **NUCLEO-U545RE-Q** — Cortex-M33 TrustZone'iga. Samuti madal tarbimine, aga riistvaralise
  turvalisusega.

Ülejäänud plaate on üks kummastki.

## Programmaatorid

Karbis on mitu kompaktset **ST-LINK V3** — tavalised silumisprogrammaatorid nende plaatide jaoks,
millel oma peal ei ole.

Eraldi on **ST-LINK V3-PWR**. See on programmaator ja voolutarbe mõõtja ühes: ta toidab plaati
1,6–3,6 V pingega ja mõõdab samal ajal voolu 100 nA-st 550 mA-ni, kuni sada tuhat näidet sekundis,
koodi täitmisega sünkroonis. Nii on näha mitte ainult „kui palju ta sööb", vaid ka see, mis iga
püsivara osa maksab.

Kui on vaja laiemat vahemikku või seade ei ole STM32, on kõrval
[Nordic Power Profiler Kit II](/et/seadmed/voolutarbe-mootja-nordic-ppk2): kuni 1 A, 0,8–5 V ja
kaheksa loogikasisendit, kuigi ilma siluri küljes olemiseta.

## CatCon-üleminekud

Karbis on üleminekud **STDC14-lt** — ST-LINK-i standardselt 14-kontaktiliselt pistikult — **CatCon**
peale, mis on KIISU ja teiste RW plaatide pistik. Ilma selleta ei saa silurit nende plaatide külge
üldse panna, nii et kui töötad RW riistvaraga, alusta sellest üleminekust.

## Koosseis muutub

Ülaltoodud loend kehtib **19. oktoobri 2026 seisuga**. Karp on elav asi: plaate lisandub ja mõni
läheb projekti. Kui midagi loendist kohal ei ole, siis nii juhtub — küsi meilt.

Ja vastupidi: **kui sinu projekt vajab arendusplaati, mida meil ei ole, kirjuta meile.** Oleme
tavaliselt valmis juurde ostma — see maksab vähem, kui arvad, ja järgmine inimene tahab seda ka.

## Kuidas kasutada

1. Võta konteinerist plaat ja vajadusel programmaator koos kaabliga.
2. Paigalda STM32CubeIDE või mõni muu keskkond, millega oled harjunud.
3. Nucleo plaatidele eraldi programmaatorit vaja ei ole — see on plaadi peal, ühenda USB kaudu.
4. Oma plaadi jaoks võta ST-LINK V3 ja sobiv kaabel; RW plaatide jaoks CatCon-üleminek.
5. Pane kõik konteinerisse tagasi, kaablid kaasa arvatud. Kaablid kaovad esimesena.

## Ligipääs

Konteiner asub hackspace'i ruumis, seega on vaja hackspace'i ligipääsuga paketti. Instruktaaži ei
ole vaja.
