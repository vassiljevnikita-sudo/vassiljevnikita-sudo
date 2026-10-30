# Nikita Vassiljev

Pharmacy student at FU Berlin (semester 7 of 8) and working student in pharmaceutical quality assurance. Alongside my studies I build software with multi-agent workflows: I set the goal, the requirements and the acceptance checks; the agents plan, implement, test, review each other's work and keep going until the goal is met. I run the infrastructure myself: my own server, a Tailscale network across my devices and virtual machines for load balancing, faster worktree setup and shorter builds.

## Projects

### Complaint Dossier

A PowerShell workflow that drafts the individual report for each complaint in an Excel complaint list. For every open complaint it builds a prompt from that row, earlier complaints for the same batch and product, and the case folder, and hands it to the Microsoft 365 Copilot desktop app, which drafts the report. Each complaint gets its own Word report, marked DRAFT until a reviewer has checked and approved that report, and its own audit log with SHA-256 hashes. `./Invoke-ComplaintDossier.ps1 -Demo` runs on synthetic complaints with prewritten sample answers instead of Copilot, and CI runs it on every push. The project is a public rebuild of a prototype from my working-student job, made with synthetic data and a neutral template; it contains no company material. Designed along GAMP 5 principles; not validated.

[Repo](https://github.com/vassiljevnikita-sudo/complaint-dossier) · [Design note (GAMP 5)](https://github.com/vassiljevnikita-sudo/complaint-dossier/blob/main/docs/design-note.md) · [Sample report (PDF)](https://github.com/vassiljevnikita-sudo/complaint-dossier/blob/main/docs/sample/complaint-dossier-sample-DRAFT.pdf) · [CI runs](https://github.com/vassiljevnikita-sudo/complaint-dossier/actions)

### Life OS

A personal decision system as an Android app; a development project with one user, code private. It connects FinTS (bank approval pending), Android Health Connect, Google Calendar, Gmail, Google Maps, weather and AI models; input comes from a journal and tasks. Its core is a deterministic decision engine that plans the day, learns from actual behavior and keeps the plan load at about 70 % expected completion. A language model phrases follow-up questions and maps journal answers; only fixed, reversible rules take effect.

[Screenshots and videos](https://github.com/vassiljevnikita-sudo/life-os-showcase)

### Stock selection with Quality by Design (work in progress)

Python research on picking stocks that beat the world index fund URTH, using only information available on each day. 2,790 model families and 1.63 billion prediction rows (2016–2025) are judged by Quality by Design: map how the result responds to each setting and keep robust regions instead of the single best setting. The current selector is a fixed rule, Leader5. In backtests on EUR 10,000 it beat URTH by a mean EUR 1,658 a year in 2017–2021 and EUR 2,328 a year in 2022–2025; 2022–2025 informed the choice of the rule, so it is not an independent test. Since 5 Oct 2026 a paper-trading demo runs on a Trading 212 demo account with virtual money; no real capital is involved. A learned method for choosing between the models has not met its predefined criteria yet, and the repo documents what failed and why.

[Paper-trading demo](https://simple-light-qbd.expo.app/graphen) · [Start page](https://simple-light-qbd.expo.app/) · [Repo](https://github.com/vassiljevnikita-sudo/simple-and-light-research)

### Questify

A to-do app in German where finished tasks earn XP and levels, and friends compete on weekly and monthly leaderboards. I built it with AI coding agents. It is released as an Android APK and as a web app; the source code is private, the repo holds the APK releases.

[Open the app](https://mastertasker.expo.app/willkommen/) · [Releases repo](https://github.com/vassiljevnikita-sudo/questify-releases)

### portfolio-check

Every morning it checks that project links, demo pages, READMEs and CI work for a logged-out visitor, and it scans my public repos for secrets and confidential employer terms. [Repo](https://github.com/vassiljevnikita-sudo/portfolio-check)

### Battery fixes in forks

- [tailscale-android-screen-power](https://github.com/vassiljevnikita-sudo/tailscale-android-screen-power): Tailscale for Android pauses the VPN while the screen is off and reconnects when it turns on, to cut background battery use. Experimental, with tests.
- [t3code, branch fix/android-background-battery](https://github.com/vassiljevnikita-sudo/t3code/tree/fix/android-background-battery): the T3 Code Android app suspends its connections and activity reports in the background.

## Publication

Jones E, Vassiljev N. Zukunft der Pharmazie: Welche Kompetenzen brauchen Apotheker*innen? Die Perspektive der Studierenden auf Studium und Approbationsordnung [The future of pharmacy: What knowledge and skills do pharmacists need? The students' perspective on the curriculum and licensing regulations for pharmacists]. *Bundesgesundheitsblatt* 68(5), 519–525 (2025). [doi:10.1007/s00103-025-04050-4](https://doi.org/10.1007/s00103-025-04050-4) · [Google Scholar](https://scholar.google.com/citations?user=4rua7qYAAAAJ)

## Availability

Up to 15 hours a week from 1 Feb to 30 Jun 2027, full-time from 15 Sep 2027.

## Contact

[vassiljev.nikita@gmail.com](mailto:vassiljev.nikita@gmail.com)
