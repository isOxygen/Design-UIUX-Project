# Information architecture

| Level | Purpose | Contents |
|---|---|---|
| Service details / Status | Monitor the service | Remaining data and time, status, usage, auto-renew and next renewal |
| Service details / Manage / Get connected | Set up a device | Get config, Subscription link, apps and auto-subscribe, download center |
| Service details / Manage / Management | Maintain account details | Change note |
| Service details / Manage / Upgrade | Adjust the plan when available | Add traffic and Add time |

```mermaid
flowchart LR
    A[Goal: connect another device] --> B[Status]
    B --> C[Manage]
    C --> D[Get config]
    C --> E[Subscription link]
    D --> F[Demo: configuration ready]
    E --> G[Demo: link ready]
    E -.-> H[Link unavailable: retry or return]
    D -.-> I[No compatible config: return to Manage]
    C -.-> J[Inactive service: explain what is unavailable]
```

The dotted branches are design cases. The prototype is expected to demonstrate one recoverable exception; do not infer the remaining branches are implemented. The prototype never exposes a real configuration or link. The four core wireframes are Status, Manage, configuration outcome and subscription-link outcome.

