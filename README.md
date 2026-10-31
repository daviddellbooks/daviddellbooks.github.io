# The Watchers Among Us: book site

Static landing site for **The Watchers Among Us: Unveiling the Spiritual Truth of the UFO Phenomenon** by David Dell.

- Kindle: https://www.amazon.com/dp/B0DYY7GZ7S
- Paperback: https://www.amazon.com/dp/B0DYYMQYPJ
- Site URL (once deployed): https://daviddellbooks.github.io/

## What's here

| Path | What it is |
|---|---|
| `index.html`, `style.css` | Landing page: the verbatim Amazon description (labeled), the book's case in short (description points only), both Amazon links, our own clearly labeled commentary sections, the title-collision note and schema.org `Book` JSON-LD |
| `guide/watchers-in-scripture.html` + `guide/guide.css` | Free companion reading guide "Watchers in Scripture": KJV passages on the unseen realm, angels, fallen angels, Ezekiel's wheels and discernment, with discussion questions. It's a general study aid, not a summary of the book. |
| `guide/watchers-in-scripture.pdf` | Printable Letter-size PDF of the guide (Chrome print-to-PDF of the HTML) |
| `assets/hero.jpg`, `assets/og-image.png`, `assets/favicon.png` | Original, code-generated art (no stock or third-party images) |
| `assets/fonts/Cinzel-VariableFont_wght.ttf` + `OFL-Cinzel.txt` | Heading font, SIL Open Font License 1.1 (license file included as required) |
| `robots.txt` | Allows all crawlers |

Plain HTML/CSS: no build step, no JavaScript, no cookies, **no trackers or analytics**. Every internal link and asset path is relative, so the folder works as-is at the site root. Outbound links go only to Amazon, BibleGateway (KJV passages) and the public sources cited on the page.

## Content rules

- Claims about the book use only its Amazon description (quoted verbatim) and its core view, presented as the book's view.
- Genesis 6, 1 Enoch and the 2023 hearing appear only in sections labeled as our own commentary.
- Prices (Kindle $4.99, paperback $12.99) and Kindle+ (formerly Kindle Unlimited) enrollment were verified on Oct 30, 2026. They appear as visible text with "prices may change; see Amazon" inside the marked `PRICE/KINDLE+ BLOCK` in the hero and in the bottom note. They are deliberately left out of the JSON-LD.

## SEO

- `canonical`, `og:url`, `og:image` and `twitter:image` use absolute URLs on https://daviddellbooks.github.io/.
- JSON-LD uses only verified fields: name, subtitle, author, description excerpt, ASINs, paperback ISBN-13 979-8312378887, publication dates (paperback 2025-02-27, Kindle 2025-02-28), Amazon URLs.

## Deploying to GitHub Pages (not done; nothing has been deployed)

1. Sign in to the GitHub account created for David Dell, then create a public repository named exactly `daviddellbooks.github.io` (if that account's username is `daviddellbooks`).
2. In the new repository, choose **Add file → Upload files**.
3. Drag in the **contents** of this folder (`index.html`, `style.css`, `robots.txt`, `README.md` and the `assets/` and `guide/` folders), not the folder itself, so `index.html` sits at the repository root. Don't upload the hidden `.git` folder.
4. Commit to `main`.
5. In **Settings → Pages**, set the source to **Deploy from a branch**, branch `main`, folder `/ (root)`, if it isn't already.
6. After a minute or two the site will be live at https://daviddellbooks.github.io/. Check the page, the guide and the PDF, then test a link preview.

If the account username differs, update the absolute URLs in `index.html` and `guide/watchers-in-scripture.html`.

## Credits

- Scripture: King James Version (public domain).
- Artwork: original, generated with code (Python/Pillow).
- Font: Cinzel, © The Cinzel Project Authors, SIL OFL 1.1.
