# DLSP case study

## The decision
A returning VPN subscriber may need to check how much data or time is left, or to set up another device. The implemented mobile interface splits those goals. Status keeps usage, validity and renewal information together. Manage puts **Get config** and **Subscription link** first, then app help, notes and upgrades. **Add traffic** and **Add time** stay together under Upgrade.

<table><tr><th>Status: monitor</th><th>Manage: act</th></tr><tr><td><img src="assets/status.jpg" alt="Status tab showing usage and time remaining" width="250"></td><td><img src="assets/manage.jpg" alt="Manage tab showing configuration and subscription actions" width="250"></td></tr></table>

These are two current screens of the same service, not a before/after pair. Service identifiers were masked; the full screenshot frame was retained. The split was implemented before the course. The split keeps monitoring and service actions from getting mixed together. That gives each view a clear purpose, especially when setup may involve different protocols or devices. Less scrolling is one benefit of keeping unrelated controls out of the way. Informal feedback from live users supported keeping the two views separate.

## Evidence and design
- [Architecture and task flow](docs/architecture.md)
- [Decisions, trade-offs and risks](docs/decisions.md)
- [Wireframes and view rules](docs/wireframes.md)
- [Testing plan and results boundary](docs/validation.md)
- [Project timeline](docs/timeline.md)
