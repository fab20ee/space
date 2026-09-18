---
title: "Plaadihoidik ja mõõteotsikud Sensepeek PCBite"
seoDescription: "Sensepeek PCBite Tallinna hackspace'is: A4 ja A5 terasplaadid, magnetilised plaadihoidikud ja otsikud painduvatel varrastel, sealhulgas SQ200 ostsilloskoobi otsik 200 MHz."
specs:
  - { label: "Alusplaadid",     value: "kaks, terasest: A4 (297 × 210 mm) ja A5 (210 × 148 mm)" }
  - { label: "Plaadihoidikud",  value: "neli magnethoidikut kummagi plaadi kohta" }
  - { label: "Ostsilloskoobi otsik", value: "SQ200, 10:1, DC – 200 MHz, 10 MΩ / 13,9 pF tipus — üks" }
  - { label: "Nõelotsikud",     value: "neli koos juhtmetega, multimeetri või toite jaoks" }
  - { label: "Ostsilloskoobi sisend", value: "1 MΩ" }
  - { label: "Max pinge",       value: "300 V RMS CAT II, ja ainult koos sõrmekaitsmega" }
  - { label: "Otsiku kinnitus", value: "painduv vars magnetalusel, seisab plaadil ükskõik kus" }
  - { label: "Kuluvosa",        value: "varunõelad katsutis" }
---

PCBite lahendab selle, mis muudab plaadi silumise tsirkuseks: käsi on kaks, aga hoida tuleb
plaati, kahte otsikut ja samal ajal ostsilloskoobi nuppe keerata. Plaat kinnitub magnethoidikute
vahele terasplaadi kohal ja otsikud seisavad painduvatel varrastel magnetalustel — panid nõela
jala peale ja see jääbki sinna.

Edasi saab rahulikult ekraani vaadata, ajatelge muuta, kõrval joota või pildistada: otsik ei libise
ära ja plaat ei jookse minema.

## Millest komplekt koosneb

See ei ole karbis ostetud komplekt, vaid Sensepeeki osad, mis pannakse kokku vastavalt tööle:

- **Kaks alusplaati**, mõlemad terasest ja magnetilised: suur A4 ja väike A5. Üks külg on matt,
  teine peegelpoleeritud — poleeritud küljel on hea filmida ja kukkunud SMD-detaili otsida.
- **Magnetilised plaadihoidikud**, neli plaadi kohta. Plaat toetub neile servadega ja ripub
  alusplaadi kohal, nii et joota ja mõõta saab mõlemalt poolt. Hoidikud käivad ükskõik kuhu, sest
  nad püsivad magnetiga.
- **SQ200 ostsilloskoobi otsik** — tavaline 10:1 otsik, konksu asemel vedruga nõel, riba kuni
  200 MHz. Neid on **üks**: kahe kanali vaatamiseks tuleb teist käes hoida tavalise
  ostsilloskoobiotsikuga.
- **Neli nõelotsikut** koos juhtmetega — multimeetri, toite ja kõige muu jaoks, millel on
  banaanpistikud.
- **Katsuti varunõeltega.**

Kombineerida saab vabalt: väike plaat kahe otsikuga mikroskoobi all, suur plaat nelja hoidikuga
pika plaadi jaoks või mõlemad plaadid kõrvuti, kui plaate on kaks.

## Milleks see sobib

- Vaadata signaale ostsilloskoobiga, ilma et peaks otsikut käes hoidma
- Panna multimeeter ja toide korraga nelja punkti ega hoida midagi käes
- Hoida plaati jootmise ja ümbertegemise ajal „kolmanda käe" asemel
- Otsida hüplevat kontakti: otsik ei liigu ja plaat ka mitte
- Töötada mikroskoobi all — väike plaat ongi täpselt selleks

10:1 otsik on tehtud 1 MΩ sisendi jaoks, see tähendab [Micsig TO3004
ostsilloskoobi](/et/seadmed/ostsilloskoop-micsig-to3004) jaoks, mis seisab samal laual.

## Kuidas seda mitte lõhkuda

- Nõelad on vedruga ja peenikesed. Kontakt tekib kerge surve peale; tugevamini surudes need
  painduvad ja murduvad. Varunõelad on katsutis, aga neid ei ole lõputult.
- 300 V RMS CAT II on piir ja see kehtib ainult koos sõrmekaitsmega. Võrguahelaid nende otsikutega
  ei mõõdeta.
- Alusplaat on terasest ja juhib voolu. Plaat käib hoidikute peale, mitte alusplaadile lamama.
- Painduvat vart painuta varrest, mitte otsiku kaablist.

## Kuidas kasutada

1. Võta oma plaadile sobiv alusplaat, sea neli hoidikut paika ja kinnita plaat servadest.
2. Pane otsiku magnetalus alusplaadile soovitud koha lähedale, vii nõel varrega jala juurde ja suru
   kergelt.
3. Otsiku maa ühenda plaadi maaga lühikese juhtmega, mitte pika sabaga — kõrgel sagedusel näitab
   pikk maasilmus sulle häiret, mitte sinu signaali.
4. Sea ostsilloskoobil 10:1, kui see ise suhet ei tuvastanud.
5. Lõpus võta otsikud ära, pane varred kokku ja tõsta see, mille riiulilt võtsid, karpi tagasi.
   Painutatud nõel vaheta katsutist ja anna meile teada, et uued tellitaks.

## Kus mis asub

Elektroonikalaual on tavaliselt väike plaat, neli hoidikut ja paar nõelotsikut — sellest piisab
enamiku tööde jaoks. Kõik ülejäänu, sealhulgas suur plaat ja ostsilloskoobi otsik, on riiulil
plastkarbis. Mis karbist välja tuleb, läheb karpi tagasi.

## Ligipääs

Komplekt asub hackspace'i ruumis, seega on vaja hackspace'i ligipääsuga paketti. Instruktaaži ei
ole vaja.
