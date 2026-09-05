# College Clubs Portal

A responsive college clubs and events portal built with HTML, CSS, JavaScript, Express, JWT, and MongoDB models.

## Run locally

1. Install Node.js 18+.
2. Run `npm install`.
3. Copy `.env.example` to `.env` and set `JWT_SECRET` and (optionally) `MONGODB_URI`.
4. Run `npm start` or `npm run dev`. If PowerShell blocks the `npm` script on Windows, run `npm.cmd start` or double-click `run-website.cmd`.
5. Open http://localhost:3000 locally, or https://kongunadu.club.in after deployment.

The demo works without MongoDB using seeded in-memory data. When MongoDB is available, models in `backend/models` are ready for persistence. Demo login: use any email and password on the sign-in screen; the UI demonstrates the portal flow. Production deployments should enable the database connection and use a real user store.

## API

`/api/auth/register`, `/api/auth/login`, `/api/clubs`, `/api/clubs/:id/join`, `/api/clubs/:id/leave`, `/api/events`, `/api/events/:id/register`, `/api/events/:id/register`, `/api/users/profile`. Admin mutations require a JWT with an admin role.
