# FoxDebloater 🦊🚫

<p align="center">
  <img src="https://img.shields.io/badge/Firefox-Hardened-orange?style=for-the-badge&logo=firefox" />
  <img src="https://img.shields.io/badge/Windows-Ready-blue?style=for-the-badge&logo=windows" />
</p>

## 🛠️ Mi ez?

A **FoxDebloater** egy rendszerszintű Windows Firefox hardening és debloat konfiguráció, amely a telemetria, a felesleges háttérszolgáltatások és a böngészőbe épített ajánlórendszerek minimalizálására készült.

A megoldás nem profil-szintű (`user.js`) finomhangolásra épít, hanem Windows **Group Policy (GPO) / Registry policy layer** használatára, amely a beállításokat rendszer szinten érvényesíti és a böngésző frissítései után is megőrzi azokat.

---

## 🔥 Mit tartalmaz?

- Teljes telemetria tiltás  
  (Firefox Studies, Crash/Health Reporting, Default Browser Agent, Mozilla feedback szolgáltatások)

- Böngésző bloat eltávolítás  
  (Pocket, Screenshots, Firefox Accounts opcionális funkciók, ajánlórendszerek, "More from Mozilla" elemek)

- Privacy hardening  
  (DNS-over-HTTPS kényszerítés, Tracking Protection, fingerprinting és cryptomining védelem, search suggestion és URL bar tracking tiltása)

- Rendszerszintű perzisztencia  
  (HKLM policy szint, minden user profilra érvényes beállítások, frissítések és reset után is aktív kontroll)

- Teljesítmény optimalizáció  
  (háttér telemetria folyamatok kikapcsolása, recommendation engine eltávolítása, gyorsabb startup viselkedés)

---

## ⚠️ Jognyilatkozat (Disclaimer)

A konfiguráció használata minden esetben saját felelősségre történik.

A projekt rendszer szintű módosításokat végez a Windows Registry-ben és a Firefox policy rendszerében. A szerző nem vállal felelősséget:

- rendszerinstabilitásért,
- funkcióvesztésért,
- kompatibilitási problémákért,
- adatvesztésért,
- vagy bármilyen közvetlen vagy közvetett káreseményért.

A konfiguráció szándékosan korlátozhat bizonyos funkciókat, például a beépített jelszókezelőt, a Firefox Sync-et és egyes Mozilla szolgáltatásokat.

Erősen ajánlott külső jelszókezelő használata.

---

## 🚀 Telepítés

```bash
1. Töltsd le a FoxDebloater.reg fájlt
2. Futtasd rendszergazdai jogosultsággal
3. Hagyd jóvá a Registry módosításokat
4. Indítsd újra a Firefoxot
```

---

## 🔄 Visszaállítás (FoxRestore.reg)

A projekt tartalmaz egy `FoxRestore.reg` fájlt is, amely teljesen eltávolítja a FoxDebloater által létrehozott Firefox policy beállításokat a Windows Registry-ből.

A restore script:

- törli a `HKLM\SOFTWARE\Policies\Mozilla\Firefox` policy ágat,
- visszaállítja a Firefox alapértelmezett működését,
- megszünteti a `"Managed by your organization"` állapotot,
- nem törli a profiladatokat, jelszavakat, könyvjelzőket vagy böngészési adatokat.

### Restore használata

```bash
1. Futtasd a FoxRestore.reg fájlt rendszergazdai jogosultsággal
2. Hagyd jóvá a Registry módosításokat
3. Indítsd újra a Firefoxot
```

---

## 🛠 Ellenőrzés

Nyisd meg a Firefox címsorát és írd be:

```text
about:policies
```

Ha a policy-k aktívak, a böngésző `"Managed by your organization"` állapotban jelenik meg, ami azt jelenti, hogy a konfiguráció sikeresen érvényesült.

---

## 🤝 Közreműködés

A projekt szabadon használható és módosítható. Pull request-ek és issue-k nyitása üdvözölt.

A módosított verziók publikálhatók, amennyiben:

- az eredeti projekt (**FoxDebloater**) forrásként fel van tüntetve,
- az eredeti szerzői munka korrekt módon meg van említve.

A projekt változatlan formában történő értékesítése nem engedélyezett.

---

## 📄 Licenc

Ez a projekt a **Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)** licenc alatt áll.

A projekt szabadon használható és módosítható, de kereskedelmi célra nem használható fel az eredeti szerző engedélye nélkül.

A felhasználás során kötelező feltüntetni az eredeti szerzőt és a projektet.

A teljes licenc szövege a `LICENSE` fájlban található.

---

**FoxDebloater Project — 2026**
