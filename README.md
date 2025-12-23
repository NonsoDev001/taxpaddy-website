# TaxPaddy Website

Complete TaxPaddy website with landing page, privacy policy, terms of service, and support pages.

## Structure

```
taxpaddy-website/
├── index.html                    # Landing page
├── vercel.json                   # Vercel configuration for clean URLs
├── images/                       # All images
│   ├── TAX PADDY 3.png          # Logo
│   ├── 927shots_so.png          # Hero image
│   └── image.png                # Additional image
├── privacy-policy/
│   └── index.html               # Privacy Policy page
├── terms-of-service/
│   └── index.html               # Terms of Service page
├── support/
│   └── index.html               # Support page
├── email-verified/
│   └── index.html               # Email verification success page (for app)
└── reset-password/
    └── index.html               # Password reset page (for app)
```

## URLs After Deployment

- `https://taxpaddy.com` - Landing page
- `https://taxpaddy.com/privacy-policy` - Privacy Policy
- `https://taxpaddy.com/terms-of-service` - Terms of Service
- `https://taxpaddy.com/support` - Support page
- `https://taxpaddy.com/email-verified` - Email verification success (for app authentication)
- `https://taxpaddy.com/reset-password` - Password reset (for app authentication)

## Deployment Instructions

### 1. Create GitHub Repository

1. Go to https://github.com/new
2. Repository name: `taxpaddy-website`
3. Description: "TaxPaddy official website"
4. Public repository
5. Click "Create repository"

### 2. Upload Files to GitHub

**Option A - Via GitHub Web Interface:**
1. In your new repository, click "uploading an existing file"
2. Drag and drop ALL files and folders from this directory
3. Commit changes

**Option B - Via Git Command Line:**
```bash
cd taxpaddy-website
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/YOUR-USERNAME/taxpaddy-website.git
git push -u origin main
```

### 3. Deploy to Vercel

1. Go to https://vercel.com/new
2. Click "Continue with GitHub"
3. Find "taxpaddy-website" repository
4. Click "Import"
5. Framework Preset: Select "Other"
6. Click "Deploy"
7. Wait 30-60 seconds

### 4. Configure Custom Domain

1. After deployment, go to Settings → Domains
2. Click "Add"
3. Enter: `taxpaddy.com`
4. Vercel will show DNS records (write them down!)

### 5. Update DNS in GoDaddy

1. Log into GoDaddy
2. Go to Domain Settings → DNS Management
3. **Update the A record:**
   - Type: A
   - Name: @
   - Data: Change from `75.2.60.5` to `216.198.79.1` (Vercel's IP)
   - TTL: 1 Hour
4. **Delete the CNAME record for "legal" subdomain** (if it exists)
5. Save changes

### 6. Wait for DNS Propagation

- Timeline: 10-30 minutes
- Check status at: https://dnschecker.org

### 7. Test Your URLs

After DNS propagates, test:
- https://taxpaddy.com
- https://taxpaddy.com/privacy-policy
- https://taxpaddy.com/terms-of-service
- https://taxpaddy.com/support

## App Store URLs

Use these URLs for app store submissions:

**Google Play Console:**
- Privacy Policy: `https://taxpaddy.com/privacy-policy`
- Support URL: `https://taxpaddy.com/support`

**Apple App Store Connect:**
- Privacy Policy: `https://taxpaddy.com/privacy-policy`
- Terms of Service: `https://taxpaddy.com/terms-of-service`
- Support URL: `https://taxpaddy.com/support`
- Marketing URL: `https://taxpaddy.com`

## Features

✅ Clean URLs (no .html extensions)
✅ Professional landing page
✅ Complete legal pages (Privacy Policy, Terms)
✅ Comprehensive support page with FAQ
✅ Mobile responsive design
✅ Fast loading with Vercel CDN
✅ Free SSL certificate (HTTPS)
✅ TaxPaddy brand colors (#10B981)

## Tech Stack

- Static HTML/CSS/JavaScript
- No build process required
- Vercel hosting (free tier)
- GitHub for version control

## Maintenance

To update content:
1. Edit files in GitHub
2. Commit changes
3. Vercel automatically redeploys (takes 30 seconds)

---

© 2025 TaxPaddy Inc. All Rights Reserved.
