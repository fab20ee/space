---
title: "Signaaligeneraator Rohde & Schwarz SMIQ 03B"
seoDescription: "Rohde & Schwarzi SMIQ 03B vektorsignaaligeneraator Tallinna hackspace'is: 300 kHz – 3,3 GHz, tase −140 kuni +13 dBm, analoog- ja digitaalmodulatsioon."
specs:
  - { label: "Sagedusala",   value: "300 kHz – 3,3 GHz" }
  - { label: "Tase",         value: "−140 kuni +13 dBm, samm 0,1 dB" }
  - { label: "Sageduse samm", value: "0,1 Hz" }
  - { label: "Modulatsioon", value: "analoog (AM, FM, ΦM, impulss) ja vektor-I/Q" }
  - { label: "Väljund",      value: "50 Ω" }
---

Seade, mis annab raadiosignaali, mille sagedus, tase ja modulatsioon on täpselt teada. Teda on vaja
alati, kui katsetatakse vastuvõtupoolt: spektrianalüsaator näitab, mis eetris on, generaator laseb
sinna panna täpselt selle, mida sa mõtlesid.

Kõige olulisem ots on siin taseme alumine piir. Miinus sada nelikümmend dBm on signaal vastuvõtja
tundlikkuse piiril, ja just sellistel tasemetel selgub, kas sinu seade üldse midagi kuuleb.

## Milleks see sobib

- Mõõta vastuvõtja tundlikkust: anda signaal ja langetada taset, kuni vastuvõtt laguneb
- Katsetada filtrit või võimendit, andes sisendisse teadaoleva signaali
- Siluda raadiomoodulit, omades etaloni teadaoleval sagedusel
- Kontrollida, kas seade jääb kurdiks tugeva signaali kõrval naabersagedusel
- Anda moduleeritud signaal ja vaadata, mida trakt sellega teeb

## Mida meeles pidada

- **Generaatori väljund on õrn.** Sinna ei anta midagi väljastpoolt: ei saatjat, ei alalispinget
  ega antenni, mille peale indutseerub kellegi teise signaal. Kaitse on olemas, aga seda ei tasu
  katsetada.
- **Sea tase enne ühendamist**, mitte pärast. Seade mäletab eelmist seadistust ja see on tavaliselt
  +13 dBm, mida kellegi vastuvõtja üle ei pruugi elada.
- Pistikud ja üleminekud on [RF-konteineris](/et/seadmed/rf-tarvikud), seal on ka
  kalibreerimiskomplektid ja DC-blokk.

## Kuidas kasutada

1. Lülita sisse ja lase soojeneda — taseme täpsuse jaoks on sellel tähtsust.
2. Sea sagedus ja tase. Alusta madalast tasemest ja tõsta ülespoole, mitte vastupidi.
3. Lülita vajadusel sisse modulatsioon ja väljund eraldi nupust.
4. Mida välja tuli, saab kontrollida [RIGOLi
   spektrianalüsaatoriga](/et/seadmed/spektrianaluusaator-rigol-rsa3030n) või
   [tinySA-ga](/et/seadmed/kaasaskantav-spektrianaluusaator-tinysa-ultra).
5. Lõpus lülita välja väljund, siis seade.

## Ligipääs

Generaator asub hackspace'i ruumis, seega on vaja hackspace'i ligipääsuga paketti. Instruktaaži ei
ole vaja.
