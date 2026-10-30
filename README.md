# Nikita Vassiljev

Pharmacy student at FU Berlin (semester 7 of 8) and working student in pharmaceutical quality assurance. I build software for QA work with AI coding agents: I set the requirements and acceptance checks, the agents write the code and tests, and CI runs the tests on every change.

## Projects

### Complaint Dossier

A PowerShell workflow that drafts a complaint trend report in Word, for example as input to a product quality review. The report stays marked DRAFT until a reviewer approves it. The workflow reads complaint cases from Excel, computes the statistics and builds the prompt for the Microsoft 365 Copilot desktop app, which drafts the assessment text. An audit log with SHA-256 hashes covers every input and output. `./Invoke-ComplaintDossier.ps1 -Demo` runs on synthetic cases with a prewritten sample answer instead of Copilot, and CI runs it on every push. The live Copilot round trip is not yet confirmed end to end. The project is a public rebuild of a prototype from my working-student job, made with synthetic data and a neutral template; it contains no company material. Designed along GAMP 5 principles; not validated.

[Repo](https://github.com/vassiljevnikita-sudo/complaint-dossier) · [Design note (GAMP 5)](https://github.com/vassiljevnikita-sudo/complaint-dossier/blob/main/docs/design-note.md) · [Sample report (PDF)](https://github.com/vassiljevnikita-sudo/complaint-dossier/blob/main/docs/sample/complaint-dossier-sample-DRAFT.pdf) · [CI runs](https://github.com/vassiljevnikita-sudo/complaint-dossier/actions)

### Stock-selection research: chronological model evaluation

Python research on how to train and select stock-selection models over time without using information from the future. It evaluates 2,790 model families chronologically on 1.63 billion prediction rows with known outcomes from 2016 to 2025. Each experiment fixes its pass/fail criteria before it runs. No tested method for choosing between models met all of them, and the repo documents what failed and why. The final test period has not been evaluated yet, and no real capital is involved.

[Demo](https://simple-light-qbd.expo.app/) · [Repo](https://github.com/vassiljevnikita-sudo/simple-and-light-research)

### Questify

A to-do app in German where finished tasks earn XP and levels, and friends compete on weekly and monthly leaderboards. I built it with AI coding agents. It is released as an Android APK and as a web app; the source code is private, the repo holds the APK releases.

[Open the app](https://mastertasker.expo.app/willkommen/) · [Releases repo](https://github.com/vassiljevnikita-sudo/questify-releases)

### portfolio-check

Every morning it checks that project links, demo pages, READMEs and CI work for a logged-out visitor, and it scans my public repos for secrets and confidential employer terms. [Repo](https://github.com/vassiljevnikita-sudo/portfolio-check)

## Publication

Jones E, Vassiljev N. Zukunft der Pharmazie: Welche Kompetenzen brauchen Apotheker*innen? Die Perspektive der Studierenden auf Studium und Approbationsordnung [The future of pharmacy: What knowledge and skills do pharmacists need? The students' perspective on the curriculum and licensing regulations for pharmacists]. *Bundesgesundheitsblatt* 68(5), 519–525 (2025). [doi:10.1007/s00103-025-04050-4](https://doi.org/10.1007/s00103-025-04050-4) · [Google Scholar](https://scholar.google.com/citations?user=4rua7qYAAAAJ)

## Availability

Up to 15 hours a week from 1 Feb to 30 Jun 2027, full-time from 15 Sep 2027.

## Contact

[vassiljev.nikita@gmail.com](mailto:vassiljev.nikita@gmail.com)
