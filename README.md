# DS Furniture & Interior

Luxury inquiry-first showroom built with Next.js App Router, TypeScript, Tailwind CSS v4, React View Transitions, and a custom dark/light/system liquid-glass theme.

## Included

- Home showroom experience with editorial hero, featured pieces, and service routes
- Data-driven collection pages for `chairs-sofas`, `tables`, and `beds-bedroom`
- Thirteen product detail pages seeded from the stitched prototype catalogue
- `Workspace Design` and `Interior Design` service pages
- A contact flow that prepares WhatsApp or email drafts without needing a backend
- Localized premium imagery under `public/images`

## Important Config

Update live contact values in:

- `src/data/site.ts`

Fields to replace:

- `whatsappNumber`
- `contactEmail`
- `showroomAddress`
- `mapUrl`
- optional social links

## Commands

These scripts are configured for the current project structure:

```bash
npm install
npm run dev
npm run lint
npm run build
```

If you are running inside the Codex desktop bundled runtime instead of a system Node install, direct CLI verification was performed with:

```powershell
& "C:\Users\zaing\.cache\codex-runtimes\codex-primary-runtime\dependencies\node\bin\node.exe" ".\node_modules\next\dist\bin\next" build --webpack
```

## Notes

- Production verification in this workspace used `next build --webpack` because Turbopack child-process spawning was blocked by the local Windows runtime.
- `src/app/sitemap.ts` reads `NEXT_PUBLIC_SITE_URL` if you want sitemap URLs to match your final domain.
