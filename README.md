# FoxDebloater 🦊🚫

A **FoxDebloater** egy rendszerszintű Windows Firefox hardening és debloat konfiguráció, amely a telemetria, a felesleges háttérszolgáltatások és a böngészőbe épített ajánlórendszerek minimalizálására készült.

A megoldás nem profil-szintű (`user.js`) finomhangolásra épít, hanem Windows **Group Policy (GPO) / Registry policy layer** használatára, amely a beállításokat rendszer szinten érvényesíti és a böngésző frissítései után is megőrzi azokat.

## 🔥 Főbb funkciók

- Teljes telemetria tiltás (Firefox Studies, Crash/Health Reporting, Default Browser Agent, Mozilla feedback szolgáltatások)
- Böngésző bloat eltávolítás (Pocket, Screenshots, Firefox Accounts opcionális funkciók, ajánlórendszerek, “More from Mozilla” elemek)
- Privacy hardening (DNS-over-HTTPS kényszerítés, Tracking Protection, fingerprinting és cryptomining védelem, search suggestion és URL bar tracking tiltása)
- Rendszerszintű perzisztencia (HKLM policy szint, minden user profilra érvényes beállítások, frissítések és reset után is aktív kontroll)
- Teljesítmény optimalizáció (háttér telemetria folyamatok kikapcsolása, recommendation engine eltávolítása, gyorsabb startup viselkedés)

## 🚀 Telepítés

1. Töltsd le a `FoxDebloater.reg` fájlt.  
2. Futtasd **rendszergazdai jogosultsággal**.  
3. Hagyd jóvá a Registry módosításokat.  
4. Indítsd újra a Firefoxot.

## 🛠 Ellenőrzés

Nyisd meg a Firefox címsorát és írd be:

about:policies

Ha a policy-k aktívak, a böngésző “Managed by your organization” állapotban jelenik meg, ami azt jelenti, hogy a konfiguráció sikeresen érvényesült.

## ⚠️ Fontos (Disclaimer)

Ez a konfiguráció rendszer szintű módosításokat végez a Windows Registry-ben és a Firefox policy rendszerében.

A használat teljes mértékben saját felelősségre történik. A szerző nem vállal felelősséget semmilyen közvetlen vagy közvetett kárért, beleértve a rendszerinstabilitást, funkcióvesztést, kompatibilitási problémákat, adatvesztést vagy harmadik féltől származó szolgáltatások hibáit.

A konfiguráció szándékosan korlátozhat bizonyos funkciókat, például a beépített jelszókezelőt, a Firefox Sync-et és egyes Mozilla szolgáltatásokat. Erősen ajánlott külső jelszókezelő (pl. Bitwarden vagy KeePassXC) használata.

## 🤝 Felhasználás és közreműködés

A projekt szabadon használható és módosítható. A módosított verziók publikálhatók, amennyiben az eredeti projekt (FoxDebloater) forrásként meg van említve. A projekt nem értékesíthető változatlan formában, és elvárt az eredeti szerzői munka korrekt feltüntetése minden származtatott változatban.

**FoxDebloater Project — 2026**
