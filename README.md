# Skladník PWA

Mobilní PWA aplikace pro skladovou kontrolu, skenování EAN, diktování a export inventury.

## Nahrání na GitHub Pages

1. Rozbalte ZIP.
2. Obsah složky `skladnik-pwa` nahrajte do kořene GitHub repozitáře.
3. V GitHubu otevřete **Settings → Pages**.
4. Zvolte **Deploy from branch**.
5. Branch: `main`, složka: `/root`.
6. Počkejte na vygenerování odkazu.
7. Otevřete odkaz v mobilu přes HTTPS a z nabídky prohlížeče zvolte instalaci aplikace.

## Důležité

- Kamera i mikrofon na mobilu vyžadují HTTPS. GitHub Pages HTTPS poskytuje automaticky.
- Skener je od této verze uložený lokálně v `vendor/html5-qrcode.min.js`, takže aplikace není závislá na CDN.
- Po nahrání nové verze může být potřeba v mobilu aplikaci jednou zavřít a znovu otevřít, aby service worker stáhl nové soubory.

## Co bylo opraveno ve verzi v2

- Automatické ukládání po ruční úpravě buněk v tabulce.
- Ošetření prohlížečů, které nepodporují hlasové diktování.
- Lokální knihovna skeneru místo načítání z internetu.
- Ochrana proti dvojitému spuštění skeneru.
- Lepší hláška při chybě kamery.
- Bezpečnější vytváření řádků tabulky přes `textContent` místo `innerHTML`.
- Bezpečnější export CSV s ošetřením uvozovek.
- Lepší import CSV včetně hodnot v uvozovkách.
- Při importu rozdělané práce volba nahradit/přidat.
- Zobrazení počtu viditelných řádků po filtrování.
