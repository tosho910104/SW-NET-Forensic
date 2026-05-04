# Zoznam zmien / Changelog

Všetky dôležité vylepšenia, nové funkcie a opravy v softvéri sú popísané nižšie.
/ All important improvements, new features, and fixes are described below.

---

## [1.1.0] - 2026-05-03

### 🆕 Nové funkcie / New Features

#### 🇸🇰 Jazyková verzia – Slovenčina / English
- Pridaná kompletná lokalizácia do slovenčiny. Softvér si môžete prepnúť medzi SK a EN kedykoľvek počas používania.
- Added complete localization to English. Switch between SK and EN anytime while using the software.

#### 🔗 Timeline sieťových spojení
- Nová obrazovka, ktorá vám ukáže **kedy sa prvýkrát objavilo** nové sieťové spojenie a kedy zmizlo. Užitočné na sledovanie podozrivej aktivity v čase.
- New timeline view shows **when a network connection first appeared** and when it disappeared. Great for tracking suspicious activity over time.

#### 📊 Nové grafy
- **Graf prenosu dát (RX/TX)** pre každé vybrané spojenie – vidíte, koľko dát váš počítač odosiela a prijíma v reálnom čase.
- **Graf top 5 procesov** – ktoré programy najviac komunikujú cez sieť (podľa objemu dát).
- **RX/TX traffic chart** for each selected connection – see real-time data sent and received.
- **Top 5 processes chart** – which programs consume the most network bandwidth.

#### 🔍 Podrobnosti o spojení na jeden klik
- Po kliknutí na ľubovoľné spojenie teraz vidíte:
  - **WHOIS / RDAP** – kto vlastní vzdialený server
  - **Ping** – odozva spojenia
  - **Traceroute** – cesta paketov cez internet
  - **DNS / reverzné DNS** – názov domény k IP adrese
  - **TLS certifikát** – bezpečnostný certifikát vzdialeného servera (ak existuje)
- One-click connection details now include:
  - WHOIS / RDAP – who owns the remote server
  - Ping – connection response time
  - Traceroute – packet path through the internet
  - DNS / reverse DNS – domain name for an IP address
  - TLS certificate – security certificate of the remote server

#### 🧠 Forenzné nástroje pre procesy
- Ku každému bežiacemu procesu (programu) vám softvér ukáže:
  - **Zoznam knižníc (DLL)** – čo si proces načítal do pamäte
  - **SHA-256 hash** – jedinečný digitálny odtlačok
  - **Veľkosť, verziu, metadata** súboru
  - **Strom procesov** – kto spustil koho (rodič-dieťa)
- Enhanced process forensics:
  - List of loaded libraries (DLLs)
  - SHA-256 hash – unique digital fingerprint
  - File size, version, metadata
  - Process tree – parent-child relationships

#### 🔎 Vyhľadávanie textových reťazcov v pamäti
- Nová funkcia, ktorá prehľadá pamäť vybraného procesu a nájde všetky čitateľné texty (ASCII / Unicode). Užitočné na odhalenie skrytých príkazov alebo URL adries.
- Scan memory of any process for readable text strings (ASCII / Unicode). Useful for finding hidden commands or URLs.

#### 🛡️ Reputačné a threat-intel panely
- **VirusTotal** – kontrola reputácie IP adresy
- **Hybrid Analysis** – analýza podľa SHA-256 hashu súboru
- **GreyNoise** – zistenie, či IP adresa patrí bezpečnostnému skeneru alebo útoku
- Samostatná **tabuľka alertov** – všetky podozrivé nálezy na jednom mieste
- Reputation and threat intelligence panels:
  - VirusTotal – IP reputation check
  - Hybrid Analysis – file analysis by SHA-256
  - GreyNoise – detect if IP is a security scanner or attacker
  - Dedicated **alerts table** – all suspicious findings in one place

#### 🛡️ Ochrana pred pádom systému (Anti-BSOD)
- Keď sa pokúsite ukončiť proces (program), softvér **vyhodnotí riziko**. Nebezpečné systémové procesy sú blokované alebo vyžadujú vaše potvrdenie. Žiadne modré obrazovky smrti.
- When attempting to kill a process, the software **assesses the risk**. Dangerous system processes are blocked or require confirmation. No more Blue Screen of Death.

#### ☁️ Vylepšená práca s cloudovými službami
- API odpovede sa **ukladajú do vyrovnávacej pamäte (cache)** – menej čakania a menej spotrebovaných požiadaviek.
- Lepšia logika **opakovania (retry)** a **časového limitu (timeout)** – ak služba nereaguje, softvér to elegantne ošetrí.
- API responses are now **cached** – faster loading, fewer API calls consumed.
- Better **retry and timeout logic** – graceful handling when services are slow.

#### 🔐 Bezpečnosť API kľúčov
- Vaše API kľúče (napr. k VirusTotal) sa teraz ukladajú **šifrovane**, nie ako obyčajný text. Vaše kľúče sú v bezpečí.
- Your API keys (e.g., for VirusTotal) are now stored **encrypted**, not as plain text. Your keys stay safe.

---

### 🔧 Opravy a vylepšenia / Fixes & Improvements

#### 🧹 Lepšie filtrovanie IP adries
- Opravená normalizácia IPv6 a IPv4-mapped adries
- Softvér teraz správne ignoruje:
  - Súkromné IP (192.168.x.x, 10.x.x.x, 172.16.x.x)
  - CGNAT adresy (100.64.x.x)
  - Multicast, dokumentačné a vyhradené rozsahy
- Better IP filtering:
  - Fixed IPv6 and IPv4-mapped address normalization
  - Now correctly ignores:
    - Private IPs (192.168.x.x, 10.x.x.x, 172.16.x.x)
    - CGNAT addresses (100.64.x.x)
    - Multicast, documentation, and reserved ranges

#### 🚪 Čisté ukončovanie aplikácie
- Pri zatvorení softvéru sa teraz **korektne zastavia** všetky časovače, pozadia úlohy a internetové spojenia. Žiadne visiace procesy.
- Clean application shutdown – all timers, background tasks, and connections are properly stopped.

#### 🔄 Update checker – už bez falošných správ
- Kontrola aktualizácií teraz číta **skutočnú verziu** vášho softvéru. Už vám nebude hlásiť "nová verzia 1.0.0" stále dookola.
- Update checker now reads your **actual software version**. No more false "new version 1.0.0" notifications.

#### 🌐 Viac textov ide cez prekladový systém
- Väčšina dialógových okien a správ je teraz preložená. Menej angličtiny, keď používate slovenčinu.
- Most dialog windows and messages are now translated. Less English when using Slovak language.

---

## [1.0.0] - 2026-04-15

### 🎉 Prvé vydanie / Initial release
- Prvá verejná verzia SW-NET Forensic
- First public release of SW-NET Forensic

---

*Posledná aktualizácia / Last updated: 2026-05-03*
