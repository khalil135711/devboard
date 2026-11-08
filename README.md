# DevBoard

Jira-style ticket board with GitHub, CI/CD and Jitsi Meet links. No build step.
<img width="1916" height="881" alt="Bildschirmfoto 2026-11-08 um 17 43 05" src="https://github.com/user-attachments/assets/b24143e1-8436-4bc8-a408-e5158e87b31f" />

<img width="1916" height="881" alt="Bildschirmfoto 2026-11-08 um 17 43 15" src="https://github.com/user-attachments/assets/3dabfa0c-9e17-4e3d-84e5-5827f87fa96a" />

## Run
Open `index.html` in a browser, or serve the folder:

    python3 -m http.server 8080

## Setup
1. Open Settings, enter your repository as `owner/name` and a ticket prefix (for example DEV).
2. Copy `.github/workflows/ci.yml` into your repository.
3. Name branches like `DEV-12-fix-login` so each ticket's "CI runs" link filters GitHub Actions to its branch.

## Notes
- Tickets are saved in the browser (localStorage). Use Export JSON / Import JSON to move them.
- Meet links open https://meet.jit.si/<room-prefix>-<ticket-key> in a new tab.
- CI status is set manually on each ticket.
