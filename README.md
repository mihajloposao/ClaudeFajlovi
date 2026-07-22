# ClaudeFajlovi

Trajna baza konteksta za rad sa Claude-om (Cowork). Lokalno stoji u
`C:\Users\Mihajlo\Desktop\Claude`, a sinhronizuje se sa ovim repoom, pa je isti
kontekst dostupan i kad lokalni folder nije.

Čita ga i održava skill **`radni-kontekst`**: na početku sadržajnog rada učitava
ono što je relevantno, na kraju beleži napredak i pušuje izmene.

## Struktura

```
Memorija/          ko sam, kako radim, hronologija sesija
  memorija.md        <- POČNI ODAVDE: srž konteksta + linkovi na ostalo
  profil.md          detaljan profil: studije, stack, radni obrasci
  stil-komunikacije.md   kako Mihajlo voli da Claude odgovara
  dnevnik-rada.md    hronologija sesija (najnovije na vrhu)

Planovi/
  Faks/              raspored ispita (slika + tekstualna verzija)
  Generalni planovi/ lični planovi po periodima (PDF + sažetak)

Projekti/
  pregled-projekata.md   status svih projekata na jednom mestu
  Celi projekti/     izvorni kod (fokus, Helthy) — ugnježdeni git repoi
  Samo zapisi/       ideje i backlog

Zdravlje/            ciljevi forme, trening, ishrana, ritual

Slovenija/           master u Sloveniji (cilj okt 2027) — referentno, ne za
  README.md            svaku sesiju; počni od README.md
```

## Pravila

- **Ne brisati postojeću strukturu.** Dodavanje fajlova i foldera je u redu.
- Uz svaki veliki fajl (PDF, slika) ide i tekstualni sažetak, da se original ne
  mora otvarati u svakoj sesiji.
- Fajlovi u `Celi projekti/` su zasebni git repoi — njihovo git stanje se ne dira.
