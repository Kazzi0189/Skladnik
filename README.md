# Skladník PWA

Toto je instalační PWA verze aplikace Skladník.

## Nahrání na GitHub Pages

1. Vytvoř na GitHubu nový repozitář, například `skladnik-pwa`.
2. Nahraj do něj všechny soubory z této složky:
   - `index.html`
   - `manifest.webmanifest`
   - `sw.js`
   - složku `icons`
   - `.nojekyll`
3. V GitHubu otevři **Settings → Pages**.
4. V části **Build and deployment** nastav:
   - Source: **Deploy from a branch**
   - Branch: **main**
   - Folder: **/root**
5. Po uložení GitHub zobrazí adresu aplikace.

## Instalace do mobilu

### Android / Chrome

1. Otevři adresu GitHub Pages v Chrome.
2. V menu prohlížeče zvol **Přidat na plochu** nebo **Nainstalovat aplikaci**.
3. Aplikace se zobrazí mezi aplikacemi v mobilu.

### iPhone / Safari

1. Otevři adresu v Safari.
2. Klepni na sdílení.
3. Zvol **Přidat na plochu**.

## Poznámka

Skenování kódů a mikrofon v mobilu vyžadují HTTPS. GitHub Pages HTTPS poskytuje automaticky, takže je pro tuto aplikaci vhodný.
