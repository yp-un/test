# test


```mermaid
flowchart LR
  U[User Browser]
  M[next-intl Middleware]
  A[Next.js App Router]
  Q[React Query / Axios]
  B[Spring REST API]
  W[Spring WebSocket + STOMP]
  C[R2 / CDN]

  U --> M
  M --> A
  A --> Q
  Q --> B
  A <-->|STOMP| W
  A --> C
```