# Nikita Vassiljev

Pharmacy student at FU Berlin (semester 7 of 8) and working student in pharmaceutical quality assurance. Alongside my studies I build software with multi-agent workflows: I set the goal, the requirements and the acceptance checks; the agents plan, implement, test, review each other's work and keep going until the goal is met. I run the infrastructure myself: my own server, a Tailscale network across my devices and virtual machines for load balancing, faster worktree setup and shorter builds.

## Projects

### Complaint Dossier

A PowerShell tool for an existing complaint process: it fills your own Word report template from your Excel complaint list, and the Microsoft 365 Copilot desktop app writes the report text. Two commands: `Setup.cmd` checks the list and the template and says what is missing, `Run.cmd` drafts the report for every complaint of a period that has none yet, for example a whole year. Every report is a draft that shows its automated check results; the review happens afterwards in Word, with a review list for who checked which report, and an audit log with SHA-256 hashes per report. `Run.cmd -Demo` runs on synthetic complaints with prewritten answers instead of Copilot, and CI runs it on every push; the live path was tested with Copilot on synthetic complaints. The project is a public rebuild of a prototype from my working-student job, made with synthetic data and neutral templates; it contains no company material. Designed along GAMP 5 principles; not validated.

[Repo](https://github.com/vassiljevnikita-sudo/complaint-dossier) · [Design note (GAMP 5)](https://github.com/vassiljevnikita-sudo/complaint-dossier/blob/main/docs/design-note.md) · [Sample report (PDF)](https://github.com/vassiljevnikita-sudo/complaint-dossier/blob/main/docs/sample/complaint-dossier-sample-DRAFT.pdf) · [CI runs](https://github.com/vassiljevnikita-sudo/complaint-dossier/actions)

### Life OS

A personal decision system as an Android app; a development project with one user, code private. It connects FinTS (bank approval pending), Android Health Connect, Google Calendar, Gmail, Google Maps, weather and AI models; input comes from a journal and tasks. Its core is a deterministic decision engine that plans the day, learns from actual behavior and keeps the plan load at about 70 % expected completion. A language model phrases follow-up questions and maps journal answers; only fixed, reversible rules take effect.

[Screenshots and videos](https://github.com/vassiljevnikita-sudo/life-os-showcase)

### Simple & Light: stock selection by Quality by Design, paper-traded on Trading 212

A fixed rule, Leader5, picks up to five large US stocks (at most 70 % of the account, the rest in an MSCI World ETF) and trades them on a Trading 212 demo account with virtual money: the account since 5 Oct 2026, Leader5 since 12 Oct. It came after a Quality by Design study of 2,790 model families and 1.63 billion prediction rows in which a learned model selection failed its own gates. In backtests on EUR 10,000 Leader5 beat the index fund URTH by a mean EUR 1,658 a year in 2017–2021 and EUR 2,328 a year in 2022–2025; 2022–2025 informed the choice of the rule, so it is not an independent test. Orders are DAY limit orders with exactly-once broker logic; my laptop runs them, and my desktop GPU adds price forecasts over my Tailscale network. The README lists every generation with its result, the failures included.

[Timeline and README](https://github.com/vassiljevnikita-sudo/simple-and-light-research#1-how-it-got-there) · [Demo account and trades](https://simple-light-qbd.expo.app/graphen) · [Start page](https://simple-light-qbd.expo.app/)

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
