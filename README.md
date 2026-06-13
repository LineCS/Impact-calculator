# SES Family – økonomisk model & metodevælger

Interaktiv beslutningsstøtte, der oversætter de dokumenterede effekter fra **SES ONE/CAD** og **SES NXT** til kroner — fordelt på aktører (kommune, region, stat, arbejdsplads, borger) og over tid.

Hele værktøjet er **én selvstændig HTML-fil** uden afhængigheder, build-trin eller netværkskald. Det kan åbnes direkte i en browser eller hostes gratis via GitHub Pages.

## Indhold

- `index.html` — hele modellen (HTML + CSS + JavaScript i én fil)

## Sådan åbner du den lokalt

Dobbeltklik på `index.html`, eller åbn den i en browser. Intet andet kræves.

## Sådan udgiver du den med GitHub Pages

1. Læg `index.html` i roden af et GitHub-repository (eller i en `docs/`-mappe).
2. Gå til **Settings → Pages**.
3. Under **Build and deployment → Source** vælg **Deploy from a branch**.
4. Vælg branch (fx `main`) og mappe (`/ (root)` eller `/docs`), og gem.
5. Efter et øjeblik er siden live på `https://<brugernavn>.github.io/<repo>/`.

## Hvad modellen gør

- **Metodevælger (CCA):** vælg en eller flere værdisætningsmetoder. Ingen beregning er slået til som standard — man vælger aktivt.
- **Populations- og adgangslag:** vælg kommune (auto-udfylder indbyggertal), estimér forventede brugere ud fra udbredelsesindsatsen, og vælg aktørperspektiv.
- **Økonomiske beregninger:** CCA-regnskab, effekt over tid (nutidsværdi ved 3,5 %), og fordeling på aktører.
- **Cost-effectiveness:** licens pr. produkt (ONE/NXT/PRO) + anslået udbredelsesudgift sættes op mod værdi pr. naturlig enhed, med business case pr. enhed, valg af scope (hele kohorten / 1 voksen / 1 barn) og en opsummeringsfunktion.

## Metode og forbehold

- Bygget på **SØM v3.4** (Social- og Boligstyrelsen), 2025-priser, og de publicerede SES-effektstudier.
- Modellen er en bevidst **konservativ cost-consequence-analyse** af direkte målte effekter. Statistisk usikkerhed er beskrevet i forskningen, ikke regnet ind i tallene.
- Business case-tal pr. enhed er **alternative nævnere** og må ikke lægges sammen — hver post forudsætter, at hele licensen retfærdiggøres af netop den effekt.
- Tallene er beslutningsstøtte, ikke en garanti, og afhænger af de valgte antagelser.

## Licens

Vælg selv en licens til repositoryet (fx via GitHub: **Add file → Create new file → `LICENSE`**). Indtil da betragtes indholdet som ophavsretligt beskyttet af rettighedshaver.
