# Fortune Serv website

Static site for Fortune Serv (Fortune Movers + Fortune Recovery). No build step: plain HTML/CSS, hosted on GitHub Pages.

## Pages
- `index.html` – landing page (Movers / Recovery)
- `movers.html` – choose Home / Student / Commercial moves
- `home-moves.html`, `student-moves.html`, `commercial-moves.html` – services + "Get a quote"
- `recovery.html` – "Broken down? Call now"
- `contact.html` – phone number + enquiry form

## Making the enquiry form send emails
GitHub Pages can't process forms itself, so the form uses Formspree (free tier):
1. Sign up at https://formspree.io and create a new form using the email you want enquiries sent to.
2. Copy the form ID (the part after `/f/`, e.g. `xyzabcd`).
3. In `contact.html`, replace `YOUR_FORM_ID` with it, then commit and push.

## Adding service photos
Put the photo in `images/`, then in the service page replace
`<div class="service-img">Photo coming soon</div>` with
`<img class="service-img" src="images/your-photo.jpg" alt="Describe the photo">`.
