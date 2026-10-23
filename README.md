# His Grace & Power School

Website and staff portal for **His Grace & Power School**, a Nursery, Primary & Secondary School.
Motto: *God Our Rock.*

Ilesanmi area, Olodo Garage, Ibadan. Tel: 08073950062, 07033950815.

## What is inside

```
.
├── index.html            Public school website
├── portal/index.html     Staff portal (students, attendance, grades, fees)
├── assets/logo.png       School crest
├── .github/workflows/    Automatic deploy to GitHub Pages
├── .nojekyll
└── .gitignore
```

Both pages are plain HTML, CSS and JavaScript. There is nothing to install or build.

## Run it on your computer

Open `index.html` in a browser. The staff portal is at `portal/index.html`.

## Put it online with GitHub Pages

1. Create a new repository on GitHub and upload all these files (keep the folder layout).
2. Go to **Settings, then Pages**, and set **Source** to **GitHub Actions**.
3. Push to the `main` branch. The workflow in `.github/workflows/pages.yml` publishes the site.
4. Your site will be at `https://<your-username>.github.io/<repository-name>/` and the portal at `.../portal/`.

To use your own domain, add it under **Settings, then Pages, then Custom domain**.

## Staff portal: how data is stored

The portal saves records in the **browser on the device you use**. It does not send anything to a server.

- Records on one computer do not appear on another.
- Clearing browser data deletes the records.
- Use **Download backup** on the Dashboard often, and **Restore backup** to load a backup on another device.
- The portal page is not password protected. Anyone with the link can open it, but they would see only their own browser's data (empty on a new device). Do not put real student records on a shared computer.

To share one set of records between staff, the portal needs a hosted database and logins (for example Firebase or Supabase). Ask for this when you are ready.

## Edit the content

- School name, phone numbers and address: search `index.html` for `08073950062` and `Olodo Garage`, and update `portal/index.html` the same way.
- Colours: change the variables at the top of the `<style>` block (`--blue` is the school green, `--gold` is the gold).
- Logo: replace `assets/logo.png` with a file of the same name.

## Notes

- Fonts load from Google Fonts. Without internet the pages fall back to Georgia and system fonts.
- The enquiry form on the website does not send messages yet. It shows a thank-you note asking visitors to call.
