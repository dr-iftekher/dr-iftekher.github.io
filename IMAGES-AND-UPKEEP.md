# Images & Upkeep — A Working Guide
### Dr. Md Iftekher Iqbal · driftekheriqbal.com

---

## PART 1 — Making the header photographs look professional

### The three specifications that matter

| | Header photos (`hero-*.jpg`) | Portrait (`photo.jpg`) |
|---|---|---|
| Dimensions | **1920 × 1080 px** (16:9) | **800 × 800 px** (square) |
| File size | **under 400 KB** | under 200 KB |
| Format | JPG, sRGB colour | JPG, sRGB colour |

**File size is not a detail.** The reference photographs you sent are 4–6 MB each. On a 4G connection in Dhaka, one such file takes several seconds to appear; six of them make the site feel broken. Compressed to 300–400 KB, the same photograph looks identical on screen and loads instantly. This single step does more for the "professional" impression than any amount of retouching.

**To compress:** open **squoosh.app** in your browser (works on phone and desktop, free, no signup). Drop the photo in, set the right panel to **MozJPEG**, drag quality to around **75**, set **Resize → width 1920**, and download. Watch the file-size readout at the bottom until it sits under 400 KB.

### Composition — where the subject should sit

The header darkens from left to right, because your text sits on the left. So:

- **Put the subject in the right half of the frame.** A photo with your face dead-centre will have it partly buried under the dark veil.
- **Leave the left third comparatively empty** — a wall, an out-of-focus background, the drape of a surgical field. That emptiness is where your name goes.
- **Shoot or crop wide.** The header crops to fill, so a tight portrait loses its edges. Give the frame air.

### Two new controls I've built into the stylesheet

If a photograph still doesn't sit right, you can now fix it by adding a word to the page's `<header>` line — no image editing needed.

**To move the visible area** (when the crop cuts off the wrong part):

```html
<header class="hero hero--page hero--about focus-right">
```

Available: `focus-left`, `focus-right`, `focus-top`, `focus-bottom`, `focus-top-left`, `focus-top-right`

**To darken or lighten the veil** (when text is hard to read over a busy photo):

```html
<header class="hero hero--page hero--about veil-strong">
```

Available: `veil-strong` (busy or bright photos), `veil-soft` (dark, simple photos)

**Combine them freely:**

```html
<header class="hero hero--page hero--about focus-right veil-strong">
```

Change nothing and the defaults apply, which suit most photographs.

### What makes a clinical photograph read as vibrant rather than flat

- **Light from the side, not the front.** Overhead OR lighting flattens faces. A window or a light to one side gives shape.
- **One clear subject.** A photo of you at the microscope reads instantly. A photo of six people at a booth reads as nothing.
- **Correct the white balance.** Operating theatres push everything green or blue. Even a phone editor's "warmth" slider, nudged slightly, transforms the result.
- **Lift contrast a little, saturation barely.** Oversaturated medical images look amateur and, in a clinical context, slightly untrustworthy.
- **Shoot in landscape.** Always, for headers.

### Before you upload any image

- Use only photographs **you own**. Images published by The Ophthalmologist, CAKE Magazine, or Media MICE belong to those publishers even when you are the subject.
- **No patient-identifiable content** without documented consent. A bare anterior segment view is generally not identifiable; a periocular view including facial features usually is.
- Keep to your standing image-integrity practice — no manipulation beyond global exposure, white balance, and cropping.

---

## PART 2 — Keeping the site current

### The rhythm

| When | What to do |
|---|---|
| **Each new publication** | Add to `research.html` **and** `research-bn.html`; update the "10+" figure if it crosses a round number |
| **Each new award, faculty invitation, or media feature** | Add to `about.html` + `about-bn.html` (Recognition and Milestones); add media items to `teaching.html` + `teaching-bn.html` |
| **Every 3 months** | Check the four pinned films on the teaching pages still play; refresh one header photograph |
| **Every 6 months** | Re-read the biography — has the interventional glaucoma story moved on? Verify chamber days, hours, and all phone numbers |
| **Annually** | Confirm domain auto-renew is on at Namecheap; confirm the `CNAME` file is still in the repository |

### The rule that prevents every inconsistency

**Two files, one fact.** Every change to a fact happens twice — once in `page.html` and once in `page-bn.html`. Chamber hours, phone numbers, a new award, a swapped film. If you only have time to update one language, update both or neither; a patient reading the Bangla page and arriving an hour early is worse than a slightly stale site.

### How to make an edit

1. github.com → your repository → click the file
2. Pencil icon ✏️ → find the `EDIT HERE` comment for that section
3. Change the text between tags, never the tags themselves
4. **Commit changes** → live in 1–2 minutes

Every previous version is kept. Click "History" on any file to restore one. You cannot permanently break anything.

### Things that never need editing again

- **The homepage featured film** — it plays the newest item in your `MIIQ - Featured Surgical Films` playlist. Reorder that playlist on YouTube to change what leads.
- **Copyright year, hosting, HTTPS certificate** — all handled automatically.

### One standing caution

The four pinned films on the teaching pages are fixed references. If you make one private, unlisted, or delete it, that slot shows an error box. Whenever you reorganise your channel, glance at `driftekheriqbal.com/teaching.html` afterwards.
