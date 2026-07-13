# Shahnoome website structure

## Folder structure

```
shahnoome-organized/
├── index.html
└── assets/
    ├── css/
    │   └── style.css
    ├── js/
    │   └── main.js
    ├── images/
    │   ├── shahnoome-logo.jpg
    │   ├── ferdowsi.png
    │   ├── tree-of-wisdom.png
    │   ├── giomarth.png
    │   ├── banu.png
    │   └── coming-soon.png
    └── videos/
        └── shahnoome-intro.mp4
```

## What to do on GitHub

1. Download and unzip `shahnoome-organized.zip`.
2. Open your existing GitHub repository: `shahnoome`.
3. Delete the old single-file `index.html` only after keeping a backup.
4. Upload **all contents inside** the `shahnoome-organized` folder:
   - `index.html`
   - the complete `assets` folder
   - optionally this `README.md`
5. Commit the changes to the same branch currently used for deployment, usually `main`.
6. Wait for GitHub Pages and Cloudflare to redeploy.
7. Test both URLs in a private/incognito browser window.

## Important

- Do not upload only `index.html`; the entire `assets` folder must be uploaded with the same structure.
- Keep filenames and folder names unchanged unless you also update their paths in `index.html`.
- The Persian page remains at `/`.
- For the English version later, create `en/index.html`. It can reuse shared files with paths such as `../assets/css/style.css` and `../assets/images/...`.

## Cloudflare

If your Cloudflare Worker/Pages project is connected to this GitHub repository, no separate upload is needed. A new Git commit should trigger deployment automatically. If it does not, open the project in Cloudflare and choose **Deployments → Retry deployment**.
