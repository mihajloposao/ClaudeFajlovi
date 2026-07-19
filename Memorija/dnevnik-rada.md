# Dnevnik rada

Hronologija sesija sa Claude-om: šta je urađeno, šta je odlučeno, šta ostaje.
Novi unosi idu **na vrh**. Kratko — detalji žive u fajlovima projekata.

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
