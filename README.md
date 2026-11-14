# REVA University B.Tech in Design Engineering | Outreach landing page

A single mobile-friendly page with the programme brochure first, the TV9 Kannada Education Expo interview second, and the official REVA University video third. The videos open on YouTube. The original PDF is included without modification (about 22 MB) and is only loaded when a visitor opens or downloads it.

## Publish on GitHub Pages

1. Create a GitHub repository. A school- or university-controlled account is preferable if this will become the permanent outreach link.
2. Extract the ZIP. Commit the contents of the extracted site folder to the root of the `main` branch, including `.nojekyll` and the `assets` folder. `index.html` should be at the repository root, not in a nested folder. No dependencies or build commands are needed.
3. In the repository, go to **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**, then choose **main** and **/(root)**. Save.
4. Wait for Pages to show the published URL. Open it on a phone and a desktop and test the brochure and both video links before using the address for outreach.

Official instructions: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## Update content without changing the page URL

- **Brochure:** Replace `assets/btech-design-engineering-brochure.pdf` with the revised PDF using the same filename. If the cover or hero artwork changes, replace `assets/brochure-cover.webp` and `assets/brochure-artwork.webp` as well. Update the image alternatives in `index.html` if needed.
- **Videos:** Each video card in `index.html` contains two copies of its YouTube link, one for the thumbnail and one for the text link. Update both together. Replace the corresponding thumbnail in `assets/` and update the title, source label, accessible labels and description as applicable.
- **Website links:** Update the school and programme links in `index.html` if REVA changes those URLs.
- **Permanent address:** Keep the published page address stable after it is printed or encoded in a QR code. A school-controlled custom domain can make it easier to change hosting later. There is no QR code in this release.

For a local preview, open `index.html` directly or run `python3 -m http.server 8000` from the site folder and visit `http://localhost:8000`.

Artwork and REVA mark are from the supplied programme brochure. Video thumbnails are from the two linked YouTube videos. Verify any institutional branding and hosting requirements before public launch.
