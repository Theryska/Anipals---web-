# AniPals — web

Web pro AniPals: hlídání mazlíčků s ověřenými hlídači po celé ČR.
Pět propojených stránek (záložek) se stejným designem podle stránky Domů.

## Obsah

- `index.html` — Domů
- `sluzby.html` — Služby
- `jak-to-funguje.html` — Jak to funguje
- `cenik.html` — Ceník/Storno podmínky (**zatím jen struktura** — ceny a znění
  storno podmínek si doplňte, místa k doplnění jsou v textu jasně označená)
- `caste-dotazy.html` — Časté dotazy
- `css/style.css` — společný vzhled všech stránek (barvy, layout, responzivita)
- `js/script.js` — mobilní menu, drobné doplňky
- `assets/` — místo pro obrázky/logo (zatím prázdné, logo je zatím jen SVG přímo v HTML)

## Nasazení na Cloudflare Pages (přes Git)

1. Nahrajte tuto složku do nového repozitáře na GitHubu.
2. V Cloudflare Dashboardu: **Workers & Pages → Create → Pages → Connect to Git**.
3. Vyberte repozitář. Jako **build command nechte prázdné** a **output directory
   nastavte na `/`** (kořen repozitáře) — žádný build krok tu není potřeba,
   jde o čistý statický web.
4. Deploy. Po dokončení dostanete adresu `*.pages.dev`, ke které lze později
   připojit vlastní doménu (Cloudflare Pages → Custom domains).

Jakákoli další změna v repozitáři na GitHubu se po pushnutí automaticky
znovu nasadí.
