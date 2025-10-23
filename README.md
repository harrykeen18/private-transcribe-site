# Private Transcribe Marketing Site

Simple, single-page marketing website for Private Transcribe.

## Deployment Options

### Option 1: GitHub Pages (Recommended - Simplest)

1. Create a new GitHub repository (or use existing one)
2. Push this folder to the repository
3. Go to repository Settings → Pages
4. Under "Source", select "Deploy from a branch"
5. Select branch: `main` and folder: `/ (root)`
6. Click Save
7. Your site will be live at `https://yourusername.github.io/repo-name/`

### Option 2: Firebase Hosting

1. Install Firebase CLI: `npm install -g firebase-tools`
2. Login: `firebase login`
3. Initialize: `firebase init hosting`
   - Select your project or create new one
   - Set public directory to `.` (current directory)
   - Configure as single-page app: No
   - Don't overwrite index.html
4. Deploy: `firebase deploy --only hosting`

## Configuration Required

Before going live, update these placeholders in `index.html`:

1. **Download link** (line 173):
   - Replace `YOUR_USERNAME` with your GitHub username
   - Update the DMG filename if different
   - Or use a direct link to your latest release

2. **Buy Me a Coffee link** (line 176):
   - Replace `YOUR_USERNAME` with your Buy Me a Coffee username
   - Create account at https://buymeacoffee.com if needed

3. **Plausible Analytics** (line 160):
   - Replace `yourdomain.com` with your actual domain
   - Or sign up at https://plausible.io to get your domain
   - Free tier available for small sites

## Optional: Custom Domain

### For GitHub Pages:
1. Add a `CNAME` file with your domain name
2. Configure DNS with your domain provider:
   - Add CNAME record pointing to `yourusername.github.io`
3. Enable "Enforce HTTPS" in GitHub Pages settings

### For Firebase:
1. Run: `firebase hosting:channel:deploy live --only hosting`
2. Add custom domain in Firebase Console → Hosting

## File Structure

```
.
├── index.html          # Main (and only) page
└── README.md          # This file
```

## Testing Locally

Simply open `index.html` in a browser. No build process required!

## Analytics

The site includes Plausible Analytics (privacy-friendly, no cookies):
- Lightweight script (~1KB)
- GDPR compliant
- No personal data collected
- Real-time dashboard at plausible.io

If you prefer no analytics at all, remove line 160 from `index.html`.
