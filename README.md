# ClinicalScribe — Deployment Guide

## What this is
An AI-powered ambient clinical scribe prototype. Demo mode only — do not use with real patient data.

## Files
- `index.html` — the full application
- `vercel.json` — Vercel configuration
- `README.md` — this file

## How to deploy (no coding required)

### Step 1 — Create a GitHub repository
1. Go to github.com and sign in
2. Click the **+** icon (top right) → **New repository**
3. Name it: `clinicalscribe`
4. Set to **Public**
5. Click **Create repository**

### Step 2 — Upload the files
1. On your new repository page, click **uploading an existing file**
2. Drag and drop ALL THREE files: `index.html`, `vercel.json`, `README.md`
3. Click **Commit changes**

### Step 3 — Deploy on Vercel
1. Go to vercel.com and sign in with GitHub
2. Click **Add New Project**
3. Find `clinicalscribe` in the list and click **Import**
4. Click **Deploy** (leave all settings as default)
5. Wait ~60 seconds — your app is now live at `clinicalscribe.vercel.app`

### Step 4 — Add your Anthropic API key
This is the critical step that makes the AI work.

1. In Vercel, go to your project → **Settings** → **Environment Variables**
2. Click **Add New**
3. Name: `ANTHROPIC_API_KEY`
4. Value: paste your `sk-ant-...` key
5. Click **Save**
6. Go to **Deployments** → click the three dots on your latest deployment → **Redeploy**

Your app is now fully live and working.

## Sharing your demo
Your live URL will be: `https://clinicalscribe.vercel.app`

Send this URL to anyone — they can open it in any browser with no installation.

For the demo, use the pre-loaded scenarios (hypertension, diabetes, chest pain) in the Live scribe → Type/paste tab. Do not enter real patient data.

## Important notices
- This is a prototype for demonstration purposes only
- Do not enter real patient data — GDPR and HIPAA compliance not implemented
- The Anthropic API key in Vercel is private and never exposed in the browser
- Suitable for investor and clinic demos using fictional cases only
