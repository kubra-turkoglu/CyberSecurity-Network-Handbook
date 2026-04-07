# CyberSecurity-Network-Handbook
Network Fundamentals for BlueTeam

```mermaid
graph TD
    A[Network Architecture Documentation] --> B[SOHO Networks]
    A --> C[Enterprise Networks]
    A --> D[WAN Networks]
    B --> E[End Devices]
    B --> F[Intermediate Devices]
    C --> E
    C --> F
    D --> E
    D --> F
    E --> G[Laptops]
    E --> H[IoT Hardware]
    F --> I[Routers]
    F --> J[Switches]
    F --> K[Firewalls]
    L[Infrastructure Concepts] --> M[Fault Tolerance]
    L --> N[Scalability]
    L --> O[Quality of Service QoS]
    P[Network Security] --> Q[Protocols]
    P --> R[Ports]
    Q --> S[Admin Usage]
    Q --> T[Attacker Usage]
    R --> S
    R --> T
