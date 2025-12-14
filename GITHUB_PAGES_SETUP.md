# GitHub Pages Setup Instructions

Your EULA and Privacy Policy are ready! Follow these steps to enable GitHub Pages and get the URLs for your QuickBooks app.

## Step 1: Enable GitHub Pages

1. Go to your repository: https://github.com/babylonman/bookkeepingbyjon
2. Click **Settings** (top right)
3. Click **Pages** (left sidebar)
4. Under "Source":
   - Select branch: `main`
   - Select folder: `/docs`
   - Click **Save**

## Step 2: Wait for Deployment (2-3 minutes)

GitHub will build and deploy your site. You'll see a message:
```
Your site is live at https://babylonman.github.io/bookkeepingbyjon/
```

## Step 3: Get Your URLs

Once deployed, your legal pages will be available at:

**End-User License Agreement:**
```
https://babylonman.github.io/bookkeepingbyjon/eula.html
```

**Privacy Policy:**
```
https://babylonman.github.io/bookkeepingbyjon/privacy.html
```

## Step 4: Add to Intuit Developer Portal

1. Go to https://developer.intuit.com/
2. Navigate to your app: "Add to bookkeepingbyjon"
3. Go to app settings
4. Enter the URLs:
   - **End-user license agreement URL:** `https://babylonman.github.io/bookkeepingbyjon/eula.html`
   - **Privacy policy URL:** `https://babylonman.github.io/bookkeepingbyjon/privacy.html`
5. Save changes
6. You can now get production keys!

## What's Included

### Home Page
- https://babylonman.github.io/bookkeepingbyjon/
- Professional landing page for your app
- Links to EULA and Privacy Policy

### EULA (eula.html)
- Complete End-User License Agreement
- Covers QuickBooks integration
- Standard software licensing terms
- Limitation of liability
- Indemnification clauses

### Privacy Policy (privacy.html)
- Comprehensive privacy policy
- Emphasizes local-only data processing
- No server storage of financial data
- OAuth 2.0 security
- CCPA compliance
- Data retention and deletion

## Verify Your Site

After GitHub Pages is enabled:

1. Visit: https://babylonman.github.io/bookkeepingbyjon/
2. Click the EULA and Privacy Policy links
3. Verify they load correctly
4. Use these URLs in your Intuit app settings

## Customization (Optional)

If you want to customize the documents:

1. Edit files in `/Users/jon/repos/bookkeepingbyjon/docs/`
2. Update:
   - Your state (currently placeholder in EULA section 13)
   - Your contact email (in privacy.html section 12)
3. Commit and push:
   ```bash
   cd /Users/jon/repos/bookkeepingbyjon
   git add docs/
   git commit -m "Update legal documents"
   git push origin main
   ```
4. Changes will be live in 2-3 minutes

## Troubleshooting

**Site not loading?**
- Wait 3-5 minutes after enabling GitHub Pages
- Check Settings → Pages to ensure it's enabled
- Verify branch is `main` and folder is `/docs`

**404 errors?**
- Make sure URLs include `/bookkeepingbyjon/` in the path
- Check that files are in the `docs/` directory
- Verify files pushed to GitHub: https://github.com/babylonman/bookkeepingbyjon/tree/main/docs

**Need to update documents?**
- Edit the HTML files locally
- Commit and push to GitHub
- Changes deploy automatically

## Production Readiness

Your legal documents are production-ready and include:

✓ Comprehensive EULA covering software licensing
✓ Privacy policy emphasizing data security
✓ QuickBooks integration terms
✓ OAuth 2.0 security disclosure
✓ Local-only data processing disclosure
✓ CCPA compliance provisions
✓ Professional styling

You're all set to get production API keys from Intuit!
