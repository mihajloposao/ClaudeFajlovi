# Dnevnik rada

Hronologija sesija sa Claude-om: šta je urađeno, šta je odlučeno, šta ostaje.
Novi unosi idu **na vrh**. Kratko — detalji žive u fajlovima projekata.

## 22.07.2026 (sreda)

- **Nov folder `Slovenija/`** — istraživanje za master u Sloveniji (cilj oktobar
  2027): troškovi života po gradovima, smeštaj, uporedna analiza IT master
  programa, i kako radi prijava preko eVŠ. Pregled u
  [`../Slovenija/README.md`](../Slovenija/README.md).
- **Tri nalaza koja menjaju planiranje:**
  1. Redni master je **besplatan** za državljane Srbije, ali **nema prava na
     subvencionisan studentski dom** — smeštaj je puna cena.
  2. **Jezik je glavni filter.** UL FRI i UM FERI predaju na slovenačkom.
     Potpuno na engleskom: UP FAMNIT Koper, IPS Jožef Stefan, UL EF.
  3. Prijava za master **nije lista želja** — svaki fakultet vodi svoj postupak
     sa svojim rokom, a rokovi za ne-EU kandidate su često raniji.
- **Otvorena odluka:** da li se uči slovenački do 2027. Sa B2 se otvara FRI,
  bez njega FAMNIT je primarni cilj. Učenje je i dalje odloženo do posle rokova.
- Ništa nije menjano u planu za ispitni period — Slovenija je posle rokova.

## 19.07.2026 (nedelja)

- Napravljen i testiran Claude skill **`radni-kontekst`** — automatski učitava ovaj
  folder na početku sadržajnog rada, sinhronizuje ga sa GitHub-om, štedi usage
  (pita pre analize PDF-ova/slika) i na kraju rada beleži napredak nazad.
  Testiran na 3 scenarija: 12/12 provera prošlo, protiv 6/12 bez skilla.
- **Popravljena memorija:** `memorija.md` je ranije bio prepisan sadržajem "Test";
  vraćen pravi sadržaj i lokalno usklađeno sa GitHub-om.
- **Folder popunjen kontekstom** — dodati: `profil.md`, `stil-komunikacije.md`,
  ovaj dnevnik, `Planovi/Faks/ispiti-rokovi.md`,
  `Planovi/Generalni planovi/plan_14jul-23avgust_sazetak.md`,
  `Projekti/pregled-projekata.md`, `Projekti/Samo zapisi/ideje-backlog.md`,
  `Zdravlje/ciljevi-i-navike.md`.
  Sažeci su napravljeni namerno: PDF plana i slika rasporeda više ne moraju da se
  otvaraju u svakoj sesiji.
- Napomena: danas je **dan nedeljnog pregleda (19–20h)** po planu 14.7–23.8.

## Ranije (bez tačnog datuma)

- **Košarkaški menadžer:** MVP funkcionalno zaokružen (backend rute + svih 5
  ekrana + cela petlja). Ostaju dizajn i sitnice iz backloga.
- **Helthy** izdvojen iz Fokusa u zaseban projekat, deli isti Supabase backend.
- **Fokus** dobio REST endpointe za čitanje i upis, da Claude može direktno da
  radi sa podacima.
