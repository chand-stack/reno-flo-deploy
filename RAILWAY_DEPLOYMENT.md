# 🚀 Railway Deployment Guide for Reno-Flo Landing Page

## Prerequisites
- [Railway account](https://railway.app/) (free tier available)
- [GitHub account](https://github.com/) (to connect your repository)

## Step-by-Step Deployment

### 1. Push to GitHub
```bash
git init
git add .
git commit -m "Initial commit: Reno-Flo landing page"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
git push -u origin main
```

### 2. Deploy on Railway
1. Go to [Railway Dashboard](https://railway.app/dashboard)
2. Click "New Project"
3. Select "Deploy from GitHub repo"
4. Choose your repository
5. Railway will automatically detect it's a Node.js app
6. Click "Deploy"

### 3. Configure Environment Variables (if needed)
- Railway will automatically set `PORT` environment variable
- No additional configuration needed for this simple app

### 4. Get Your Live URL
- Railway will provide a URL like: `https://your-app-name.railway.app`
- Your landing page will be live at this URL!

## File Structure
```
├── server.js              # Express server
├── package.json           # Dependencies
├── reno-flo-landing.html # Your landing page
├── railway.toml          # Railway config
├── .nixpacks            # Build configuration
└── README.md            # This file
```

## Testing Locally
```bash
npm install
npm start
# Open http://localhost:3000
```

## Customization
- Edit `reno-flo-landing.html` to change content
- Modify `server.js` to add more routes
- Update `package.json` to add more dependencies

## Troubleshooting
- Check Railway logs if deployment fails
- Ensure all files are committed to GitHub
- Verify Node.js version compatibility (>=18.0.0)
