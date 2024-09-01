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
- **Kasutamine**: Vaatame näiteid `unittest` kasutamisest.


# Pytest

**Pytest** on populaarne ja paindlik testimisraamistik Python'i keeles, mis lihtsustab testide loomist ja käivitamist. See pakub mitmeid võimsaid funktsioone, et aidata arendajatel kirjutada ja hallata teste efektiivselt.

## Põhiomadused

- **Lihtne Kasutamine**: Pytest on tuntud oma lihtsa ja selge süntaksi poolest, mis muudab testide kirjutamise intuitiivseks ja kiireks.
- **Täiendav Tugi**: Toetab mitmeid testimismeetodeid, sealhulgas üksikteste, integratsiooniteste ja jõudlusteste.
- **Täpne Vigade Raporteerimine**: Pakub üksikasjalikke ja selgeid vigade aruandeid, mis aitavad kiirelt leida ja parandada probleeme.
- **Kohandatavus**: Pytest võimaldab testide käitumist kohandada ja laiendada pluginate ja konfigureerimise kaudu.
- **Automatiseerimine**: Automatiseeritud testide käivitamine ja koodi katvuse mõõtmine on lihtne ja mugav.

## Miks on see oluline?

- **Tõhus Testimine**: Pytest muudab testimise tõhusaks, isegi suurte ja keerukate koodibaaside korral.
- **Koodikvaliteet**: Regulaarne testimine aitab tagada koodi kvaliteedi ja töökindluse.
- **Kiirem Arendus**: Automaatsete testide abil saab kiiremini avastada ja parandada vigasid, mis kiirendab arendusprotsessi.
- **Paindlikkus**: Pytest toetab erinevaid testimisstrateegiaid ja -meetodeid, andes arendajatele paindlikkuse testimisprotsesside kohandamisel.

## Testimise meetodid

Pytest pakub laia valikut testimismeetodeid:
- **Ühiktestid** – Testivad üksikute funktsioonide ja koodilõikude tööd.
- **Integratsioonitestid** – Kontrollivad, kuidas erinevad süsteemi osad koostöös töötavad.
- **Jõudluse testid** – Hinnatakse rakenduse jõudlust ja efektiivsust.
- **Turvalisuse testid** – Uurivad turvavea ja haavatavuste olemasolu.
- **Süsteemi testid** – Testivad kogu süsteemi funktsionaalsust ja integreeritust.

## Pytest'i Kasutamine

- **Kuidas Alustada?**: Pytest'i installimine ja kasutamine on lihtne. Seda saab paigaldada Python'i pakihalduri `pip` abil.
- **Näide**: Vaatame näiteid, kuidas luua ja käivitada lihtne test Pytest'iga.

```python
# test_example.py
def test_sum():
    assert 1 + 1 == 2
```

```python
import unittest

# Funktsioon, mida testime
def add(a, b):
    return a + b

# Testide klass kasutades unittest raamistiku
class TestAddFunction(unittest.TestCase):

    def test_add_integers(self):
        self.assertEqual(add(1, 2), 3)

    def test_add_strings(self):
        self.assertEqual(add('a', 'b'), 'ab')

if __name__ == '__main__':
    unittest.main()

```

```python
# Funktsioon, mida testime
def subtract(a, b):
    return a - b

# Testide funktsioon kasutades pytest raamistiku
def test_subtract():
    assert subtract(5, 3) == 2
    assert subtract(10, 5) == 5
    assert subtract(0, 0) == 0

```

```python
# Funktsioon, mida testime
def multiply(a, b):
    return a * b

# Lihtne assert avaldus, mis kontrollib tulemusi
assert multiply(2, 3) == 6
assert multiply(5, 0) == 0
assert multiply(-1, 5) == -5

```
