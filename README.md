# Srinidhi Hospital website — redesigned static build

## What changed
- Rebuilt all public pages with a consistent, responsive visual system and a calmer green/white palette.
- Removed the cartoon/illustrated hero, decorative Unicode symbols, generic slogan copy and repeated card-grid treatment.
- Added clear contact actions, a mobile call/WhatsApp bar, keyboard-accessible navigation, visible focus states and reduced-motion support.
- Added a validated appointment enquiry form that prepares a WhatsApp message for the visitor to review and send.
- Added gallery photo slots and a lightbox, a map embed, unique page titles/descriptions, Open Graph metadata, Hospital/FAQ JSON-LD, robots.txt and sitemap.xml.
- Kept contact settings in `assets/js/config.js`.
- No stock photos, external font requests, frameworks or runtime image services are used.

## Before publishing
1. Update `assets/js/config.js` if the phone, address or opening hours need correction.
2. Confirm the deployed website URL. This build currently uses `https://srinidhi-hospital.onrender.com`; if your live URL differs, update every canonical/JSON-LD URL plus `sitemap.xml` and `robots.txt` consistently. Follow `GOOGLE_SEARCH_CONSOLE_SETUP.md` to verify ownership and submit the sitemap.
3. Add real photos using the exact filenames below. The site deliberately displays labelled slots until those photos exist. Use appropriately compressed WebP files and retain the filenames.
4. Confirm all factual details in `FACTS_TO_CONFIRM.md`; do not publish unverified doctor qualifications or policies.

## Real photos still needed
Put supplied photos in `assets/img/` with these filenames (landscape photos work best unless noted):
- `hospital-exterior.webp` — exterior/building, hero (suggested 1600×1100)
- `reception.webp` — reception or waiting area (1200×900)
- `consultation-room.webp` — consultation room (1200×900)
- `patient-room.webp` — patient room (1200×900)
- `medical-equipment.webp` — real equipment/facility (1200×900)
- `doctors-team.webp` — real doctor/team photograph (1200×900)
- `dr-krishna-kishore.webp` — doctor portrait, only with permission (800×1000)
- `general-medicine-doctor.webp` — doctor portrait, only with permission (800×1000)

If the hospital has an approved logo, supply it and replace the text/S mark wordmark treatment. Do not substitute stock photography.

## Technical notes
- Plain HTML, CSS and vanilla JavaScript.
- The map iframe needs an internet connection; all site assets and fonts are local/system-stack.
- The WhatsApp form validates required fields and opens a prefilled message. It cannot confirm or book an appointment automatically.
- A Lighthouse score of 95+ cannot be guaranteed without testing the final deployed site with real photos, hosting headers, and a confirmed domain. Run Lighthouse after photo replacement and deployment.
- The provided archive contained no real hospital photography, so image slots are used instead of invented or stock images.
\n\n## Google SEO and indexing\n- See `GOOGLE_SEARCH_CONSOLE_SETUP.md` for the Search Console verification, sitemap submission and URL inspection steps.\n- The SEO update adds canonical URLs, social preview metadata, MedicalOrganization/WebSite/WebPage structured data, robots directives and an eight-page sitemap.\n- Google indexing and rankings are controlled by Google; these files improve discovery and clarity but do not guarantee a position.\n