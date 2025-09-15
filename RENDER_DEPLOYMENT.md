
# 🚀 Deploy to Render.com (Free Tier)

## Quick Setup Instructions

### Step 1: Create Render Service
1. Go to [Render Dashboard](https://dashboard.render.com/)
2. Click "New +" → "Web Service"
3. Select "Build and deploy from a Git repository"
4. Connect to GitHub and select this repository: https://github.com/HarshilSiyani/sheet-app-nimisa-app-9465-1757941376335
5. Use branch: **main**

### Step 2: Configure Service Settings
- **Name**: nimisa-app
- **Build Command**: `npm install && npm run build`
- **Start Command**: `npm run preview`
- **Instance Type**: Free
- **Environment**: Static Site

### Step 3: Environment Variables
Add these environment variables in Render service settings:

```
NODE_ENV=production
NEXT_PUBLIC_SHEETAPPS_API_URL=http://localhost:3000/api/v1
NEXT_PUBLIC_SHEETAPPS_API_KEY=sk_8729c8ea124345afa4447771447543e9
NEXT_PUBLIC_SHEET_ID=1TkIgTxvyrDJNvvo_jBOaWxleHFpJd_8yjjrytw__XqA
NEXT_PUBLIC_SHEET_HEADERS=["PatientName","Number","Visited","AppointedStaff"]
NEXT_PUBLIC_SHEET_DATA_TYPES=["text","number","text","text"]
NEXT_PUBLIC_APP_NAME=Nimisa App
NEXT_PUBLIC_APP_DESCRIPTION=Manage and track Nimisa data with real-time Google Sheets integration
```

### Step 4: Deploy
- Click "Create Web Service"
- Wait for build and deployment (5-10 minutes)
- Your app will be live at: `https://your-service-name.onrender.com`

## 🔄 Auto-Deploy Setup (Optional)
Render automatically redeploys when you push to the **main** branch.

## 📞 Support
- Repository: https://github.com/HarshilSiyani/sheet-app-nimisa-app-9465-1757941376335
- Generated: 9/15/2025
- SheetApps Support: [Contact Us](mailto:support@sheetapps.com)
