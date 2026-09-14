---
title: "SDR-transiiver HackRF One"
seoDescription: "Tarkvaraline raadio HackRF One Tallinna häkiruumis: vastuvõtt ja saatmine 1 MHz kuni 6 GHz, kuni 20 MHz ribalaius, GNU Radio ja SDRangel. Avatud 24/7."
specs:
  - { label: "Sagedusvahemik", value: "1 MHz – 6 GHz" }
  - { label: "Töörežiim",      value: "pooldupleks — kas vastuvõtt või saatmine, mitte korraga" }
  - { label: "Ribalaius",      value: "kuni 20 Msps, 8-bitised I/Q proovid" }
  - { label: "Antenniport",    value: "SMA (emane), 50 Ω, piitsantenn kaasas" }
  - { label: "Taktimine",      value: "CLKIN ja CLKOUT, 10 MHz, välise etaloni ja sünkroonimise jaoks" }
  - { label: "Ühendus",        value: "micro-USB 2.0, toide sama kaabli kaudu" }
  - { label: "Tarkvara",       value: "GNU Radio, SDRangel, GQRX, SDR#, hackrf käsurea tööriistad" }
  - { label: "Litsents",       value: "avatud riistvara — skeemid ja püsivara on avalikud" }
---

Vastuvõtja ja saatja, mille signaalitöötlus käib peaaegu tervenisti arvutis oleva tarkvaraga.
Riistvara üksnes nihutab valitud osa eetrist baassagedusele ja saadab proovide voo USB kaudu —
mis nendega edasi saab, otsustab programm. Sama karp on täna lennuside vastuvõtja, homme sinu enda
anduri telemeetria dekooder ja ülehomme jäme ülevaatlik skanner kuni 6 GHz-ni. Vahemik katab
enamiku sellest, millega tavaliselt kokku puutud: pikklained, UKW, 433 ja 868 MHz, 2,4 GHz.

See on raadio õppimise ja oma seadmete silumise tööriist, mitte mõõteriist: signaalitee ei ole
kalibreeritud ja tasemed on ligikaudsed. Kui vaja on täpseid numbreid, seisab kõrval
spektrianalüsaator Rigol RSA3030N.

## Mida saab teha

- Kuulata eetrit ja vaadata vesilangust: ringhääling, lennuside, amatöörsagedused.
- Võtta vastu ja lahti võtta oma seadme pakette 433 või 868 MHz peal — andur, pult, LoRa-moodul.
- Püüda ADS-B lennukitelt, NOAA ilmasatelliitidelt, pakette ilmajaamadelt.
- Salvestada signaal faili ja võtta see hiljem GNU Radios lahti, riistvarast sõltumata.
- Vaadata sagedusala kiiresti üle käsuga `hackrf_sweep`, et näha, kus üldse midagi toimub.
- Ehitada ja katsetada oma vastuvõtjat või saatjat GNU Radios, ilma plaati tegemata.

## Kuidas kasutada

1. Keera antenn **ANT** pesasse käega, ilma võtmeta. Ilma antenni või koormuseta saata ei tohi.
2. Ühenda micro-USB kaabel arvutiga. Toide tuleb sama kaabliga, eraldi adapterit ei ole.
3. Kontrolli, et seade on näha: `hackrf_info`. Käsk näitab seerianumbrit ja püsivara versiooni.
4. Käivita SDRangel, GQRX või oma GNU Radio skeem ning määra sagedus ja ribalaius.
5. Tõsta võimendust järk-järgult. Kui vesilangusel tekivad sama signaali koopiad mitmel sagedusel,
   on sisend üle koormatud — võta võimendust maha, mitte juurde.
6. Lõpetuseks sulge programm, eemalda kaabel ning pane antenn ja punased korgid tagasi.

Esipaneeli tuled: **3V3** ja **1V8** on toitepinged, **USB** on side arvutiga, **RF** tähendab, et
raadioosa töötab, **RX** ja **TX** näitavad vastuvõttu või saatmist. Nupp **RESET** käivitab seadme
uuesti, **DFU** on ainult püsivara vahetamiseks — muidu ära seda vajuta.

## Oluline

- **Saatmine ei ole lihtsalt üks funktsioon veel.** Eetrisse tohib minna kas litsentsivabades
  sagedusalades, järgides võimsuse ja kanali hõivatuse piiranguid, või amatöörraadio loa alusel.
  Eestis tegeleb sellega Tarbijakaitse ja Tehnilise Järelevalve Amet (TTJA). Vastutus on sellel,
  kes vajutas saatmise nuppu.
- **Väljund ei ole filtreeritud.** Saatetee on lairibaline ilma väljundfiltriteta, harmoonikud on
  tugevad. Isegi kui kandesagedus on lubatud alas, ulatub kiirgus sellest välja. Saatmiskatseteks
  kasuta antenni asemel koormustakistit.
- **Ära sega teiste seadmeid.** WiFi, mobiilside, autovõtmed, hädaabiteenused ja GPS ei ole
  katsepolügoon. Nende häirimine on kriminaalasi, mitte majasisene küsimus.
- **Sisend on õrn.** Ära anna antenniporti üle −5 dBm ja ära ühenda seda kunagi otse saatja
  väljundiga — vaja on nõrgendit. Alalispinget sisendis seade samuti ei talu.
- **Antenniport võib anda toidet** (tarkvaraliselt lülitatav bias tee). Enne võõra aktiivantenni või
  võimendi ühendamist veendu, et see on välja lülitatud.
- Pikal saatmisel seade soojeneb. See on normaalne, aga ära kata seda kinni.

## Ligipääs

Seade seisab häkiruumi mõõtelaual, seega on vaja häkiruumi avavat paketti. Enne esimest kasutamist
tuleb lühike juhendamine: mida tohib kuulata (kõike) ja mida tohib saata (ettevalmistuseta väga
vähe). Ruumist välja seda ei anta.
