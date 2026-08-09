# Screentime

Screenshotovi **Screen Time** ekrana sa iPhone-a. Služe kao dopunski izvor podataka
za pregled perioda (skill `fokus-period-review`) — Fokus app meri koliko je rada
odrađeno, ovaj folder meri **gde je otišlo vreme koje nije radno**.

## Struktura

```
Screentime/
  README.md            <- ovaj fajl (konvencija imenovanja i čitanja)
  2026-07/             <- jedan folder po mesecu, format YYYY-MM
    24-dnevni.png
    24-aplikacije.png
    26-dnevni.png
    _sazetak.md        <- tekstualni izvod iz slika tog meseca
  2026-08/
    ...
```

**Mesečni folder `YYYY-MM/`** je jedina obavezna stvar. Datum se izvodi iz imena
foldera + imena fajla; ako fajl nema datum u imenu, čita se sa same slike.

## Imenovanje fajlova

Preporučeno: **`DD-tip.png`** — dan u mesecu + tip ekrana.

| tip | šta je na slici |
|---|---|
| `dnevni` | Screen Time → Day: ukupno vreme za taj dan + satnica po satima |
| `aplikacije` | lista aplikacija sa vremenom po svakoj (top apps) |
| `nedeljni` | Week pregled: ukupno + prosek + dnevni barovi |
| `pickups` | broj podizanja telefona |
| `notifikacije` | broj notifikacija |

Primeri: `24-dnevni.png`, `24-aplikacije.png`, `24-aplikacije-2.png` (druga slika
istog tipa istog dana, kad se lista ne vidi na jednom ekranu).

**Sirova iPhone imena (`IMG_1234.PNG`) su dozvoljena.** Claude tada čita datum i
tip direktno sa slike i predloži preimenovanje — ali ništa ne preimenuje bez
odobrenja.

**Važno kod `dnevni` i `nedeljni` ekrana:** Screen Time po defaultu prikazuje
*današnji/tekući* period. Ako je screenshot napravljen 26. za 25., datum na slici
je merodavan, ne datum kad je slikano.

## `_sazetak.md` — obavezan pratilac slika

Pravilo iz korenskog README-a: uz svaku sliku ide tekstualni sažetak, da se
originali ne otvaraju u svakoj sesiji. Slike su skupe za čitanje; tabela nije.

Jedan `_sazetak.md` po mesečnom folderu, sa tabelom:

```markdown
# Screentime — 2026-07

| Datum | Ukupno | Top aplikacije (min) | Pickups | Notif. | Izvor |
|---|---|---|---|---|---|
| 2026-07-24 | 4h 12m | Instagram 78, YouTube 55, WhatsApp 24 | 96 | 210 | 24-dnevni.png, 24-aplikacije.png |
| 2026-07-25 | 2h 40m | YouTube 61, Instagram 33 | 71 | 180 | 25-dnevni.png |

Napomene:
- 26.07. nema podataka (nije slikano).
```

Pravila za sažetak:

- Jedan red = jedan dan. Dan koji nije slikan **se ne izmišlja** — ili se izostavi
  iz tabele, ili se napiše "nema podataka" u Napomenama.
- Vremena u tabeli u minutima za aplikacije, `Xh Ym` za ukupno.
- Kolona `Izvor` mora da pokazuje na stvarno postojeće fajlove — po njoj se
  proverava da li je sažetak zastareo u odnosu na slike u folderu.
- Kad se dodaju nove slike, sažetak se dopunjuje **u istoj sesiji**. Sažetak koji
  kasni za slikama je gori od nepostojećeg, jer se u njega veruje.

## Kako se ovi podaci koriste u pregledu

`fokus-period-review` čita ovaj folder kao dopunu Fokus podacima. Screentime nije
sam po sebi cilj — koristan je isključivo kao **objašnjenje** onoga što Fokus
podaci pokažu:

- Rupa u radnom danu + visok telefon u tom istom prozoru → gde je vreme otišlo.
- Visoko večernje korišćenje (posle ~23h) → objašnjava propao jutarnji blok
  sledećeg dana.
- Pickups kao mera prekida: mnogo podizanja tokom radnih blokova znači isečene
  sesije, čak i kad je ukupan broj minuta u Fokusu pristojan.

Ono što se **ne** radi: screentime se ne pretvara u zaseban cilj ("smanji telefon
na X sati") osim ako plan po kome se sudi to eksplicitno traži.

## Privatnost

Screenshotovi mogu da sadrže imena kontakata i naslove notifikacija. Ako se slika
deli ili opisuje, imena osoba se ne prepisuju u tekst — dovoljno je "poruke" ili
"društvene mreže".
