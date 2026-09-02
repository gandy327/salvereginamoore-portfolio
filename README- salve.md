# Salve Moore — Portfolio Website

One file. `index.html` contains the page, the styling and every photograph.
There is no `images` folder to upload and nothing else to keep track of.

## Put it live on GitHub Pages

1. Create a new **public** repository, e.g. `salvemoore-portfolio`.
2. Upload `index.html` to the root of the repo (drag and drop on github.com works).
3. Go to **Settings → Pages**.
4. Under *Build and deployment* set **Source: Deploy from a branch**, **Branch: `main`**, **Folder: `/ (root)`**, then Save.
5. Wait about a minute. The site is live at
   `https://<username>.github.io/salvemoore-portfolio/`

For the shorter `https://<username>.github.io/` address, name the repository exactly `<username>.github.io`.

## What's on the page

| Section | Photograph |
|---|---|
| Hero | Cut-out portrait, with the European Escape flyer as an overlapping card |
| Work | Ten real campaign pieces — travel flyers, AEA Jewellery product ads, Yours Truly wedding promos, UGC content |
| Experience | Salve in front of a wall of client sites and landing pages |
| Contact | Salve on a client call |

Tapping any piece in the Work grid opens it full size. Escape, the × or a click outside closes it.

## Editing

Open `index.html` in any text editor. The images are stored as long `data:image/webp;base64,...`
strings — ignore those lines, all the text sits around them.

| What to change | Search for |
|---|---|
| Portfolio deck link | `canva.link/salvemooreportfolio` (4 places) |
| Email | `avzmoorenew@gmail.com` |
| Phone / Viber | `639524401181` |
| Headline | The `<h1>` inside `<section class="hero">` |
| Services | The `<div class="svc">` block |
| Industries | The `<ul class="tags">` list — `class="on"` makes a tag navy |
| Colours | The `:root { }` block at the top of the `<style>` section |

### Swapping or adding a photo

Because the images are embedded, you cannot just drop a new file in a folder. Either send the
new photo to be re-embedded, or host it somewhere (Imgur, Cloudinary, a GitHub `images` folder)
and replace the whole `src="data:image/webp;base64,..."` value with `src="https://your-url.jpg"`.

## Trade-off worth knowing

Embedding makes the file about 750 KB, so the first visit downloads a little more up front than a
normal site would, and link previews on Facebook or LinkedIn will not show a thumbnail (previews
cannot read embedded images). In exchange there is only one file to manage and no broken-image
risk. If the site later grows, moving the photos into a real `images/` folder is the upgrade path.

## Notes on the copy

Every claim comes from the CV and portfolio deck: 7+ years, the 2019–June 2026 role at Explore The
World Travel and Tours, the multi-client scope, certifications and industries. No performance
percentages are presented as client results — the reporting section lists *which* metrics get
reported rather than claiming figures, so the page holds up if a prospect asks for proof. Real,
verifiable campaign numbers with the client and period named would make it stronger still.

## Design

- Deep navy `#0C1B36`, sand `#EFE2CB`, paper `#FBF6EC`, gold `#C9992E` — carried over from the existing portfolio deck.
- Type: Bricolage Grotesque (display) and Instrument Sans (body), from Google Fonts.
- Responsive to mobile, keyboard focus visible, `prefers-reduced-motion` respected.
