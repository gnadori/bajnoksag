# Tarka-Barka Bajnokság

Ez a projekt a Csibék 2025-2026-os bajnokságainak hivatalos weboldala. Itt követhetjük nyomon a különböző házi bajnokságok (Darts, Klask, Flip 7, Sakk) eredményeit és állását.

🔗 **Élő verzió:** [https://gnadori.github.io/bajnoksag/](https://gnadori.github.io/bajnoksag/)

## Játékok és Szabályok

A rendszer többféle lebonyolítási módot támogat:

*   **Darts (Körmérkőzés)**: Mindenki játszik mindenki ellen. A győzelem 3 pont, döntetlen 1 pont.
*   **Klask (Páros Körmérkőzés)**: Hasonló a Dartshoz, de itt 2 fős csapatok mérkőznek meg.
*   **Flip 7 (Számláló)**: Egy egyszerű számláló, ahol a győztes partik számát gyűjtik a játékosok. **Különlegesség:** Folyamatosan lehet csatlakozni (a "Csatlakozás" gombbal) még a bajnokság elindítása után is!
*   **Sakk (Kieséses)**: Egyenes kieséses rendszer. Döntetlen nem lehetséges (a rendszer nem engedi rögzíteni).

## Funkciók

### Versenyzőknek
*   **Regisztráció**: Egyszerű belépés Microsoft fiókkal (AKG-s cím).
*   **Eredmények írása**: A saját meccseidnél (vagy admin joggal bárhol) beírhatod az eredményt.
*   **Állás megtekintése**: Automatikusan frissülő tabella.

### Adminisztrátoroknak
*   **Bajnokság Létrehozása**: Új verseny indítása név és típus megadásával.
*   **Bajnokság Indítása**: Ha összegyűltek a jelentkezők, a zöld gombbal generálható le a sorsolás.
*   **Lezárás**: Ha vége a bajnokságnak, lezárható (további módosítás nem lehetséges).
*   **Törlés**: A bajnokság és az összes hozzá tartozó eredmény végleges törlése.
*   **Eredmények Korrekciója**: Hibás rögzítés esetén az admin törölheti (resetelheti) a meccseredményeket, Flip 7 esetén pedig csökkentheti (-1) a pontszámot.

## Technikai Háttér

*   **Frontend**: Vanilla HTML/JS/CSS (nincs build step).
*   **Backend / Adatbázis**: Google Firebase (Firestore) - Real-time adatfrissítés.
*   **Auth**: Microsoft Authentication Library (MSAL) - Azure AD belépés.
*   **Hosting**: GitHub Pages.

## Design

A "Tarka-Barka" design célja egy vidám, barátságos, könnyen átlátható felület biztosítása, ami jól mutat mobilon és asztali gépen is.
