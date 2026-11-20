# How to edit this site (no coding tools needed)

Open `index.html` in any text editor. Everything is plain HTML, so there is no database or login to maintain.

## 1. Before you publish: 3 things to replace

| What | Where | Find this text |
|---|---|---|
| Your WhatsApp number | top of `index.html`, "EDIT ME: site settings" | `234XXXXXXXXXX` (digits only, country code first, no +). It is never shown on the page; visitors only see the WhatsApp logo. |
| Your website address | `index.html`, `robots.txt`, `sitemap.xml` | `https://www.YOURDOMAIN.com` (use Find and Replace All) |
| Form activation | first form submission | The form sends to info.anthonyjulius@yahoo.com through FormSubmit. Send one test message, then open the activation email FormSubmit sends to that inbox and click the confirm link. Check spam too. |

## 2. Add a cover
Find the comment `TO ADD A COVER` in `index.html`, copy one `<li class="c">...</li>` line, and change `src`, `alt`, `width` and `height`. Put the image in `assets/`. The cover appears in the portfolio row and in the hero automatically.

## 3. Add an A+ Content example
Find `PORTFOLIO: A+ CONTENT`, copy one `<figure>...</figure>` block, and change the image, alt text and caption.

## 4. Add a formatting example
Find `PORTFOLIO: FORMATTING`, copy one `<li style="--r:...">` line. Set `--r` to the image width divided by height (1000x667 = 1.5, 357x537 = .665).

## 5. Change the trailer
Replace `assets/book-trailer-shadowed-forest.mp4` and `assets/book-trailer-poster.jpg` with your new files (keep MP4/H.264, ideally under 8 MB), then update the caption text and the `VideoObject` block near the top of `index.html`.

## 6. Image tips for SEO and speed
- Always write a descriptive `alt` (what the image shows, not "image1").
- Keep `width` and `height` equal to the real pixel size of the file.
- Save JPGs at about 80 to 85 percent quality.
- Use file names with words (`cover-ancient-strife.jpg`), not `IMG_2041.jpg`.

## 7. After going live
1. Submit `https://www.YOURDOMAIN.com/sitemap.xml` in Google Search Console.
2. Test the page at https://search.google.com/test/rich-results to confirm the FAQ and video markup.
3. Send a test form message and confirm it reaches the inbox.
