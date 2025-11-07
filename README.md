# Starter blog gratuito (GitHub Pages + Jekyll)

## Come usarlo
1. Crea un account GitHub (se non l'hai già).
2. Crea un repository **pubblico**. Nome consigliato: `mattiadragoboardgames.github.io` (ma va bene anche un altro).
3. Carica *tutti* i file di questa cartella nel repo e fai commit su `main`.
4. Nelle impostazioni del repo vai su **Settings → Pages** e assicurati che la Source sia `GitHub Actions` o `Deploy from branch (main)`. Seleziona il tema preconfigurato **minima**.
5. Nel repo esiste un file `CNAME` già impostato su `www.mattiadragoboardgames.com`.
6. In Namecheap aggiungi i DNS:
   - **CNAME**: `www` → `USERNAME.github.io` (sostituisci USERNAME con il tuo utente GitHub).
   - **A records** (facoltativi, per usare anche il dominio nudo): punta `@` ai 4 IP di GitHub Pages (vedi documentazione GitHub).
7. Attiva **Enforce HTTPS** in Settings → Pages (GitHub genererà l'SSL gratis).
8. Scrivi post nella cartella `_posts` usando questo formato: `YYYY-MM-DD-titolo.md` con front matter Jekyll.

## Note
- I plugin inclusi (`jekyll-feed`, `jekyll-seo-tag`, `jekyll-sitemap`) sono supportati da GitHub Pages.
- I contenuti sono in Markdown. Le immagini mettile in `assets/` e linkale nei post.
- Per i commenti puoi integrare [Giscus](https://giscus.app) (gratuito) o Disqus (gratuito con pubblicità).