# Aviation Converter – Support & Privacy Mini-Site

Minimal, App Store–ready site with:
- `index.html` → **Support page** (use as *Support URL* in App Store Connect)
- `privacy.html` → **Privacy Policy** (use as *Privacy Policy URL* in App Store Connect)
- (optional) `/assets/icon/` → app/web icons & favicons

Owner: **Occam Tech S.R.L.**  
Support contact: **office@caselib.ro** · **+40 750 257 275**

---

## 1) Folder Structure
├── index.html # Support page
├── privacy.html # Privacy policy
└── assets/
└── icon/ # (optional) favicons / web manifest


> You can safely deploy with just the two HTML files. The `assets/icon` folder is optional but recommended for favicons.

---

## 2) What to Edit

- **Company block (both pages):** already filled with Occam Tech S.R.L. data.
- **Dates (privacy.html header + footer):** update if needed.
- **Links:** when you have store links, add them in `index.html` under **Links**.

If you later add analytics, cookies, user accounts, or server APIs, update **Third-Party Services**, **Data Collection**, and **Security** sections accordingly.

---

## 3) Deploy

### GitHub Pages (no build needed)
1. Create a repo and push these files.
2. In **Settings → Pages**:
   - **Source**: `Deploy from a branch`
   - **Branch**: `main` (root)
3. Your site will be at:  
   `https://<username>.github.io/<repo>/`
4. Use:
   - **Support URL** → `https://<username>.github.io/<repo>/`
   - **Privacy Policy URL** → `https://<username>.github.io/<repo>/privacy.html`

### Netlify (drag-and-drop)
1. Zip the folder or drag it into Netlify.
2. Netlify will assign a URL like `https://<site-name>.netlify.app/`.
3. Use:
   - **Support URL** → `https://<site-name>.netlify.app/`
   - **Privacy Policy URL** → `https://<site-name>.netlify.app/privacy.html`

---

## 4) Run Locally (optional)

Any static server works. Examples:

### Python
```bash
# Python 3
python -m http.server 8080
# open http://localhost:8080
npm i -g http-server
http-server -p 8080
