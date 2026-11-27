# Qamees.qa — Coming Soon

A bilingual (English / عربي) coming-soon page for Qamees.qa, styled in Qatar maroon and ivory. It's ready for GitHub Pages and needs no build step.

## 1. Add your details
Open `index.html` and edit the `CONFIG` block near the bottom:

| Field | What to put |
|---|---|
| `instagram` | Instagram username, without the @ |
| `whatsapp` | Digits only, with country code, e.g. `97455512345` |
| `phone` | Customer-service number as you want it displayed |
| `email` | Customer-service email |
| `companyName`, `crNumber`, `licenseNumber` | **Required by your MOCI eCommerce licence.** These appear in the footer and in the policies |
| `returnDays`, `refundDays`, `ackDays`, `resolveDays`, `hours` | Your return and complaint commitments |

## 2. Publish on GitHub Pages
1. Create a new public repository on github.com, e.g. `qamees-site`.
2. Click **Add file → Upload files** and drag in everything from this folder, keeping the `assets` folder intact. Then commit.
3. Go to **Settings → Pages**. Under *Build and deployment*, set Source to **Deploy from a branch**, Branch to **main** and the folder to **/ (root)**, then click **Save**.
4. After about a minute the site is live at `https://<your-username>.github.io/qamees-website/`.

## 3. Connect the qamees.qa domain
1. In **Settings → Pages → Custom domain**, enter `qamees.qa` and click **Save**. This creates a `CNAME` file in the repo.
2. With your .qa domain registrar, add these DNS records:
   - `A` records for `@` pointing to `185.199.108.153`, `185.199.109.153`, `185.199.110.153` and `185.199.111.153`
   - a `CNAME` record for `www` pointing to `<your-username>.github.io`
3. Once the DNS check passes, tick **Enforce HTTPS**.

## Licence-compliance checklist (MOCI eCommerce licence obligations)
- [x] Commercial-licence number shown on the website (footer)
- [x] Customer-service phone number and email (contact buttons, Customer Care page)
- [x] Returns and replacement policy (Returns & Exchange)
- [x] Consumer-protection measures and complaint procedure (Customer Care & Complaints)
- [x] Website terms of use (Terms of Use), plus a Privacy policy
- [ ] Licensed e-payment provider: applies when the store launches
- [ ] Product information: applies when products are listed

You can link straight to any policy: `qamees.qa/#terms`, `#returns`, `#care`, `#privacy`.

The policy texts are a good-faith starting draft. Have them reviewed by a Qatar-qualified legal adviser before launch.
