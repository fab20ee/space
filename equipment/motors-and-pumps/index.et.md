---
title: "Mootorid ja pumbad"
seoDescription: "Väikeste mootorite ja pumpade konteiner Tallinna hackspace'is: harjadega mootorid, reduktormootorid, membraan- ja peristaltilised pumbad ning solenoidventiil."
specs:
  - { label: "Mootorid",     value: "väikesed harjadega, osa reduktoriga" }
  - { label: "Pumbad",       value: "membraan- ja peristaltilised, väikese võimsusega" }
  - { label: "Lisaks",       value: "solenoidventiil, voolikud, väike kinnituskraam" }
  - { label: "Toide",        value: "valdavalt madalpinge alalisvool, mõnest voldist 12–24 V-ni" }
  - { label: "Koosseis",     value: "muutub; kirjeldatud on tüüpe, mitte artikleid" }
---

Karp sellega, mis keerleb ja pumpab. Erinevalt
[sammmootoritest](/et/seadmed/sammmootorid-ja-draiverid) on siinsed mootorid lihtsad: panid pinge
peale — keerleb, võtsid ära — jäi seisma. Asendi täpsust siin ei ole, küll aga piisab nende
juhtimiseks ühest transistorist.

Pumbad on väikese võimsusega, vee ja muude mitteagressiivsete vedelike jaoks: taimede kastmine,
vedeliku ümberpumpamine, jahutuse etteanne isetehtud seadmetes.

## Mida teada

- **Pinge on mootori peale kirjutatud** või tema koti peal. Rohkem annab rohkem pöördeid ja
  tunduvalt lühema eluea.
- **Käivitusvool on kordades suurem töövoolust.** Mootor, mis töös sööb pool amprit, võtab
  käivitusel kaks. Draiver ja toiteallikas arvesta käivituse järgi.
- **Vastuvooludiood on kohustuslik.** Iga mähis annab väljalülitamisel pingehüppe, mis tapab
  transistori või mikrokontrolleri jala. Ilma dioodita töötab skeem täpselt esimese
  väljalülitamiseni.
- **Osa pumpasid on isetäituvad, osa mitte.** Membraanpump tõstab vee ise üles, peristaltiline
  doseerib täpselt, ja kumbki ei salli kuivalt töötamist.
- **Kontrolli, kas pump tohib seista pinge all** ilma vooluta. Osa mudeleid kuumeneb üle mõne
  minutiga.

## Kuidas kasutada

1. Võta mootor või pump karbist ja vaata tema markeeringut.
2. Katseta [laboritoiteplokil](/et/seadmed/toiteplokk-owon-spe3102) voolupiiranguga: nii on kohe
   näha nii töö- kui ka käivitusvool.
3. Juhtimiseks võta transistor või valmis draiverimoodul
   [moodulite karbist](/et/seadmed/elektroonikamoodulid) ja ära unusta dioodi.
4. Pumpa katseta kraanikausi või vaagna kohal, mitte seadmetega laua kohal.
5. Pane kõik karpi tagasi ja keri voolikud kokku.

## Ligipääs

Konteiner asub hackspace'i ruumis, seega on vaja hackspace'i ligipääsuga paketti. Instruktaaži ei
ole vaja.
