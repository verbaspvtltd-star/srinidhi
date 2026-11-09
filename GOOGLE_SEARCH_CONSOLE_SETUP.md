# Google Search Console and SEO setup

## Important: verify the live website URL first
This build currently uses `https://srinidhi-hospital.onrender.com` as its canonical host because that is the host already present in the supplied website files. If the actual deployed website URL is different, replace that host consistently in:
- every HTML page's `rel="canonical"` and JSON-LD URLs
- `sitemap.xml`
- `robots.txt`

Do not submit a sitemap containing a different host from the live website.

## What this update includes
- Unique page titles and descriptions retained and improved where appropriate.
- Canonical URL on each public page.
- Index/follow directives on public pages; 404 page is noindex.
- Open Graph and Twitter preview metadata.
- Consistent MedicalOrganization, WebSite and WebPage JSON-LD.
- Sitemap listing all eight public pages.
- robots.txt pointing to the sitemap.
- Added the missing `assets/img/favicon.svg` referenced by several pages.
- Existing pages, styles, scripts and supplied image assets are retained.

## Google Search Console: setup
1. Deploy this complete folder to the same hosting service used by the current website.
2. Open https://search.google.com/search-console/about and sign in with the Google account that should own the hospital website property.
3. Add a **URL prefix** property using the exact deployed URL, including `https://` (for this build: `https://srinidhi-hospital.onrender.com/`).
4. Choose the **HTML tag** verification method. Google will show a meta tag containing a unique `content` token.
5. Copy that exact meta tag into the `<head>` section of `index.html`, then deploy again. Alternatively, use another verification method offered by Google, such as DNS TXT, if you control a custom domain.
6. In Search Console, click **Verify**. Do not copy a sample token from a tutorial; the token must come from your Search Console account.
7. Open **Sitemaps** in the left menu and submit: `sitemap.xml`
8. Open **URL Inspection**, enter the homepage URL, click **Test Live URL**, then **Request Indexing** if the page is available and indexable.
9. Repeat URL Inspection for the doctors, services, about, patient-care, FAQ and contact pages.
10. After a few days, check **Pages / Indexing**, **Sitemaps**, and **Performance** for indexing problems and search queries.

## Search terms to build relevance for
Use these phrases naturally in visible page copy, headings and relevant page descriptions—not as a hidden keyword list:
- Srinidhi Neuro & General Hospital Tanuku
- neurology hospital in Tanuku
- neurologist in Tanuku
- general hospital in Tanuku
- neurology consultation in Tanuku
- Dr. P. Krishna Kishore
- Dr. M. Vinod

Only retain doctor names, qualifications, specialties, service claims, phone number, address and opening hours if the hospital has confirmed them. Do not add fabricated testimonials, awards, patient counts, medical services or doctor credentials.

## Local visibility
- Create or claim the hospital's Google Business Profile.
- Use exactly the same official hospital name, phone number and address on the website and Business Profile.
- Select the most accurate primary category and add only services actually provided.
- Add genuine exterior, reception, facility and doctor photos with permission.
- Ask real patients for honest reviews; never buy or fabricate reviews.
- Keep phone, address and hours updated everywhere.

## Important expectations
Submitting a sitemap is a discovery hint, not a guarantee of indexing or ranking. Google chooses whether and when to index pages and where they rank. Search position depends on relevance, competition, location, website quality, reputation and other signals. Results may take days or longer to change.
