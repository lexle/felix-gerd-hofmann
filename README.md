# felix-gerd-hofmann.de

Static portfolio site. Plain HTML and one stylesheet, no build step, no JavaScript, no cookies,
no third-party requests. Fonts (Newsreader, IBM Plex Sans/Mono, SIL OFL) and photos are self-hosted.

```
public/
  index.html            Home: hero, numbers, selected work, AI, energy, record
  about.html            Story, how I work, energy thread, full record, education
  contact.html
  impressum.html        Impressum + Datenschutz (German law requires both on a .de site)
  work/douglas.html     Case study 01
  work/wiwin.html       Case study 02
  work/trusted-shops.html  Case study 03
  work/redline.html     Case study 04
  assets/site.css
  assets/fonts/  assets/img/
firebase.json           Hosting config: clean URLs, cache + security headers
.firebaserc             GCP/Firebase project: portfolio-fgh
LOVABLE.md              Prompt + copy to rebuild the site as a Lovable demo
```

## Preview locally

```bash
npx --yes serve public
```

`serve` handles clean URLs (`/about` → `about.html`) the same way Firebase does.

## Deploy to Google Cloud (Firebase Hosting, project `portfolio-fgh`)

Firebase Hosting runs inside the Google Cloud project, is free at this size, and issues the SSL
certificate for the custom domain automatically. A Cloud Storage bucket behind a load balancer would
also work but costs roughly €18+/month for the load balancer alone.

1. Log in (opens a browser):
   ```bash
   npx --yes firebase-tools login
   ```
2. Enable Firebase on the existing GCP project (once; skip if the Firebase console already shows it):
   ```bash
   npx --yes firebase-tools projects:addfirebase portfolio-fgh
   ```
3. Deploy:
   ```bash
   npx --yes firebase-tools deploy --only hosting
   ```
   The site is then live at https://portfolio-fgh.web.app.

## Connect felix-gerd-hofmann.de (DNS at hosting.de)

1. Firebase console → project `portfolio-fgh` → Hosting → **Add custom domain** →
   `felix-gerd-hofmann.de`. Then add `www.felix-gerd-hofmann.de` and set it to redirect to the apex.
2. The console shows the records to create. Enter exactly those values in the hosting.de DNS zone
   editor for `felix-gerd-hofmann.de`:
   - a **TXT** record on `@` for ownership verification
   - the **A** record(s) on `@` that Firebase lists
   - for `www`, the record Firebase lists (usually a CNAME to `portfolio-fgh.web.app`)
3. **Delete** any existing A/AAAA records on `@` and `www` (for example hosting.de's default
   parking records). If an old record stays in place, certificate issuance hangs.
4. Wait. Verification plus the SSL certificate usually takes from a few minutes to a few hours,
   occasionally up to 24 hours.

## Before going live, check

- Impressum address and email are correct (it's a legal page, so the address is public by law).
- The Sonova description on Home/About is cleared for public use.
- You're fine naming Redline publicly and describing its unfinished status.
