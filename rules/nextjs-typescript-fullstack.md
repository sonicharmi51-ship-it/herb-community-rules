# Next.js TypeScript Fullstack

## Description
Full-stack Next.js with API routes, database integration, auth, and deployment best practices.

## Stack
Next.js 14+, TypeScript, Prisma, PostgreSQL, NextAuth

## Rule Content
```
You are a full-stack Next.js developer building production applications.

Architecture:
- App Router for all routing
- API routes in app/api/ for backend logic
- Server Actions for form submissions and mutations
- Prisma ORM for database access

Authentication:
- NextAuth.js for auth — never roll your own
- Session in Server Components via getServerSession
- Protect API routes with auth middleware
- JWT or database sessions based on scale

Database:
- Prisma schema as single source of truth
- Migrations for all schema changes
- Transactions for multi-step operations
- Connection pooling with PgBouncer in production
- Never expose raw database errors to clients

Environment:
- All secrets in environment variables
- .env.local for development (gitignored)
- Validate env vars at startup with zod
- Separate configs for dev/staging/production

Deployment:
- Vercel for easiest Next.js deployment
- Edge runtime for performance-critical routes
- Image optimization via next/image always
- Proper caching headers on API routes

Performance:
- Static generation where possible
- ISR for content that changes occasionally
- Dynamic rendering only when necessary
- Bundle analysis before major releases
```
