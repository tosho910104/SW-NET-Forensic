# SW-NET Forensic v.2.0.0

## 🎨 Zmeny
* **Kompletná zmena vizuálu:** Moderné, tmavé prostredie optimalizované pre dlhé nočné smeny analytikov.

## 🚀 Pridané funkcie
* **Vizuálna GeoIP mapa:** Interaktívna mapa sieťovej prevádzky (ideálna "hračička" pre manažérov a prezentácie).
* **"Kill process with parent":** Funkcia "Zabi aj rodiča" pre nekompromisné ukončenie celého stromu procesov.
* **Karta „Skóre sieťovej anomálie“:** Nový modul v menu „Sieťové informácie“ pre rýchly prehľad rizika.
* **Filtrovanie podozrivých spojení:** Možnosť jedným klikom zobraziť v tabuľke iba rizikovú komunikáciu.
* **Skrytie systémových procesov:** Odfiltrovanie legitímnych Microsoft procesov pre čistejší výhľad na hrozby.
* **Command Line Inspector:** Inteligentné zvýrazňovanie podozrivých argumentov v príkazovom riadku.
* **Analýza úrovne oprávnení:** Informácie o pôvode a úrovni práv pri spustení.
* **Vizuálny rodokmeň procesov:** Grafické zobrazenie parent/child vzťahov vrátane indikátora, či je proces stále živý.
* **Threat Intelligence cez AlienVault API:** Automatická analýza hrozieb v reálnom čase.
* **Pokročilý Export:** Možnosť generovania reportov do PDF a HTML.
* **Advanced Search (Power-User engine):** Vyhľadávanie cez hlavičku stĺpca s podporou:
    * Rozsahov portov (napr. `1000-2000`, `>1024`, `<443`).
    * IP rozsahov cez CIDR notáciu (napr. `192.168.0.0/24`).
    * Operátorov a negácie (`-`, `!`).
* **Kontextové menu:** Pridané funkcie priamo do stromu procesov.
* **Persistent Connections Alert:** Dashboard upozornenie na podozrivé dlhotrvajúce spojenia.
* **Windows Notifications:** Natívne systémové upozornenia pri detekcii podozrivých aktivít.
* **Tray Mode:** Možnosť skryť aplikáciu do tray lišty.

## ⚙️ Nastavenia
* **Vylepšený Startup:** Možnosť spustiť aplikáciu po štarte Windows (cez startup folder) so skrytým spustením do tray a úvodnou notifikáciou.
* **AlienVault Integrácia:** Pole pre vlastný API kľúč.
* **Vizuálne úpravy:** Celkové vyladenie grafiky nastavení.

## 🔧 Opravy a vylepšenia
* **Persistence Fix:** Opravené ukladanie nastavení, logov a API kľúčov pri aktualizácii aplikácie.
* **Vylepšené logovanie:** Detailnejší zápis sieťových a procesných udalostí.
* **UI Fixes:** Oprava klikateľných labelov pre Hash a ikon pri API nastaveniach.
* **Stabilita:** Drobné opravy kódu a optimalizácia nefunkčných funkcií.
