# Curated OSINT namecheckers

A curated list of tools and sites for **username search**, **account discovery**, and **username availability** (“namecheck”) across social networks and the web. It focuses on namecheckers and related workflows—not general OSINT as a whole.

## Contents

- [Open source tools](#open-source-tools)
- [OSINT online tools](#osint-online-tools)
- [Branding](#branding)
- [Toolkits](#toolkits)
- [Useful links](#useful-links)
- [Contributing](#contributing)
- [Disclaimer](#disclaimer)
- [License](#license)

## Open source tools

- [Maigret](https://github.com/soxoj/maigret) — Username search with the largest site set and profile parsing.
  - 3100+ sites 👍; profile parsing (PII, links to other profiles) 👍; recursive search on newly found usernames 👍; filter by country/category tags 👍; very few false positives 👍; censorship and captcha detection; `pip install maigret`.

- [Sherlock](https://github.com/sherlock-project/sherlock) — The original username hunter; mature, widely packaged.
  - 479 sites; batch search 👍; Tor and proxy support 👍; CSV/XLSX/JSON export 👍; custom sites and rules; `pipx install sherlock-project`; also Docker, dnf, Homebrew.

- [Enola](https://github.com/TheYahya/enola) — Fast Go-based username hunter with modern CLI.
  - 407 sites; Go single binary 👍; Docker support; CSV/JSON export; `go install github.com/theyahya/enola/cmd/enola@latest`.

- [Snoop](https://github.com/snooppr/snoop) — Username search with the largest raw site count; partially paid.
  - ~350 sites in free demo, 5300+ in paid full version 👍; country ranking and filtering 👍; multi-format reports (CSV/HTML/maps) 👍; geolocation plugins; Android/Termux support; binary releases.

- [Aliens Eye](https://github.com/arxhr007/Aliens_eye) — AI-powered username scanner with confidence scoring.
  - 841 sites 👍; AI-enhanced detection with confidence scoring (0–100%) 👍; three scan levels (basic/intermediate/advanced); username variation generation; JSON reporting; multi-OS including Android/Termux; `pip install -r requirements.txt`.

- [Blackbird](https://github.com/p1ngul1n0/blackbird) — Username and email search using the WhatsMyName database.
  - 600+ sites 👍; email search 👍; AI-powered profiling (free) 👍; PDF/CSV/JSON export 👍; category filtering; NSFW sites included by default; `pip install -r requirements.txt`.

- [WhatsMyName](https://github.com/webbreacher/whatsmyname) — Community-maintained site-check database (data only, no built-in checker).
  - 732 sites 👍; JSON format used by Blackbird, Naminter, recon-ng, Maltego, SpiderFoot, and others; web UI at [whatsmyname.app](https://whatsmyname.app/).

- [Naminter](https://github.com/3xp0rt/Naminter) — Async username enumeration using the WhatsMyName dataset.
  - 730+ sites 👍; TLS-level browser impersonation via curl_cffi (bypasses Cloudflare and bot detection that block tools using plain requests/aiohttp) 👍; category filtering 👍; PDF/CSV/JSON/HTML export 👍; `pip install naminter`; also Docker.

- [Linkook](https://github.com/JackJuly/linkook) — Username search with email/breach checks and Neo4j graph export.
  - 64 sites; **email discovery + breach check** via HudsonRock's Cybercrime Intelligence DB or Have I Been Pwned API 👍; **Neo4j-friendly JSON export** for graph visualization of accounts/usernames/emails 👍; extracts linked accounts from profile pages (similar to Maigret + socid-extractor, but on a smaller site set); default scan covers only 10 "connected" sites, use `--scan-all` for full coverage; `pipx install linkook`.

- [social-analyzer](https://github.com/qeeqbox/social-analyzer) — Large-scale username search with layered detection.
  - 999 sites 👍; web UI 👍; multilayer detection (OCR, normal, advanced, special) 👍; metadata extraction; `pip install social-analyzer`; no granular confidence scoring — `maybe` status produces false positives 🚫.

- [nexfil](https://github.com/thewhiteh4t/nexfil) — Lightweight and fast username search.
  - 328 sites; batch processing 👍; results auto-saved to text files; `pip install nexfil`; no longer maintained (last commit Sep 2023) 🚫.

- [DetectDee](https://github.com/piaolin/DetectDee) — Search by username, email, or phone; written in Go.
  - 372 sites; screenshot capture 👍; WAF evasion; ChatGPT integration for result tagging; Google search integration; pre-compiled binaries; no longer maintained (last commit Jul 2023) 🚫.

- [vesper](https://github.com/krishpranav/vesper) — Rust-based async username scanner using a Sherlock-derived database.
  - 299 sites; Rust + Tokio for fast async scanning 👍; confidence scoring (CONFIRMED/LIKELY) 👍; headless Chrome screenshot capture 👍; Tor proxy support; JSON report export; built-in site-validation test mode; `cargo build --release`.

- [tookie-osint](https://github.com/Alfredredbird/tookie-osint) — Username discovery with a web UI.
  - 261 sites; headless mode; CSV export; multi-OS installer scripts; ~20% false positives 🚫.

- [Investigo](https://github.com/tdh8316/Investigo) — Go-based tool using Sherlock’s site database.
  - Uses Sherlock DB 👍; concurrent requests (32 default) 👍; Tor proxy support; content downloading; `go build`.

- [sagemode](https://github.com/senran101604/sagemode) — Simple username search.
  - 146 sites; real-time CLI output; known false positives on some platforms 🚫; no longer maintained (last commit Dec 2023) 🚫.

- [Arina-OSINT](https://github.com/AlexC-ux/Arina-OSINT) — Username search written in C#.
  - 76 sites; requires .NET Core 3.1; no longer maintained (last commit Mar 2022) 🚫.

- [GhostTrack](https://github.com/HunxByts/GhostTrack) — Multi-purpose OSINT tool (IP, phone, username) with interactive menu.
  - 24 sites for username tracking; primary focus is on IP/phone lookup, username search is one of four menu options; HTTP 200 status code check only — high false positive rate 🚫; no longer maintained (last commit Jan 2024) 🚫.

- [Userrecon](https://github.com/wishihab/userrecon) — Bash-based username search.
  - 66 sites; shell script (no dependencies); many checks broken (Instagram, Facebook, Twitter flagged); no longer maintained (last commit Feb 2021) 🚫.

- [NicknameFinder](https://github.com/restanse/NicknameFinder) — Username search organized by site categories.
  - 44 sites (forums, games, social, finance); no longer maintained (last commit Apr 2021) 🚫.

- [netizenship](https://github.com/rahulrajpl/netizenship) — Multi-threaded username search.
  - 36 sites; `pip install netizenship`; no longer maintained (last commit Dec 2021) 🚫.

- [Search4](https://github.com/0xknown/Search4) — Small and fast username search.
  - 35 sites; multi-threaded; `pip install search4`; no longer maintained (last commit Jul 2022) 🚫.

- [Stalkie](https://github.com/ashendilantha/stalkie) — Go-based username scanner with confidence scoring and headless browser mode.
  - 13 sites; confidence scoring (0–100%) with multi-signal analysis (HTTP status, title match, body mentions) 👍; script-tag stripping to reduce false negatives 👍; login wall detection 👍; headless browser via go-rod for JS-heavy sites 👍; Tor/SOCKS5 proxy support; bulk input; CSV/JSON/TXT export; `go build`.

- [Socialscan](https://github.com/iojw/socialscan) — Checks **email** and username availability via registration APIs (not profile URLs).
  - 11 platforms (Instagram, Twitter, GitHub, Tumblr, GitLab, Reddit, etc.) 👍; 100% accuracy by querying signup endpoints 👍; async (100 queries in ~4 sec) 👍; `pip install socialscan`.

- [recon-ng](https://github.com/lanmaster53/recon-ng/) — Full OSINT reconnaissance framework with a WhatsMyName profiler module.
  - Modular Metasploit-like architecture 👍; interactive console with tab completion 👍; REST API and web UI 👍; Docker support; username check is one module among many.

- [SocialPath](https://github.com/woj-ciech/SocialPath) — Track users across 10 platforms with deeper extraction on 4; web UI.
  - Django-based web interface; detailed data extraction (Twitter, StackOverflow, Instagram, Reddit); requires API keys; no longer maintained (last commit Jan 2021) 🚫.

- [thorndyke](https://github.com/rly0nheart/thorndyke) — Lightweight username enumeration.
  - 200+ sites; `pip install thorndyke`; archived by author — no longer supported 🚫.

- [sherlock-go](https://github.com/mesuutt/sherlock) — Minimal Go implementation of Sherlock.
  - ~164 sites; faster than Python original; pre-compiled binaries; no longer maintained (last commit Aug 2019) 🚫.

- [Gideon](https://github.com/YouVBeenHacked/gideon) — OSINT tool for phone numbers, car plates, nicknames, and torrents by IP.
  - Russian-focused; username search is a secondary feature; no longer maintained (last commit Nov 2020) 🚫.

## OSINT online tools

Websites to search from a browser. Many show ads and may log requests.

- [WhatsMyName](https://whatsmyname.app/) — ~250 sites; web UI for the [WhatsMyName](https://github.com/webbreacher/whatsmyname) dataset; rich category filters.

- [Lullar](https://com.lullar.com/) — Free email/name/username people search across 175+ platforms; no sign-up, since 2009.

- [Usersearch](https://usersearch.org/) — ~120 popular sites, 100+ generic forums, 6 dating sites, crypto forums.

- [analyzeid username checker](https://analyzeid.com/username/) — 80+ social sites; summarizes what public signals suggest about a taken username 👍.

- [iDCrawl](https://www.idcrawl.com/username) — 12 sites.

- [suIP.biz](https://suip.biz/ru/?act=sherlock) — Online Sherlock-style checker.

- [WhatsMyName App](https://whatsmynameapp.us/tools/whatsmyname-app) — 732 sites; full web UI with guides, tutorials, step-by-step walkthroughs, and CSV export. Browser-based, no login required.


## Branding

These tools focus on **username availability** and brand/domain squatting checks—not on finding a specific person’s accounts. Marketers often use them for brand protection; many include domain checks alongside social handles.


- [Namecheckup](http://namecheckup.com/) — 270+ networks and sites; 45 TLDs.

- [InstantUsername](https://instantusername.com/) — 100+ social sites; [open source](https://github.com/instant-username-search) 👍.


- [CHECKUSER.org](https://checkuser.org) — Popular domains plus 52 social sites.

- [Namechk](https://namechk.com/) — Availability across 96 sites and 36 TLDs.

- [Namecheckr](https://www.namecheckr.com/) — Domains and social handles across 38 networks and 17 TLDs.

- [Checkerapi](https://app.swaggerhub.com/apis/checker/api) — Six services; [open source](https://github.com/checker/api) 👍.

- [360username](https://360username.com/) — AI-powered Domain name and sicial media username generator and checker.

## Toolkits

- [One-plus OSINT Toolkit](https://one-plus.github.io/EmailUsername) — Email/username-oriented OSINT toolkit.

- [Aware-online username search](https://www.aware-online.com/en/osint-tools/username-search-tool/) — Browser-based username search tool.

## Useful links

- [OSINT Handbook (Sept 2020) — “Username Check”](https://i-intelligence.eu/uploads/public-documents/OSINT_Handbook_2020.pdf)

- [OH SHINT! — Usernames](https://ohshint.gitbook.io/oh-shint-its-a-blog/osint-web-resources/usernames) — Curated list of username OSINT resources.

- [What’s wrong with namecheckers?](https://soxoj.medium.com/whats-wrong-with-namecheckers-981e5cba600e) — Essay on limitations of namechecking tools.

## SOWEL Classification

- [SOWEL-8. Using Nicknames](https://sowel.soxoj.com/using-nicknames)
- [SOTL-6.2. Check Nicknames Reuse to Find Another Account](https://sowel.soxoj.com/nicknames-reuse)

## Contributing

Pull requests are welcome. Add one line per tool in the form `- [Name](url) — short summary` (optional indented sub-bullets for notable pros/cons). Prefer maintained projects and working links; note unmaintained or broken services in the line text. Avoid duplicate entries and pure spam.

## Disclaimer

Use these tools **lawfully and ethically**, only on data you are allowed to access, and in line with each platform’s terms and applicable law. This list is for **defensive OSINT and research**; authors of this repository are not responsible for misuse.

## License

This repository is licensed under the [MIT License](LICENSE).
