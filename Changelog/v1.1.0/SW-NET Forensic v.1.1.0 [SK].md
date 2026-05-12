# Zoznam zmien

Všetky dôležité vylepšenia, nové funkcie a opravy v softvéri sú popísané nižšie.

---

## [1.1.0] - 2026-05-03

### 🆕 Nové funkcie

#### 🇸🇰 Jazyková verzia – Slovenčina a angličtina
- Pridaná kompletná lokalizácia do slovenčiny. Softvér si môžete prepnúť medzi SK a EN kedykoľvek počas používania.

#### 🔗 Timeline sieťových spojení
- Nová obrazovka, ktorá vám ukáže **kedy sa prvýkrát objavilo** nové sieťové spojenie a kedy zmizlo. Užitočné na sledovanie podozrivej aktivity v čase.

#### 📊 Nové grafy
- **Graf prenosu dát (RX/TX)** pre každé vybrané spojenie – vidíte, koľko dát váš počítač odosiela a prijíma v reálnom čase.
- **Graf top 5 procesov** – ktoré programy najviac komunikujú cez sieť (podľa objemu dát).

#### 🔍 Podrobnosti o spojení na jeden klik
- Po kliknutí na ľubovoľné spojenie teraz vidíte:
  - **WHOIS / RDAP** – kto vlastní vzdialený server
  - **Ping** – odozva spojenia
  - **Traceroute** – cesta paketov cez internet
  - **DNS / reverzné DNS** – názov domény k IP adrese
  - **TLS certifikát** – bezpečnostný certifikát vzdialeného servera (ak existuje)

#### 🧠 Forenzné nástroje pre procesy
- Ku každému bežiacemu procesu (programu) vám softvér ukáže:
  - **Zoznam knižníc (DLL)** – čo si proces načítal do pamäte
  - **SHA-256 hash** – jedinečný digitálny odtlačok
  - **Veľkosť, verziu, metadata** súboru
  - **Strom procesov** – kto spustil koho (rodič-dieťa)

#### 🔎 Vyhľadávanie textových reťazcov v pamäti
- Nová funkcia, ktorá prehľadá pamäť vybraného procesu a nájde všetky čitateľné texty (ASCII / Unicode). Užitočné na odhalenie skrytých príkazov alebo URL adries.

#### 🛡️ Reputačné a threat-intel panely
- **VirusTotal** – kontrola reputácie IP adresy
- **Hybrid Analysis** – analýza podľa SHA-256 hashu súboru
- **GreyNoise** – zistenie, či IP adresa patrí bezpečnostnému skeneru alebo útoku
- Samostatná **tabuľka alertov** – všetky podozrivé nálezy na jednom mieste

#### 🛡️ Ochrana pred pádom systému (Anti-BSOD)
- Keď sa pokúsite ukončiť proces (program), softvér **vyhodnotí riziko**. Nebezpečné systémové procesy sú blokované alebo vyžadujú vaše potvrdenie. Žiadne modré obrazovky smrti.

#### ☁️ Vylepšená práca s cloudovými službami
- API odpovede sa **ukladajú do vyrovnávacej pamäte (cache)** – menej čakania a menej spotrebovaných požiadaviek.
- Lepšia logika **opakovania (retry)** a **časového limitu (timeout)** – ak služba nereaguje, softvér to elegantne ošetrí.

#### 🔐 Bezpečnosť API kľúčov
- Vaše API kľúče (napr. k VirusTotal) sa teraz ukladajú **šifrovane**, nie ako obyčajný text. Vaše kľúče sú v bezpečí.

---

### 🔧 Opravy a vylepšenia

#### 🧹 Lepšie filtrovanie IP adries
- Opravená normalizácia IPv6 a IPv4-mapped adries
- Softvér teraz správne ignoruje:
  - Súkromné IP (192.168.x.x, 10.x.x.x, 172.16.x.x)
  - CGNAT adresy (100.64.x.x)
  - Multicast, dokumentačné a vyhradené rozsahy

#### 🚪 Čisté ukončovanie aplikácie
- Pri zatvorení softvéru sa teraz **korektne zastavia** všetky časovače, pozadia úlohy a internetové spojenia. Žiadne visiace procesy.

#### 🔄 Update checker – už bez falošných správ
- Kontrola aktualizácií teraz číta **skutočnú verziu** vášho softvéru. Už vám nebude hlásiť "nová verzia 1.0.0" stále dookola.

#### 🌐 Viac textov ide cez prekladový systém
- Väčšina dialógových okien a správ je teraz preložená. Menej angličtiny, keď používate slovenčinu.

---

## [1.0.0] - 2026-04-15

### 🎉 Prvé vydanie
- Prvá verejná verzia SW-NET Forensic

---

*Posledná aktualizácia: 2026-05-03*
