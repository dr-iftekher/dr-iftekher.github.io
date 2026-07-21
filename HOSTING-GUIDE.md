# Put Your Multi-Page Website Online — Free, Secure, Editable
### Step-by-step for Dr. Md Iftekher Iqbal (no technical knowledge needed)

---

## PART 1 — Go live on GitHub Pages (one time, ~15 minutes)

**Why GitHub Pages:** free forever, no ads, no expiry, automatic HTTPS security (the padlock), owned by Microsoft, trusted by millions of professionals. Your site is "static" — no logins, no database — so there is essentially nothing to hack.

1. **Create a free account** at **github.com** → Sign up. Suggested username: **dr-iftekher** (it becomes your web address).
2. **Create the repository:** click **+** (top right) → **New repository** → name it exactly **dr-iftekher.github.io** (your username + `.github.io`) → keep **Public** → **Create repository**.
3. **Upload the site:** on a computer, unzip the website folder, click **"uploading an existing file"** on the repository page, and drag in **everything inside the folder** — all six .html files, the **css** folder, and the **img** folder together. Click **Commit changes**.
   *(Doing this from a computer is much easier than from a phone — a one-time task.)*
4. **Wait 2–3 minutes.** Your site is live at **https://dr-iftekher.github.io** with HTTPS already active.

---

## PART 2 — Editing later (any device, any time)

1. Log in at github.com → open your repository → click the file (e.g., `research.html`)
2. Click the **pencil icon** ✏️ → find the `EDIT HERE` comment for that section
3. Change the text between tags (never delete the tags) → **Commit changes**
4. The live site updates in 1–2 minutes

| Task | File & section |
|---|---|
| Add a new publication | `research.html` → EDIT HERE: PUBLICATIONS (copy one `<li>` block to the top) |
| Change chamber days/times/phones | `appointments.html` → EDIT HERE: CHAMBER DETAILS |
| Swap a featured video | `index.html` or `teaching.html` → replace the code after `embed/` |
| Add an award or milestone | `about.html` → RECOGNITION or TIMELINE sections |
| Add a new named technique | `innovations.html` → copy one card block |
| Change brand colours everywhere | `css/style.css` → the `:root` block at the top |
| Update your numbers | `index.html` → stats strip |

**Mistake-proof:** GitHub keeps every version. Click "History" on any file to restore an older one. You cannot permanently break anything.

**Shortcut:** you can always upload a file to Claude, describe the change in plain words, and put the returned file back on GitHub.

---

## PART 3 — Adding your photographs (this is what completes the look)

Each page header is designed to hold one of your own photographs — your OR photos at the ZEISS Lumera, conference lectures, mentoring moments. The branded gold artwork shows until you add them.

1. In your repository, open the **img** folder → **Add file → Upload files**
2. Upload wide photos (1600px+) named **exactly**:
   `hero-home.jpg`, `hero-about.jpg`, `hero-innovations.jpg`, `hero-research.jpg`, `hero-teaching.jpg`, `hero-appointments.jpg`
3. Also upload **photo.jpg** (a square portrait) to the main folder
4. That's all — each photo appears automatically behind its page header, with the dark overlay keeping the text readable. Only use images you own; never patient-identifiable images without documented consent.

Suggested pairings: OR action shot (Home) · portrait or lecture (About) · gonioscopy/surgical close-up you own (Innovations) · desk or conference poster (Research) · teaching or recording setup (Teaching) · hospital exterior (Appointments).

---

## PART 4 — Optional, later

- **Custom domain** (e.g., driftekher.com): the only thing that ever costs money (~USD 10–12/year for the name; hosting stays free). Buy from Namecheap or Cloudflare → repository **Settings → Pages → Custom domain** → tick **Enforce HTTPS**.
- **Account security:** turn on two-factor authentication in GitHub Settings — that protects the one thing worth protecting.
- **Backup:** keep a copy of the whole website folder in Google Drive. Those files are the entire website.
- **Keep msha.ke:** it remains your link hub for social bios; add your new official site link to it and to your visiting-card QR.
