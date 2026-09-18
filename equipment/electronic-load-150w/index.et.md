---
title: "Elektrooniline koormus 150 W"
seoDescription: "150 W elektrooniline koormus Tallinna hackspace'is: testi toiteplokki koormuse all, mõõda aku tegelikku mahtuvust, väljalülitus voolu, pinge ja aja järgi."
specs:
  - { label: "Võimsus",      value: "kuni 150 W" }
  - { label: "Režiim",       value: "voolu stabiliseerimine (CC)" }
  - { label: "Arvestus",     value: "antud ampertunnid ja vatt-tunnid, aeg koormuse all" }
  - { label: "Väljalülitus", value: "voolu, pinge ja aja järgi" }
  - { label: "Ühendus",      value: "kruviklemm, toetab nelja juhtme mõõtmist" }
  - { label: "Toide",        value: "ainult välisest toiteplokist, see on tema juures" }
  - { label: "Jahutus",      value: "radiaator ventilaatoriga" }
  - { label: "Mudel",        value: "puudub — plaadil ei ole markeeringut" }
---

Elektrooniline koormus on takisti, mida saab käskida. Sa ütled „tarbi kolm amprit", ta tarbibki
täpselt kolm amprit ja muudab kogu saadud võimsuse radiaatoril soojuseks.

Ta on olemas allikate testimiseks. Ilma koormuseta näitab iga toiteplokk ilusat 12,00 V. Huvitav on
hoopis see, mida ta näitab kolme ampri juures, kas ta viie juures kaitsesse läheb ja mis temast
tunni pärast saab. Akude ja akupankadega on sama lugu: sildil olevad milliampertunnid ja tegelikud
on tihti eri arvud, ja koormus loeb need kokku.

Seadmel ei ole nime. Plaadil ei ole mudelit ega seerianumbrit, ainult tootmiskood, nii et
kasutusjuhendit ei ole mõtet otsida — kõik, mida ta oskab, on siin kirjas.

## Tal on vaja oma toiteplokki

Paljud odavad koormused saavad toite samast allikast, mida nad mõõdavad. **See mitte.** Tal on vaja
oma toiteplokki, mis on temaga samas konteineris. Ilma selleta koormus sisse ei lülitu, ja see ei
ole rike, vaid nii ta ongi ehitatud.

## Nelja juhtmega mõõtmine

Koormus oskab mõõta pinget eraldi juhtmepaariga, otse allika klemmidel, mitte oma sisendis. Vahe
paistab suurte voolude juures: viie ampri juures on pingelang tavalistel juhtmetel mõni kümnendik
volti. Ilma nelja juhtmeta käivitub pinge järgi väljalülitus mujal, kui sa arvestasid, ja aku
mahtuvus tuleb valesti välja.

## Milleks see sobib

- Kontrollida, kas toiteplokk peab lubatud voolu vastu ja kui palju pinge seejuures langeb
- Mõõta elemendi, paki või akupanga tegelikku mahtuvust ampertundides ja vatt-tundides
- Lasta allikal koormuse all etteantud aja töötada ja vaadata, mis temast sai
- Leida vool, mille juures allika kaitse rakendub
- Tühjendada element soovitud pingeni enne hoiustamist või enne mõõtmist

## Kuidas kasutada

1. Võta koormus ja tema toiteplokk riiulil olevast konteinerist.
2. Ühenda toiteplokk koormuse külge.
3. Ühenda testitav allikas kruviklemmi, jälgides polaarsust. Kui mõõdad mahtuvust või kui
   väljalülituspinge on oluline, kasuta pinge mõõtmiseks eraldi juhtmepaari.
4. Sea vool ja väljalülituspiirid: pinge, voolu ja aja järgi. Liitiumelemendi puhul ei ole
   pingepiir valikuline — alla tema miinimumi tühjendamine tapab elemendi.
5. Lülita koormus sisse ja jälgi esimese poole minuti jooksul, et vool on see, mida sa küsisid.
6. Nulli ampertundide ja vatt-tundide loendurid enne uut mõõtmist, muidu liidad kellegi teise
   numbritele.
7. Lõpus lülita koormus välja, lase radiaatoril jahtuda ja pane kõik konteinerisse tagasi.

## Ohutus

- Koormus muudab võimsuse soojuseks. Radiaator ja ventilaatorist tulev õhk on kuumad ja see on
  normaalne.
- Ära kata ventilaatorit kinni ega pane koormust paberile, riidele või kitsasse karpi.
- 150 W on võimsuse, mitte voolu piir. Viis amprit kolmekümne voldi juures ongi juba piir.
- Polaarsus. Tagurpidi ühendamine ei tähenda „ei tööta", vaid suitsu.

## Ligipääs

Koormus on hackspace'i ruumis riiulil konteineris, seega on vaja hackspace'i ligipääsuga paketti.
Instruktaaži ei ole vaja.
