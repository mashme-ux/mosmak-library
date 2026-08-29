# Mosmak Library — Next.js + Supabase scaffold

This branch contains a minimal scaffold for the production-ready Mosmak Library app.

What I committed
- Next.js project skeleton
- Tailwind/PostCSS config
- Minimal pages and a Supabase client helper

Next steps I will implement after you provide access
1. Create a Supabase project and provide the anon key + service role key via GitHub repo secrets (recommended) — or invite me as a collaborator.
2. I will implement auth, DB schema (users/items/notes/chats), storage rules, and secure upload/download endpoints.
3. I will set up Vercel automatic deploys and open a PR with a preview URL.

Environment variables (.env.local)

NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
SUPABASE_SERVICE_ROLE_KEY=your_service_role_key  # server-side only, never expose to browser

How to run locally

1. npm install
2. copy .env.example to .env.local and fill values
3. npm run dev

When you're ready to proceed with full-managed mode (I will wire Supabase & Vercel), reply here and:
- Create a Supabase project and add the anon key in repo secrets as NEXT_PUBLIC_SUPABASE_ANON_KEY and NEXT_PUBLIC_SUPABASE_URL
- Add SUPABASE_SERVICE_ROLE_KEY as a repo secret (server-side only)
- Connect the repository to Vercel and add the same secrets in Vercel environment variables

I will not commit any secrets to the repo.
