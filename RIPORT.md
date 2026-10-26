# A dékáni hivatal „működő” kapcsolati űrlapja – hibariport

Repó: https://github.com/<bako-adam31>/umfst-bh01-kapcsolati-urlap
Készítette: <Bako Adam-Attila>, <INFO LM>

## 1. hiba
- **Hiba leírása és reprodukálása (lépések, böngésző, segédtechnológia):** 
A javitott HTML kodot a W3C Markup Validation Service ellenoriztem. A validacio soran ellenoriztem, hogy a hozzaadott `<label>` elemek, valamint a `for` es `id` attributumok szintaktikailag helyesek-e.
- **Gyökérok (melyik sor, melyik szabály sérül):** 
Az `index.html` 15–20. soraiban a form beviteli mezoi (`<input>`, `<select>`, `<textarea>`) nem rendelkeztek hozzajuk tartozo `<label>` elemmel, kizarolag `placeholder` attributum volt megadva. 
- **Javítás (commit link, előtte/utána kódrészlet):** 
*Commit link:* https://github.com/bako-adam31/umfst-bh01-kapcsolati-urlap/commit/d0fc6bb6ea4df93882fa7f9c650b367852ed2069
- **Hogyan tesztelted (W3C validátor, Lighthouse, Tab-bejárás, képernyőolvasó):** 
A javitott HTML kodot atfuttattam a W3C Markup Validation Service-en; a form szerkezete és a hozzaadott for/id attributumok hiba és figyelmeztetes nelkul átmentek.


- **Tanulság / érintett alapelv (pl. Szemantika előbb, stílus később; WCAG-kritérium):** 
A placeholder attributum nem helyettesiti a szemantikus `<label>` elemet. A placeholder csupan kiegeszito minta megadasara valo, gepeleskor eltunik, igy a kepernyoolvasok elveszitik a mezo kontextusat.
*Alapelv*
Szemantika elobb – az akadalymentesites alapja a helyes, szabvanyos HTML szerkezet (for + id), nem a vizualis trukkok.


## 2. hiba
- **Hiba leírása és reprodukálása (lépések, böngésző, segédtechnológia):** 
Devtool sagitsegevel latszott hogy a `.cim` el van irva
- **Gyökérok (melyik sor, melyik szabály sérül):** 
a `style.css` 3. sora volt serult `color` helyett `colour` eliras volt
- **Javítás (commit link, előtte/utána kódrészlet):** 
*Commit link:* 
- **Hogyan tesztelted (W3C validátor, Lighthouse, Tab-bejárás, képernyőolvasó):** 
Frissites utan eltunt a hiba es a cim is mar zolden jelent meg
- **Tanulság / érintett alapelv (pl. Szemantika előbb, stílus később; WCAG-kritérium):** 
A bongeszo nem ad hibat elgepelt css tulajdonsagoknal ezert a Devtoolban ellenorizheto az elgepeles
