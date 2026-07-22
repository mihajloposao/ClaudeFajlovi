# Profil — ko je Mihajlo

## Osnovno

- **Mihajlo Jovičić**, student **FON-a** (Fakultet organizacionih nauka, Beograd).
- Email: mihajlojovicic2205@gmail.com
- GitHub: **mihajloposao** (repoi: `ClaudeFajlovi` — ovaj folder, `fokus`)
- Radi na Windows-u, koristi Claude Cowork sa ovim folderom kao trajnom memorijom.
- Piše i razgovara na **srpskom**.

## Studije

Aktuelni ispiti (letnji rokovi 2026):

| Predmet | Skraćenica | Status / napomena |
|---|---|---|
| Operaciona istraživanja 1 | OI1 | Najveći teret. **Zadaci nisu problem, teorija jeste.** Pismeni + usmeni. |
| Numerička analiza | Numerička | Samo teorija; deo gradiva već pređen. Lakša od OI teorije. |
| Veštačka inteligencija | VI | **Prošli put pao zbog vremena, ne znanja** → brzina se trenira pod satom od prve nedelje. |
| Programski jezici 2 | PJ2 | Samo drugi deo; teži prvi deo već položen, ima gotov metod. Najmanje brige. |
| Finansijska matematika i rizik | FMiR | "Čist višak" — teži, manje ESPB, nekritičan. Prvi ispada čim nešto zaostane. |

## Kako radi (obrasci koje vredi znati)

- **Zna svoj glavni neuspešan obrazac:** kreće maksimalno → stane → počinje
  ispočetka. Zato planovi namerno kreću od minimuma i skaliraju naviše tek kad
  se pokaže da drže. Ne predlagati mu "sve odjednom od sutra".
- **Meri proces, ne ishod.** Ciljevi su mu formulisani kao merljivi međukoraci
  (streak treninga, "sve gradivo pređeno bar jednom do 9.8"), jer ishod ne
  kontroliše u potpunosti.
- **Gradi alate koje sam koristi.** Fokus i Helthy nisu vežbe iz programiranja
  nego aplikacije koje mu svakodnevno rade posao — pa mu je bitna pouzdanost
  (npr. tajmer koji preživi refresh), ne elegancija koda.
- **Ima definisan minimum za loše dane** za svaku naviku, da stvar preživi lošu
  nedelju umesto da pukne.
- **Sve što gradi ima i "AI ulaz"** — Fokus ima REST endpointe baš zato da Claude
  može da čita i upisuje podatke (vidi skillove `fokus-period-review` i
  `fokus-upis-podataka`).

## Tehnički stack i navike

- **Frontend:** plain HTML + CSS + vanilla JavaScript, bez frameworka i build alata.
  PWA (manifest + service worker), "Add to Home Screen" na telefonu.
- **Backend / baza:** Supabase (PostgreSQL + PostgREST RPC funkcije).
- **Za veće projekte:** Python (FastAPI) + React Native.
- **Deploy:** Netlify / Vercel, bez build komande.
- **Vizuelni identitet:** "Ink + Paper" — deljen između Fokusa i Helthy-ja.
- Verzionisanje PWA keša: ručno povećavanje verzije u `service-worker.js`.

## Duži planovi

- **Master u Sloveniji** — **oktobar 2028** (ranije se računalo na 2027).
  Slovenački jezik se sigurno uči i nastava će najverovatnije biti na
  slovenačkom; jezik nije prioritet sada, nego kreće posle rokova.
  Detalji: [`../Slovenija/README.md`](../Slovenija/README.md)
- **Motiv brend** — ideja u pauzi do posle ispita.
