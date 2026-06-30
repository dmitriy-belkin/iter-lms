# ITER-LMS

Learning platform demo: courses, chapters, video lessons, progress, and Stripe checkout.

**Stack:** Next.js 14 · React 18 · TypeScript · Prisma · PostgreSQL · Tailwind · Clerk auth · Mux video · Stripe · UploadThing

## Features

- Course catalog with categories and drag-and-drop chapter ordering
- Mux-powered video player for lessons
- Student progress tracking and analytics charts
- Stripe payments for paid courses
- Teacher dashboard for content management

## Prerequisites

- Node.js 18+
- PostgreSQL database
- Accounts / keys for [Clerk](https://clerk.com), [Mux](https://mux.com), [Stripe](https://stripe.com), and [UploadThing](https://uploadthing.com) (see `.env.example` patterns in repo)

## Quick start

```bash
npm install
cp .env.example .env.local   # fill in keys and DATABASE_URL
npx prisma generate
npx prisma db push
node scripts/seed.ts           # optional: seed categories
npm run dev
```

Open [http://localhost:3000](http://localhost:3000).

## Scripts

| Command | Description |
|---------|-------------|
| `npm run dev` | Development server |
| `npm run build` | Production build |
| `npm run start` | Start production server |
| `npm run lint` | ESLint |

## License

MIT — sample / portfolio project.
