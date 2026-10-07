# mindstitch.dev

Static landing site for Mindstitch: home page, Terms, Privacy, Refund Policy, 404, `security.txt`.
No build step, no cookies, no analytics, no third-party requests.

## Before publishing

- Fill the yellow `[placeholders]` in `terms.html` and `privacy.html` (company legal name, registration number, address, email provider) once the company is registered.
- Remove the "Draft" boxes after a lawyer has reviewed the legal pages.
- `security.txt` expires 2027-10-01. Renew the date before then.

## Deploy on GitHub Pages

1. Create a public repo `mindstitch/website` and push these files (including `.nojekyll`, `CNAME` and `.well-known/`).
2. Repo → Settings → Pages → Source: Deploy from a branch → `main` / root.
3. Org → Settings → Pages → add and verify `mindstitch.dev` (prevents domain takeover).
4. In Namecheap → Domain List → mindstitch.dev → Advanced DNS, add:

   | Type | Host | Value |
   |---|---|---|
   | A | @ | 185.199.108.153 |
   | A | @ | 185.199.109.153 |
   | A | @ | 185.199.110.153 |
   | A | @ | 185.199.111.153 |
   | CNAME | www | mindstitch.github.io. |

   Remove any Namecheap parking/URL-redirect records for `@` and `www`. Leave the MX and TXT records for Private Email untouched.
5. Back in Pages settings, once the DNS check passes, tick **Enforce HTTPS**.
