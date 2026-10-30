# Nikita Vassiljev

Pharmacy student at FU Berlin (semester 7 of 8) and working student in pharmaceutical quality assurance. I build software with AI coding agents and check their output with tests and CI.

## Projects

### Complaint Dossier

A public rebuild of a prototype from my working-student job, made with synthetic data and a neutral template; it contains no company material. The PowerShell workflow reads complaint cases from Excel, computes the statistics, builds the prompt for the Microsoft 365 Copilot desktop app and writes a Word report that stays marked DRAFT until a reviewer signs it. A JSON audit log records SHA-256 hashes of inputs and outputs. `./Invoke-ComplaintDossier.ps1 -Demo` runs on synthetic cases with a recorded answer, and CI runs it on every push. The live Copilot round trip is not yet confirmed end to end. Designed along GAMP 5 principles; not validated.

[Repo](https://github.com/vassiljevnikita-sudo/complaint-dossier) · [Design note (GAMP 5)](https://github.com/vassiljevnikita-sudo/complaint-dossier/blob/main/docs/design-note.md) · [Sample report (PDF)](https://github.com/vassiljevnikita-sudo/complaint-dossier/blob/main/docs/sample/complaint-dossier-sample-DRAFT.pdf) · [CI runs](https://github.com/vassiljevnikita-sudo/complaint-dossier/actions)

### Stock-selection research without future information

Python research on how to train and select stock-selection models over time without using information from the future. It evaluates 2,790 model families chronologically on 1.63 billion prediction rows with known outcomes from 2016 to 2025. Each experiment fixes its pass/fail criteria before it runs. No tested method for choosing between models met them, and the repo documents what failed and why. The final holdout period is still closed, and no real capital is involved.

[Demo](https://simple-light-qbd.expo.app/) · [Repo](https://github.com/vassiljevnikita-sudo/simple-and-light-research)

### Questify

A to-do app in German where finished tasks earn XP and levels, and friends compete on a season leaderboard. I built it with AI coding agents. It is released as an Android APK and as a web app; the source code is private, the repo holds the APK releases.

[Open the app](https://mastertasker.expo.app/willkommen/) · [Releases repo](https://github.com/vassiljevnikita-sudo/questify-releases)

### portfolio-check

Checks every morning, logged out, that the project links, demo pages, READMEs and CI work, and scans the public repos for secrets and confidential employer terms. [Repo](https://github.com/vassiljevnikita-sudo/portfolio-check)

## Publication

Jones E, Vassiljev N. Zukunft der Pharmazie: Welche Kompetenzen brauchen Apotheker*innen? Die Perspektive der Studierenden auf Studium und Approbationsordnung. *Bundesgesundheitsblatt* 68(5), 519–525 (2025). [doi:10.1007/s00103-025-04050-4](https://doi.org/10.1007/s00103-025-04050-4) · [Google Scholar](https://scholar.google.com/citations?user=4rua7qYAAAAJ)

## Availability

Full-time from 15 Feb to 11 Apr 2027, up to 20 hours a week from 12 Apr 2027, and full-time from 18 Jul 2027.

## Contact

[vassiljev.nikita@gmail.com](mailto:vassiljev.nikita@gmail.com)
