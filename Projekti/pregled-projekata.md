# Pregled projekata

**Statusi na dan 19.07.2026. Svi projekti su u pauzi do kraja ispitnih rokova** —
Fokus i Helthy se koriste svakodnevno, ali se nove funkcionalnosti ne razvijaju.

## Fokus — planiranje dana tokom rokova

`Projekti/Celi projekti/fokus/` · GitHub: `mihajloposao/fokus` · **PAUZA (koristi se)**

Lična PWA za praćenje dnevnog rasporeda učenja. Jednokorisnička, plain HTML/CSS/JS,
bez frameworka. Ekrani: Danas, Plan, Istorija, Detalj dana.

- **Najvažniji deo — tajmer:** pri startu se upisuje tačan timestamp početka, a
  proteklo vreme se uvek računa kao `sada − start`. Zato refresh ili zatvaranje
  taba ne gube ništa. Svaki start→stop par je posebna sesija.
- **Podaci:** Supabase, ključ `fokus-planovi` (dnevni objekti).
- **AI pristup:** `supabase-izvestaj.sql` (čitanje) i `supabase-dodavanje.sql`
  (upis: obrok, kilaža, trening, obaveza, stavka sa ciljem) — POST RPC endpointi
  koje koriste skillovi `fokus-period-review` i `fokus-upis-podataka`.
- Deploy: Netlify/Vercel bez build komande. Za svaku izmenu povećati verziju keša
  u `service-worker.js`.

## Helthy (Kilaža & Trening)

`Projekti/Celi projekti/Helthy/` · **PAUZIRAN do septembra 2026**

Izdvojen iz Fokusa: Fokus je ostao samo za planiranje dana, a kilaža/trening/obroci
žive ovde. Ekrani: Kilaža, Treninzi, Detalj treninga.

- Kilaža: dnevni unos, grafik trenda sa 7-dnevnim prosekom, ciljna kilaža sa
  trakom napretka.
- Obroci: kalorije i makroi po obroku, dnevni zbir (na Kilaža ekranu).
- Treninzi: naziv, termin, težina sesije (1–5), vežbe, beleška.
- **Deli backend sa Fokusom** — isti Supabase projekat i ključevi. `kilaza-trening`
  je samo njegov; `fokus-planovi` deli sa Fokusom (`dan.treninzi`, `dan.obroci`).
  Sinhronizacija je "poslednji upis pobeđuje" — konflikt je moguć samo ako se
  isti dan menja u obe aplikacije istovremeno.

## Košarkaški menadžer (igra)

Nije u ovom folderu — živi u zasebnom projektu na računaru. **PAUZA · MVP zaokružen**

Python **FastAPI** backend + **Supabase** + **React Native** frontend.

- **Backend rute:** health, `/create-team` (sa `is_ai`), `/team/{id}` (tim + igrači),
  `POST /team/{id}/starters` (validacija 5 igrača + pozicije), `/play-random`
  (random protivnik, snima meč, ažurira `wins/losses`), `/history`.
- **Frontend — cela petlja radi:** Napravi tim → Dashboard → Postava (izbor
  petorke) → Meč/Box score → Istorija, uz pamćenje tima i osvežavanje pri fokusu.
- **Poznate sitnice (nijedna nije blokada):** moral se ne menja posle meča (stoji
  na 70); frontend nema `try/catch` na `fetch`-u pa ekran može zauvek stajati na
  "Učitavam…"; box score prikazuje svih 10 igrača nerazdvojeno po timovima;
  `get_random_opponent_id` ne filtrira `is_ai`; legacy rute `/match` i `/play`
  su ostale.
- **Sledeće kad se vrati:** dizajn/izgled ili neka od gornjih sitnica.

## Motiv (brend)

Ideja, **pauzirana do posle ispita**. Nema fajlova u folderu.

## Claude skillovi

Van ovog repoa (instalirani u Cowork-u), ali deo iste priče:
`radni-kontekst` (ovaj folder), `fokus-period-review`, `fokus-upis-podataka`,
`meal-nutrition-estimator`, `life-period-planner`, `project-planning-assistant`.
