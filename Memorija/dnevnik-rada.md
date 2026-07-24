# Dnevnik rada

Hronologija sesija sa Claude-om: šta je urađeno, šta je odlučeno, šta ostaje.
Novi unosi idu **na vrh**. Kratko — detalji žive u fajlovima projekata.

## 24.07.2026 (petak) — Kriza plana + novi sistem rada

- **Povod:** plan 14.7–23.8 je stao — prvih ~10 dana neujednačeno, pa 21–24.7
  potpuna tišina u Fokusu. Povučeni Fokus podaci i planovi; kroz razgovor se došlo
  do uzroka i do sistema koji ga sprečava.
- **Pravi uzrok (ne lenjost):** anticipatorna anksioznost — pre podne strah od
  popodneva (nemir kod kuće, van kontrole) → zamrzavanje → grabljenje dopamina
  „sad ili nikad" → popodne propadne uz krivicu → sutradan se strah potvrdi. Uz to
  obrazac „kreni maksimalno pa stani" i beg energije u projekte (6,5h na
  StartingFive prvog dana plana).
- **Novi dokument** `Planovi/Generalni planovi/sistem-rada.md` — lični sistem
  rada: tri prozora (jutro nosivi / popodne oportuno / veče bonus), blok
  (vreme = granica, cilj = kompas), stepenovani minimum po oceni dana
  (dobar/onako/loš), odmor sa dve kočnice (pod + ivica/tajmer), kritična stanja →
  potez, re-entry posle pada, nedeljni pregled. Drži pravila, ne sate — konkretne
  brojke i planove postavlja Mihajlo sam.
- **Izmenjen zakazani zadatak `fokus-weekly-review`:** sada traži kritične momente
  (zašto dolazi do pada) i prolazi ih s Mihajlom; meri output, ne samo minute.
- **Otvorena tema:** strah od napretka (pad odmah posle dobrih dana) i osećaj
  „napredak ili mir". Sistem je namerno građen da napredak može da živi pored mira,
  ne kao rat.

## 22.07.2026 — Kupovina laptopa (istraživanje i strategija)

- Kroz više krugova pitanja utvrđeni parametri kupovine i napravljen plan.
  Sve zapisano u novom folderu **`Planovi/Kupovina/Laptop/`** (README + plan +
  način razmišljanja + izvori/praćenje).
- **Ključna odluka:** kupiti **krajem 2028 u Sloveniji, kao student** — poklapa se
  sa OLED redizajnom (M7 Air, 2028) i studentskim popustom + EU garancijom.
  Trenutni desktop pokriva period do tada; ako se preseli ranije, pomera se unapred.
- **Favorit:** MacBook Air **24GB** (RAM > generacija čipa za horizont 2027–2031).
  Ne-Apple (Zenbook S14 OLED 32GB / ThinkPad T14 nadogradiv) samo ako pobeđuje u
  RAM-u/nadogradivosti/ceni/ekranu.
- **Princip biranja:** troši na nepromenljivo (RAM, storidž, ekran, izrada),
  štedi na neosetnom (generacija čipa).
- **Tržišni nalazi (jul 2026):** M5 Air izašao mart 2026; M6 (~mart 2027)
  evolutivan i skuplji; OLED (M7) 2028/2029. Za Apple je Srbija cenovno na nivou
  EU — put se ne isplati osim studentskog statusa 2028.
- **Postavljen zakazani zadatak** `nedeljna-analiza-laptop-trzista` (ponedeljkom
  u 8h): analiza srpskog tržišta sa tri kategorije preporuka (iznad budžeta /
  do budžeta / znatno jeftinije) + događaji za pratiti + preporuka nedelje.

## 22.07.2026 (sreda)

- **Nov folder `Slovenija/`** — istraživanje za master u Sloveniji: troškovi
  života po gradovima, smeštaj, uporedna analiza IT master programa, i kako radi
  prijava preko eVŠ. Pregled u
  [`../Slovenija/README.md`](../Slovenija/README.md).
- **Dve odluke potvrđene u razgovoru:**
  - **Učenje slovenačkog je zagarantovano**, nastava na masteru najverovatnije
    na slovenačkom. Time jezik prestaje da bude filter i **UL FRI i UM FERI
    postaju primarni ciljevi** umesto FAMNIT-a.
  - **Upis pomeren sa 2027 na oktobar 2028.** Dobija se dodatna godina za jezik
    i za pripremu izbirnog izpita za FRI.
- **Tri nalaza koja menjaju planiranje:**
  1. Redni master je **besplatan** za državljane Srbije, ali **nema prava na
     subvencionisan studentski dom** — smeštaj je puna cena.
  2. UL FRI ima obavezan **izbirni izpit** (matematika, programiranje,
     algoritmi, računarski sistemi) — to je glavni filter, priprema se unapred.
  3. Prijava za master **nije lista želja** — svaki fakultet vodi svoj postupak
     sa svojim rokom, a rokovi za ne-EU kandidate su često raniji.
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
