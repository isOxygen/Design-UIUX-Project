# Design decisions and trade-offs

| Decision | Evidence | Alternative | Expected effect and open question |
|---|---|---|---|
| Separate Status and Manage | Two implemented screens show distinct information and actions. | One scrolling page | Monitoring and service actions no longer compete in the same view. The trade-off is one tap to switch goals. |
| Put connection actions first on Manage | The captured screen groups both actions under Get connected. | Put Upgrade first or hide setup in a menu | Easier access for a new-device task. Will users distinguish a single config from a subscription link? |
| Keep Upgrade together and secondary | Both upgrade options are separate from setup in the captured UI. | Add independent actions to Status | Keeps monitoring quiet without hiding plan changes. Can a subscriber still find upgrades when they need them? |

These are rationale entries, not three participant-led iteration records. Research is still needed to distinguish an obvious structure to its author from a quick route for a first-time viewer.

**Accessibility risks to check:** Gauges cannot be the only way to tell data from time; retain numbers and labels. Use visible focus plus an explicit selected state for tabs. Pair any failure message with an actionable Retry or Back path and keep status text readable at narrow widths.
