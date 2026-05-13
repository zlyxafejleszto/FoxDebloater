# FoxDebloater 🦊🚫

A **FoxDebloater** egy rendszerszintű Windows Firefox hardening és debloat konfiguráció, amely a telemetria, a felesleges háttérszolgáltatások és a böngészőbe épített ajánlórendszerek minimalizálására készült.

A megoldás nem profil-szintű (`user.js`) finomhangolásra épít, hanem Windows **Group Policy (GPO) / Registry policy layer** használatára, amely a beállításokat rendszer szinten érvényesíti és a böngésző frissítései után is megőrzi azokat.

## 🔥 Főbb funkciók

* Teljes telemetria tiltás (Firefox Studies, Crash/Health Reporting, Default Browser Agent, Mozilla feedback szolgáltatások)
* Böngésző bloat eltávolítás (Pocket, Screenshots, Firefox Accounts opcionális funkciók, ajánlórendszerek, “More from Mozilla” elemek)
* Privacy hardening (DNS-over-HTTPS kényszerítés, Tracking Protection, fingerprinting és cryptomining védelem, search suggestion és URL bar tracking tiltása)
* Rendszerszintű perzisztencia (HKLM policy szint, minden user profilra érvényes beállítások, frissítések és reset után is aktív kontroll)
* Teljesítmény optimalizáció (háttér telemetria folyamatok kikapcsolása, recommendation engine eltávolítása, gyorsabb startup viselkedés)

## 🚀 Telepítés

1. Töltsd le a `FoxDebloater.reg` fájlt.
2. Futtasd **rendszergazdai jogosultsággal**.
3. Hagyd jóvá a Registry módosításokat.
4. Indítsd újra a Firefoxot.

## 🔄 Visszaállítás (FoxRestore.reg)

A projekt tartalmaz egy `FoxRestore.reg` fájlt is, amely teljesen eltávolítja a FoxDebloater által létrehozott Firefox policy beállításokat a Windows Registry-ből.

A restore script:

* törli a `HKLM\SOFTWARE\Policies\Mozilla\Firefox` policy ágat,
* visszaállítja a Firefox alapértelmezett működését,
* megszünteti a “Managed by your organization” állapotot,
* nem törli a profiladatokat, jelszavakat, könyvjelzőket vagy böngészési adatokat.

### Restore használata

1. Futtasd a `FoxRestore.reg` fájlt rendszergazdai jogosultsággal.
2. Hagyd jóvá a Registry módosításokat.
3. Indítsd újra a Firefoxot.

## 🛠 Ellenőrzés

Nyisd meg a Firefox címsorát és írd be:

about:policies

Ha a policy-k aktívak, a böngésző “Managed by your organization” állapotban jelenik meg, ami azt jelenti, hogy a konfiguráció sikeresen érvényesült.

## ⚠️ Fontos (Disclaimer)

Ez a konfiguráció rendszer szintű módosításokat végez a Windows Registry-ben és a Firefox policy rendszerében.

A használat teljes mértékben saját felelősségre történik. A szerző nem vállal felelősséget semmilyen közvetlen vagy közvetett kárért, beleértve a rendszerinstabilitást, funkcióvesztést, kompatibilitási problémákat, adatvesztést vagy harmadik féltől származó szolgáltatások hibáit.

A konfiguráció szándékosan korlátozhat bizonyos funkciókat, például a beépített jelszókezelőt, a Firefox Sync-et és egyes Mozilla szolgáltatásokat. Erősen ajánlott külső jelszókezelő használata.

## 🤝 Közreműködés

A projekt szabadon használható és módosítható. Pull request-ek és issue-k nyitása üdvözölt.

A módosított verziók publikálhatók, amennyiben:
- az eredeti projekt (FoxDebloater) forrásként fel van tüntetve,
- az eredeti szerzői munka korrekt módon meg van említve minden származtatott változatban,
- a [LICENSE](LICENSE) fájlban foglalt feltételek teljesülnek.

A projekt változatlan formában történő értékesítése nem engedélyezett.

**FoxDebloater Project — 2026**
