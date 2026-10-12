# Juba Moslem Care Foundation website

A static website: no server, database or build step needed. It runs on any static web host.

## Contents
- `index.html`: the whole site (all pages, styles and code)
- `assets/`: logo, photos, videos, favicon and social share image
- `robots.txt`: lets search engines index the site

## Put it online (about 10 minutes, free)
1. Go to https://app.netlify.com/drop and drag the `jmcf-website` folder onto the page.
2. Sign up to keep the site. It gets an address like `jmcf.netlify.app`.
3. Optional: connect your own domain (for example `jubamoslemcare.org`) in Netlify's domain settings.

Cloudflare Pages and GitHub Pages work the same way.

## Edit content
Open `index.html` and find the `SITE` block near the top of the main script.
Every name, contact detail, impact figure, story and link is set there.
Anything left as `null` shows on the site as a labelled placeholder.

## Make the contact form send messages
1. Create a free form at https://formspree.io using the foundation's email.
2. Copy the form's endpoint (looks like `https://formspree.io/f/abcd1234`).
3. Paste it into `contactFormEndpoint` in the `SITE` block, then redeploy.

## Turn on online donations
Never add card fields to this site. Use a provider's hosted checkout page and paste its link into `donation.checkoutUrl`.
Check eligibility first: several major processors do not onboard organisations registered in South Sudan. Options to discuss:
- Muslim giving platforms that handle Zakat and Sadaqah campaigns, such as LaunchGood
- A registered fiscal sponsor or partner charity abroad that receives funds on the foundation's behalf
- Mobile money for local and regional donors (publish the official merchant number on the Donate page)

## After going live
- Uncomment the `og:image` line in `index.html` and set your real domain, so links shared on WhatsApp and Facebook show a photo.
- Test the contact form and the videos on a phone.
