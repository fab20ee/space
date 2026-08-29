---
title: "Lauamultimeeter OWON XDM1241"
seoDescription: "55 000 näiduühikuga lauamultimeeter Tallinna hackspace'is. OWON XDM1241 True RMS-i, mahtuvuse, sageduse, temperatuuri ja USB-logimisega täpseteks mõõtmisteks elektroonikalaual."
specs:
  - { label: "Lahutusvõime", value: "55 000 näiduühikut, 4½ kohta" }
  - { label: "Mõõdab",      value: "V, A, Ω, mahtuvus, sagedus, temperatuur, diood, pidevus" }
  - { label: "AC",          value: "True RMS" }
  - { label: "Ekraan",      value: "3,7\" värviline LCD, kaks näitu" }
  - { label: "Liidesed",    value: "USB logimiseks ja arvutitarkvaraks" }
  - { label: "Sisendid",    value: "10 A, mA/µA, COM, V/Ω/°C" }
---

<!-- TODO: kontrolli päris seadme järgi — millised mõõteotsikud ja termopaar on kaasas, kas
     arvutitarkvara on laua arvutisse paigaldatud. -->

Lauamultimeeter on suureks kasvanud käsimultimeeter: võrgutoide, suur ekraan, rohkem numbreid, ja
see ei kao kuhugi. 55 000 näiduühikuga eristab see 5 V vahemikus 0,1 mV, mida on vaja
pingereferentsi kontrollimiseks, takistite sobitamiseks või mõõtetakisti pingelangu nägemiseks.
Topeltekraan näitab kahte suurust korraga — näiteks pinget ja sagedust.

See logib ka üle USB, nii et saad salvestada, kuidas väärtus tunni jooksul triivib, ilma et peaksid
kõrval numbreid üles kirjutama.

## Milleks see sobib

- Täpsed alalispinge ja -voolu mõõtmised prototüüpidel
- Takistite ja kondensaatorite sobitamine, komponentide sorteerimine karpidest
- Mittesiinuseliste vahelduvsignaalide True RMS mõõtmine
- Temperatuur K-tüüpi termopaariga
- Pidevuse ja dioodi testid plaadi silumisel
- Aeglaselt muutuva väärtuse logimine arvutisse

## Ohutus

- Kontrolli **enne** mõõtmist, millistes pesades juhtmed on. Pinge voolusisenditel põletab
  parimal juhul kaitsme.
- 10 A sisend on suure voolu jaoks kaitsmeta — ära ületa seda ja ära kasuta seda kunagi
  võrgupingel.
- Hoia sõrmed mõõteotsikute kaitsekrae taga ja ära mõõda võrgupinget, kui sa ei tea, mida teed, ja
  pole kellelegi öelnud.
- Tühjenda kondensaatorid enne mahtuvuse või takistuse mõõtmist.

## Kuidas kasutada

1. Lülita sisse, ühenda juhtmed COM-i ja mõõdetava suuruse pesasse — V/Ω pinge ja takistuse
   jaoks, mA või 10 A voolu jaoks.
2. Vali funktsioon esipaneeli nuppudega; automaatne vahemik sobib enamiku tööde jaoks, kui näit
   hüpleb, fikseeri vahemik Range-nupuga.
3. Voolu mõõtmiseks katkesta ahel ja ühenda mõõtur jadamisi — selles režiimis on mõõtur lühis.
4. Kasuta Dual-nuppu teise väärtuse näitamiseks ning Record-nuppu või arvutitarkvara ajas
   logimiseks.
5. Lõpus pane juhtmed tagasi pingepesadesse, et järgmine inimene voolukaitset läbi ei põletaks, ja
   lülita välja.

## Ligipääs

Mõõtur asub hackspace'i ruumi elektroonikalaual, seega on vaja paketti, mis sisaldab hackspace'i
ligipääsu. Ohutusinstruktaaži pole vaja.
