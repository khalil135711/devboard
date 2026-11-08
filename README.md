# DevBoard

Jira-style ticket board with GitHub, CI/CD and Jitsi Meet links. No build step.

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
