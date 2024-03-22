# Schedule

### Backend

- [ ] pnpm workspace
- [ ] monorepo (Turborepo or Nx?)
- [ ] Nestjs
- [ ] logging with Pino
- [ ] Swagger for API documentation
- [ ] testing with Jest
- [ ] Fastify
- [ ] GraphQL
- [ ] API versioning
- [ ] Drizzle
- [ ] Supabase (database, auth, storage)
- [ ] KeyDB/Dragonfly cache (Redis alternative)
- [ ] rate limiting with KeyDB/Dragonfly
- [ ] Memphis.dev (queue alternative to Kafka/Bullmq/RabbitMQ, ...)
- [ ] ElectricSQL as localfirst sync integraded with Supabase

---

### Frontend

- [ ] Next.js
- [ ] TailwindCSS
- [ ] Shadcn
- [ ] Auth JWT with action token and refresh token

---

### Base, repo, automation

- [ ] CI/CD (Github Actions)
- [ ] linting, etc... and Biome
- [ ] Storybook
- [ ] Dockerize

---

### Models / CRUD

- [ ] Users
- [ ] Workspaces
- [ ] Tasks
- [ ] Projects
- [ ] Notes
- [ ] Timesheets
- [ ] Toast notifications
- [ ] Realtime updates
- [ ] Websockets???????
- [ ] App updates with git hash versioning

---

### Schema

```mermaid
graph TD;
  subgraph "Frontend"
    A[Next.js Frontend] --> B[Login Page]
    A --> C[Signup Page]
    A --> D[Dashboard]
    style B,C,D fill:#0b6b00,stroke:#0b6b00,stroke-width:4px
  end
  subgraph "Backend"
    E[NestJS with Fastify API Backend] --> F[Authentication & Authorization]
    E --> G[CRUD Operations for Tasks]
    F --> H[JWT Tokens]
    G --> I[Supabase Database]
    style F,H,G fill:#85007c,stroke:#85007c,stroke-width:4px
  end
  subgraph "Database"
    I[Supabase Database] --> J[Users Table]
    I --> K[Tasks Table]
    style J,K fill:#00328f,stroke:#00328f,stroke-width:4px
  end
  subgraph "Auth with JWT Refresh Tokens"
    F --> L[Token Generation & Refresh]
    style L fill:#f00,stroke:#f00,stroke-width:4px
  end
  subgraph "Security Considerations"
    B --> M[Secure Storage]
    E --> N[Input Validation & Sanitization]
    N --> O[HTTPS Communication]
    style M,N,O fill:#bd6202,stroke:#bd6202,stroke-width:4px
  end

```

---

### Links & information

- [Rokas Dam](https://github.com/devRokas)
- [Rokas Dam nestjs starter - Nestjs + Supabase (no fastify, no drizzle, no auth)](https://github.com/devRokas/supabase-nestjs-rest-api-starter-kit)
- [Sakura Dev - video 1: Nestjs with Prisma and Nextauth](https://www.youtube.com/watch?v=khNwrFJ-Xqs)
- [Sakura Dev - Video 2: refactoring Nestjs with Drizzle](https://www.youtube.com/watch?v=l1DGXmmgZ9w)
- [NestJS](https://nestjs.com/)
- [Fastify](https://www.fastify.io/)
- [Pino](https://getpino.io/)
- [Memphis.dev](https://memphis.dev/)
- [KeyDB](https://keydb.dev/)
- [Dragonfly](https://dragonflydb.com/)
- [Supabase](https://supabase.io/)
- [ElectricSQL](https://electricsql.com/)
- [ElectricSQL integration Supabase](https://supabase.com/partners/integrations/electricsql)
- [Shadcn](https://shadcn.com/)
- [Drizzleorm](https://drizzleorm.com/)
- [pnpm](https://pnpm.io/)
