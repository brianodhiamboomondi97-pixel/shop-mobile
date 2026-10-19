# Shop Mobile

Monorepo scaffold for a mobile e-commerce app.

Stack
- Mobile: Expo (React Native) + TypeScript
- Server: Node.js + Express + TypeScript
- Database: PostgreSQL + Prisma
- Payments: Stripe

Quick start (local)
1. Clone
   git clone https://github.com/brianodhiamboomondi97-pixel/shop-mobile.git
   cd shop-mobile

2. Install dependencies
   npm ci

3. Copy env example and set secrets
   cp .env.example .env
   # Edit .env to add DATABASE_URL, STRIPE_SECRET_KEY, JWT_SECRET

4. Start the server
   npm run dev:server

5. Start the Expo app (in another terminal)
   npm run dev:app

What I scaffolded
- /app: Expo starter (App.tsx with a sample product list)
- /server: Express API (sample product endpoints, checkout stub)
- /prisma: Prisma schema for Product model
- CI workflow: type-checking on push/PR
- README and .env.example

Next steps I can do (pick any):
- Wire real Stripe Checkout/session creation on the server
- Add Prisma migrations and seed script, connect a hosted Postgres
- Add auth (email/password + JWT) and protected APIs
- Build a lightweight admin UI for product management
- Create GitHub Actions to run tests and deploy server# shop-mobile
Mobile e-commerce app with Expo frontend and Node/Express backend.
