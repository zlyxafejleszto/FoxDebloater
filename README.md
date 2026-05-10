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

## ⚖️ Disclaimer / Felelősségkizárás

A szoftver használata csak saját felelősségre történik. A Registry módosítása nem megfelelő használat esetén rendszerhibákat okozhat. A készítő nem vállal felelősséget semmilyen adatvesztésért, hardveres vagy szoftveres kárért, amely a szkript használatából ered. 

**Figyelem:** Ez a konfiguráció biztonsági okokból tiltja a Firefox beépített jelszókezelőjét és a Sync funkciót. A telepítés előtt gondoskodj külső jelszókezelő (pl. Bitwarden) használatáról.

## 📜 Licenc és Felhasználás

Ez a projekt a **CC BY-NC-SA 4.0** licenc alatt áll.

*   **Nevezd meg! (Attribution):** A kód felhasználása, terjesztése vagy továbbfejlesztése esetén kötelező az eredeti szerző megemlítése és a forrásra (erre a repóra) mutató link elhelyezése.
*   **Így add tovább! (ShareAlike):** Ha módosítod vagy továbbfejleszted a kódot, azt csak ugyanezen feltételek mellett (ingyenesen és megnevezéssel) teheted közzé.
*   **Ne add el! (NonCommercial):** A projekt és annak részei kereskedelmi forgalomba nem hozhatók.

---
**Copyright © 2024 - FoxDebloater Project**
