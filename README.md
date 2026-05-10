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

## ⚠️ Fontos (Disclaimer)

A szkriptet mindenki **saját felelősségére** használja. A Registry módosítása komoly beavatkozás, így garanciát semmire nem tudok vállalni. Nem tartozom felelősséggel semmilyen adatvesztésért vagy rendszerhibáért – én csak a kódot adom, te pedig eldöntöd, használod-e. 

**Figyelem:** Ez a konfiguráció biztonsági okokból tiltja a Firefox beépített jelszókezelőjét és a Sync funkciót. Használj külső jelszókezelőt (pl. Bitwarden).

## 🤝 Felhasználás és Közreműködés

Ez a projekt szabadon felhasználható és alakítható az alábbiak szerint:

*   **Használd szabadon:** Nyugodtan alakítsd át, szabd személyre vagy fejleszd tovább.
*   **Add tovább:** A módosított verziókat is kiadhatod, de kérlek, **említsd meg az eredeti projektet (FoxDebloater)** forrásként. Ennyi tisztelet jár a befektetett munkáért.
*   **Maradjon ingyenes:** Ne add el másnak azt, amit én ingyen adtam neked.
*   **Ne élj vissza vele:** Ne hirdesd sajátodként a módosítatlan kódot.

---
**FoxDebloater Project - 2026**
