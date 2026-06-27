# Real Estate Listing Portal (starter)

Stack:
- Next.js (TypeScript)
- Prisma (PostgreSQL)
- TailwindCSS (optional)
- Cloudinary for images (or local uploads)
- Docker Compose for Postgres

Quick start (local)
1. Clone repo
2. Copy .env.example to .env and set DATABASE_URL, CLOUDINARY_* keys
3. Start Postgres:
   docker-compose up -d
4. Install and generate Prisma client:
   pnpm install    # or npm/yarn
   npx prisma migrate dev --name init
   npx prisma db seed
5. Start dev server:
   pnpm dev

Notes
- Add authentication (NextAuth) for user/agent flows.
- Replace Cloudinary with S3 if you prefer.