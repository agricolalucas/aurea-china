# Aurea China

Copied from `agricolalucas/aurea-india` to an independent Supabase project `xnjusxpyguqqujpbwkot`.

## Current status

- `index.html` copied with China Supabase URL and publishable key; India branding partly replaced.
- `schema.sql` applied: 11 base tables with RLS, initially empty.
- Login is backed by Supabase Auth and `india_members` membership policies inherited from India.
- The intended admin email `comercial@aureainternacional.com` was **not present in this China project's auth.users** at last verification. Create/invite it in this project, confirm the email, and assign membership using its real UUID: `insert into public.india_members(user_id, role) values ('REAL_AUTH_UUID','admin');`
- India-specific table names, INR fields, and parts of the UI remain; China-specific adaptation and any missing tables need separate migration.
- No production site has been published or tested. GitHub Pages must be configured before there is a working site URL.

**Do not enter real business data until authorization, RLS and the remaining modules are validated.** Do not commit passwords or secret/service-role keys.
