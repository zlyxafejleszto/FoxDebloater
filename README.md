# FoxDebloater 🦊🚫

A **FoxDebloater** egy agresszív, rendszerszintű Windows Registry optimalizáció, amelynek célja a Firefox teljes megtisztítása a telemetriától, a bloatware-től és a felesleges háttérfolyamatoktól. 

Míg a legtöbb megoldás csak profil szinten (`user.js`) babrál, a FoxDebloater a Windows Group Policy (GPO) réteget használja. Ez garantálja, hogy a beállítások **felülírhatatlanok** maradnak a böngésző frissítései után is.

## 🔥 Főbb funkciók

*   **Zéró Telemetria:** Teljes körű adatgyűjtés-tiltás (Mozilla Studies, Crash Reporting, Default Browser Agent).
*   **UI Tisztítás:** Pocket, Screenshots, Firefox Accounts és minden "More from Mozilla" marketing elem végleges kiirtása.
*   **Adatvédelmi Hardening:** DNS-over-HTTPS kényszerítés, keresési javaslatok (keystroke logging) tiltása.
*   **Rendszerszintű perzisztencia:** A beállítások minden felhasználói profilra érvényesek és immunisak a böngésző alaphelyzetbe állítására.
*   **Maximális Sebesség:** Megszünteti a háttérben futó felesleges ellenőrzéseket és "ajánló" motorokat.

## 🚀 Telepítés

1. Töltsd le a `FoxDebloater.reg` fájlt.
2. Futtasd **rendszergazdaként**.
3. Hagyd jóvá a Registry módosítást.
4. Indítsd újra a Firefoxot.

## 🛠 Ellenőrzés

Nyisd meg a Firefoxot és írd be a címsorba:
`about:policies`

Ha a lista aktív, a rendszered **Managed** állapotban van: a FoxDebloater átvette az irányítást a telemetria felett.

## ⚖️ Jogi Nyilatkozat (Disclaimer)

A **FoxDebloater** használatával a felhasználó elismeri és elfogadja az alábbiakat:
*   **Saját felelősség:** A szkriptet mindenki saját felelősségére futtatja. A Windows Registry módosítása kritikus beavatkozásnak minősül.
*   **Garancia hiánya:** A szoftver "AS IS" (ahogy van) állapotban kerül közzétételre. Semmilyen kifejezett vagy hallgatólagos garancia nem vonatkozik a működésre vagy a hibamentességre.
*   **Felelősség korlátozása:** A készítő semmilyen körülmények között nem tehető felelőssé a szkript használatából eredő közvetlen vagy közvetett károkért (ideértve az adatvesztést, rendszerösszeomlást vagy bármilyen hardveres/szoftveres meghibásodást).

## 🔒 Felhasználási Feltételek és Licenc

Ez a projekt egyedi licenc alatt áll a szerzői jog védelme érdekében:

1.  **Személyes felhasználás:** Ingyenesen használható bármilyen magáncélú eszközön.
2.  **Megnevezés kötelezettsége:** A kód bármilyen részletének felhasználása, publikálása vagy bemutatása esetén az eredeti szerzőt (FoxDebloater Project) jól látható módon meg kell nevezni, és linkelni kell az eredeti forrást.
3.  **Továbbfejlesztés:** A kód módosítható, de a módosított változat csak akkor tehető közzé, ha az eredeti szerző megnevezésre kerül, és a módosított változat is ugyanezen feltételekkel (ingyenesen és megnevezéssel) marad elérhető.
4.  **Kereskedelmi felhasználás:** A kód vagy annak bármely részének árusítása, fizetős szoftverbe építése vagy bármilyen pénzügyi haszonszerzésre irányuló felhasználása szigorúan TILOS.
5.  **Visszaélés:** A projekt nevével vagy tartalmával való visszaélés, illetve sajátként való feltüntetése jogi következményeket vonhat maga után.

---
**Copyright © 2026 - FoxDebloater Project. Minden jog fenntartva.**
