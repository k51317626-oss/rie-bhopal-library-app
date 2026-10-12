# RIE Bhopal Library — Mobile App (GitHub Pages)

A mobile-first, installable Progressive Web App (PWA) for quick access to RIE Bhopal Library's website, catalogue, research support and digital resources. It is built with plain HTML, CSS and JavaScript; **Android Studio is not required**.

## What is included
- Responsive design for smartphones, tablets and desktops
- Search across the visible services and resources
- Quick access cards for catalogue, institutional repository, ONOS, newspapers, e-textbooks, e-books, e-journals, open-access resources, research support and new arrivals
- Share button and an install prompt when the browser supports it
- App manifest, SVG and PNG app icons, and a service worker for caching the app shell
- Links to the known official website and e-textbook page

## Publish using GitHub Pages
1. Sign in at https://github.com/.
2. Click **+** (top-right) → **New repository**. Name it `rie-bhopal-library-app`.
3. Choose **Public** if you want the app page publicly accessible. Click **Create repository**.
4. Extract this ZIP on your computer.
5. Open the extracted `rie-library-app-v2` folder. Select its contents (`index.html`, `manifest.webmanifest`, `service-worker.js`, `README.md`, and `assets` folder). Upload the contents directly into the repository root using **Add file → Upload files**. Do not upload only the ZIP or the outer folder.
6. Click **Commit changes**.
7. In the repository, open **Settings → Pages**.
8. Under **Build and deployment**, choose **Deploy from a branch**. Select branch `main` and folder `/(root)`, then click **Save**.
9. Wait for GitHub Pages to publish. Open the URL shown on the Pages screen. It usually looks like `https://YOUR-USERNAME.github.io/rie-bhopal-library-app/`.

## Install on Android
1. Open the published HTTPS URL in Chrome.
2. Use the browser menu (⋮) → **Install app** or **Add to Home screen**.
3. Follow the on-screen prompt. Menu wording can vary by browser/version.

## Important notes
- This is an installable web app (PWA), **not an Android APK**.
- The app uses the direct service URLs supplied in the reference code, including:
- Catalogue: `http://13.126.40.108:8001/`
- Institutional repository: `http://13.126.40.108:8080/jspui/`
- ONOS: `https://www.onos.gov.in/ums/check-access`
- E-books, e-journals, newspapers, open-access resources, research support and contact pages on `https://riebhopallibrary.joomla.com/`.

The catalogue and repository URLs use HTTP rather than HTTPS, so some browsers or networks may show a security warning or block them from an HTTPS-hosted app. The destinations are preserved from the supplied reference code; confirm that they are still active before publishing. Do not add passwords or private login details to this public code.
- The app shell can be cached for repeat visits, but external library pages still need internet access.
