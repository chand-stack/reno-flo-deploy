# 🚀 Vercel Deployment Guide for Reno-Flo Landing Page

## Prerequisites
- [Vercel account](https://vercel.com/signup) (free tier available)
- [GitHub account](https://github.com/) (to connect your repository)

## Step-by-Step Vercel Deployment

### 1. Push Updated Code to GitHub
```bash
git add .
git commit -m "Add Vercel deployment configuration"
git push
```

### 2. Deploy on Vercel

#### Option A: Deploy from GitHub (Recommended)
1. Go to [Vercel Dashboard](https://vercel.com/dashboard)
2. Click **"New Project"**
3. Select **"Import Git Repository"**
4. Choose your `reno-flo-landing` repository
5. Vercel will automatically detect it's a Node.js app
6. Click **"Deploy"**

#### Option B: Deploy from Local Directory
1. Install Vercel CLI: `npm i -g vercel`
2. Run: `vercel` in your project directory
3. Follow the prompts to deploy

### 3. Automatic Configuration
Vercel will automatically:
- Detect your Node.js app from `vercel.json`
- Install dependencies (`npm install`)
- Deploy your serverless function
- Provide a live URL

### 4. Get Your Live URL
- Vercel provides: `https://your-app-name.vercel.app`
- Your landing page will be live at this URL
- Custom domains available in Vercel dashboard

## File Structure for Vercel
```
├── server.js              # Express server (Vercel function)
├── package.json           # Dependencies & scripts
├── vercel.json           # Vercel configuration
├── reno-flo-landing.html # Your landing page
├── .gitignore            # Excludes unnecessary files
└── README.md             # This file
```

## Vercel vs Railway Comparison

| Feature | Vercel | Railway |
|---------|--------|---------|
| **Deployment Speed** | ⚡ Very Fast | 🚀 Fast |
| **Free Tier** | ✅ Generous | ✅ Available |
| **Node.js Support** | ✅ Excellent | ✅ Excellent |
| **Custom Domains** | ✅ Free | ✅ Available |
| **Serverless** | ✅ Yes | ❌ No |
| **Ease of Use** | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ |

## Testing Locally
```bash
npm install
npm start
# Open http://localhost:3001
```

## Customization
- Edit `reno-flo-landing.html` to change content
- Modify `vercel.json` for custom routing
- Update `package.json` to add more dependencies

## Environment Variables (if needed)
- Add in Vercel Dashboard → Project Settings → Environment Variables
- No `.env` files needed in production

## Automatic Deployments
- Every push to GitHub automatically redeploys
- Preview deployments for pull requests
- Easy rollback to previous versions

## Troubleshooting
- Check Vercel build logs if deployment fails
- Ensure all files are committed to GitHub
- Verify Node.js version compatibility (>=18.0.0)
- Check Vercel function logs for runtime errors

## Next Steps After Deployment
1. Test your live site
2. Set up custom domain (optional)
3. Configure environment variables (if needed)
4. Set up monitoring and analytics
