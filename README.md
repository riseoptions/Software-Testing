# Tarkvara testimine

**Tarkvara testimine** on protsess, mille käigus kontrollitakse, kas teatud koodiosad ja kogu rakendus toimivad soovitud viisil. Testimine hõlmab testide loomist ja käivitamist, et veenduda koodi õigsuses. Testid ei ole rakenduse osa, vaid sõltumatud kontrollpunktid.

## Miks on see oluline?

- **Väikeste Rakenduste Testimine**: Väikseid rakendusi on lihtne testida, lihtsalt neid käivitades.
- **Suuremate Koodibaaside Testimine**: Suuremate koodibaaside puhul muutub kõikide funktsioonide ja nende tulemuste testimine keerulisemaks.
- **Hea Praktika**: Iga kord, kui lisate uue funktsiooni, on soovitatav testida oma koodi.
- **Automatiseeritud Testimine**: Automatiseeritud testimine on oluline, et efektiivselt ja järjepidevalt testida suurt hulka koodi.

## Testimise meetodid

Erinevaid testimise meetodeid on palju. Siin on mõned levinumad:
- **Ühiktestid** – Keskendume sellele meetodile selles moodulis.
- **Integratsioonitestid**
- **Jõudluse testid**
- **Turvalisuse testid**
- **Süsteemi testid**
- Ja palju muud

## Ühiktestid

- **Põhiline Testimise Tüüp**: Ühiktestid on kõige põhilisemad, kuid samas väga võimsad.
- **Funktsiooni Testimine**: Need peaksid testima väikest koodilõiku, nagu funktsioon või selle osa.
- **Mitmekordne Testimine**: Funktsiooni või koodilõiku saab testida mitme erineva testiga.
- **Koodiharude ja Äärealade Testimine**: On tavaline proovida testida kõiki koodiharusid ja äärealasid.

## `unittest` – Sisseehitatud Testimisraamistik

- **Mis on `unittest`?**: `unittest` on Python'i sisseehitatud testimisraamistik, mis on mõeldud üksikute testide loomiseks.
- **Kasutamine**: Vaatame näidet `unittest` kasutamisest.
