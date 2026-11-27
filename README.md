# FA Software

**Software built in public, one project at a time.**

I build practical software: automation, data tools, bots, network and security utilities, and web. Every project here is a real, working piece of a growing portfolio, and I document the process as I go.

---

## What I build

| Area | What it means |
|---|---|
| **Automation** | Scripts and tools that remove repetitive work (reports, file handling, scheduled jobs) |
| **Data** | Collecting, storing and presenting data so it is easy to understand |
| **Bots** | Assistants and notifiers that run on their own |
| **Network & security tools** | Monitoring, scanning and alerting, built defensively |
| **Web** | Clean, fast sites and dashboards (a side service, not the only one) |

## Projects

| Project | What it does | Stack | Version |
|---|---|---|---|
| [**Lynceus**](https://github.com/fas0ftware/lynceus) | Home network watch (formerly Home Network Monitor): finds every device, alerts on new devices and risky ports (desktop or phone push), activity timeline; a security advisor explains every open port and how to close it, with a network score | Python, Scapy, SQLite, Flask, Docker | 2.5 |
| [**Maze**](https://github.com/fas0ftware/maze) | Layered honeypot with a C engine: fake progress, growing delays, every move logged; passive attacker reports; Docker image, production WSGI server | C, libsodium, Python, Flask | 0.3.1 |
| [**Janus**](https://github.com/fas0ftware/janus) | Dependency-free TCP and UDP port scanner with a browser interface (Janus Web), service and version detection, TLS certificate checks and STARTTLS; host discovery, one worker pool for all hosts, adaptive timeouts, IPv4/IPv6, CIDR, JSON; fuzzed parsers, clean under ASan, UBSan, TSan and valgrind | C11, POSIX, pthreads | 1.9 |
| [**Ariadne**](https://github.com/fas0ftware/ariadne) | Phone app that scores your day with hourly check-ins, streaks, insights and backups | React Native, Expo, TypeScript | 1.1.1 |
| [**Heimdall**](https://github.com/fas0ftware/Project_Heimdall) | Stock dashboard: RSI, MACD, moving-average crosses, risk metrics, lump sum vs. monthly investing | Python, Streamlit, Plotly | 2.0 |
| [**Hugnin**](https://github.com/fas0ftware/Project_Hugnin) | RSI scanner for 109 stocks and cryptos: an RSI map in the browser, a terminal scanner and a private Telegram alert bot | Python, yfinance | 3.1 |
| [**Orion**](https://github.com/fas0ftware/Project_Orion) | Price-drop alerts on Telegram for any shop page; the watchlist with price history in the browser | Python, BeautifulSoup | 2.1 |
| [**JUDA**](https://github.com/fas0ftware/JUDA) | Smart-home assistant with Turkish commands, roles, scenes and schedules | Python (stdlib only) | 0.2.2 |
| [**Dionysus**](https://github.com/fas0ftware/Project_Dionysus) | Live weather of any city turned into a mood and a playlist | Python, Streamlit | 2.0 |
| [**Zarathustra**](https://github.com/fas0ftware/Zarathustra_TTS) | Text-to-speech studio for long scripts: 300+ neural voices, timed subtitles, a narration library in the browser | Python, Edge-TTS | 2.1 |
| [**Ratatoskr**](https://github.com/fas0ftware/Project_Ratatoskr) | WhatsApp Web messages from the browser or the command line: preview, scheduling, dry runs | Python, Selenium | 2.1 |
| [**Daedalus**](https://github.com/fas0ftware/daedalus) | Coding assistant on Telegram and in the browser: Claude writes Python and runs it in a locked-down Docker sandbox | Python, Claude API, Docker | 0.2 |
| [**Mnemosyne**](https://github.com/fas0ftware/mnemosyne) | Encrypted, deduplicating backups that test their own restores: content-defined chunks, keyed BLAKE3 ids, Argon2id-wrapped keys, restore that treats snapshots as untrusted, hourly timers to two disks, snapshot diff, a local app to browse and verify, a paper recovery code | Rust, RustCrypto, zstd | 0.4 |
| [**Olympos**](https://github.com/fas0ftware/olympos) | One page for every project and home system: stages, unpushed work, CI, backups, network watch, DNS filter, laptop security, events and health, notifications, disks and sites, problems first; each finding turned into a task with the command that fixes it, sent to Iris | Python (stdlib only), GitHub GraphQL | 0.9 |
| [**Pythia**](https://github.com/fas0ftware/pythia) | DNS filter for the whole home network: block lists, your own allow/block rules, DNS over TLS upstream, flood and open-resolver guards, a laptop that serves only itself away from home, per-device profiles with a bedtime | Python (stdlib only), asyncio | 0.3 |
| [**Aegis**](https://github.com/fas0ftware/aegis) | Security check for a Linux laptop in plain words: firewall, disk encryption, updates, SSH, kernel hardening and more, each finding with why it matters and the commands that fix it; read-only, a report page, a status file for Olympos | Python (stdlib only) | 0.2 |
| [**Themis**](https://github.com/fas0ftware/themis) | Watches a laptop's system journal: failed logins at the lock screen, sudo and SSH, brute force, a new USB device that types like a keyboard (BadUSB), services that run for the first time, programs that start listening on the network; learns what is normal first, ignore rules, a read-only page, no root | Python (stdlib only), journalctl, ss, SQLite | 0.3 |
| [**Hestia**](https://github.com/fas0ftware/hestia) | Laptop health check: disk space and I/O errors, temperatures against each sensor's limits, battery wear, wireless-device batteries, memory, load, failed services, a pending restart; days until a disk is full from its own history; alerts only when something changes, a live page | Rust | 0.3 |
| [**Charon**](https://github.com/fas0ftware/charon) | Files between laptop and phone over your own network: a QR code, a secret one-time link that expires, TLS with a kept self-signed certificate, an upload page the other way round, a note (a password) shown once, a window to drop files and show the QR code; a small HTTP server on rustls | Rust, rustls, ring | 0.3 |
| [**Iris**](https://github.com/fas0ftware/iris) | One inbox for every home tool's notifications, speaking ntfy's protocol: repeats folded, quiet hours with a morning digest, per-tool minimums, rules by text, delivery to phone and desktop with retries that never double; a to-do list tools fill ("turn the firewall on: run this") that closes itself when the problem is gone, with one plan every morning | Python (stdlib only) | 0.3 |
| [**Chronos**](https://github.com/fas0ftware/chronos) | A diary of your commits across every local repository, private and unpushed work included: streaks, this week against last, hours and weekdays, a heatmap image without project names, an evening task when a streak is at risk that closes itself after your commit | Python (stdlib only) | 0.2 |

Every repository has tests, CI with security scanning (bandit, pip-audit / npm audit / cargo audit, sanitizers for C) and the latest results as images in its README.

**In the pipeline:** an automated quote-video channel (Prometheus produces, Hermes publishes).

## Tech I work with

`Python` · `Rust` · `C` · `TypeScript` · `React Native` · `Flask` · `Streamlit` · `SQLite` · `Docker` · `ffmpeg` · `GitHub Actions` · `Git`

I build with AI assistance and focus on understanding what the code does, how the parts connect and why it is designed that way.

## Build in public: *Coding Until Noticed*

A short-video series where I show real coding progress, from first commit to working project. New posts and videos are on:

- Instagram: [@fa.software](https://instagram.com/fa.software)

## Work with me

Open to small projects and collaborations, especially automation, data tools and network utilities.

- Email: anil.hyperborea@gmail.com
- Website: [fas0ftware.github.io/FA_Software_web](https://fas0ftware.github.io/FA_Software_web/)

---

<sub>Every project here follows one rule: it has to run, and it has to be explained.</sub>
