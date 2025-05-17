# Next.js and Supabase Starter Kit

<p>
  <a href="#deploy-to-vercel"><strong>Deploy to Vercel</strong></a> ·
  <a href="#clone-and-run-locally"><strong>Clone and run locally</strong></a>
</p>
<br/>

## Features

- Works with the [Next.js](https://nextjs.org) stack
- supabase-ssr. A package to configure Supabase Auth to use cookies
- Styling with [Tailwind CSS](https://tailwindcss.com)
- Components with [shadcn/ui](https://ui.shadcn.com/)
- Deployment with [Supabase Vercel Integration and Vercel deploy](#deploy-your-own)

## Clone and run locally

1. You'll first need a Supabase project which can be made [via the Supabase dashboard](https://database.new)

2. You’ll need to have [bun installed](https://bun.sh/docs/installation)

3. Clone this repository or download it

4. Open the repository in vscode and in the terminal run `bun install`

4. Rename `.env.example` to `.env.local` and update the following:

   ```
   NEXT_PUBLIC_SUPABASE_URL=[INSERT SUPABASE PROJECT URL]
   NEXT_PUBLIC_SUPABASE_ANON_KEY=[INSERT SUPABASE PROJECT API ANON KEY]
   ```

   Both `NEXT_PUBLIC_SUPABASE_URL` and `NEXT_PUBLIC_SUPABASE_ANON_KEY` can be found in [your Supabase project's API settings](https://app.supabase.com/project/_/settings/api)

5. You can now run the Next.js local development server:

   ```bash
   bun dev
   ```

   The template should now be running on [localhost:3000](http://localhost:3000/) and allow you to authenticate users with sign up and sign in.

6. This template comes with the default shadcn/ui style initialized. If you instead want other ui.shadcn styles, delete `components.json` and [re-install shadcn/ui](https://ui.shadcn.com/docs/installation/next)

> Check out [the docs for Local Development](https://supabase.com/docs/guides/getting-started/local-development) to also run Supabase locally.

## Deploy to Vercel

1. Create a vercel account

2. Push this as a new project to Github

3. Click the add new Project button on vercel

4. Select this project from the Git repository

5. Click deploy
