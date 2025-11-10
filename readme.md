# University Lost & Found Web App

A dynamic full-stack web app for managing lost and found items at a university.

Stack:
- Backend: Node.js (Express), Prisma ORM, PostgreSQL, JWT auth, Multer for image uploads
- Frontend: React (Vite), React Router
- Dev Database: PostgreSQL via docker-compose

## Features
- User registration and login (JWT)
- Post lost/found items with images
- Browse items with filters
- Submit claims on items
- Approve/reject claims (by item owner or admin)

## Quick Start

### 1) Start PostgreSQL with Docker
```bash
docker compose up -d
```

### 2) Backend setup
```bash
cd server
cp .env.example .env        # set JWT_SECRET and DATABASE_URL if needed
npm install
npx prisma generate
npx prisma migrate dev --name init
npm run dev
```
Server runs at http://localhost:4000

### 3) Frontend setup
```bash
cd client
npm install
npm run dev
```
Frontend runs at http://localhost:5173

## Environment
- Backend `.env`
  - DATABASE_URL="postgresql://postgres:postgres@localhost:5432/lostfound?schema=public"
  - JWT_SECRET="change-me"
  - CLIENT_ORIGIN="http://localhost:5173"

## Scripts
- server
  - `npm run dev` - start dev server with TS
- client
  - `npm run dev` - start vite dev server

## Notes
- Image uploads are stored at `server/uploads/` and served via `/uploads/<filename>`.
- Make the first registered user an admin manually (or via DB) if you want admin moderation.
