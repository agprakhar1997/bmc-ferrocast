# BMC Ferrocast · Filter Detection System

Industrial vision app powered by Roboflow — detects filter availability on the production line.

## Project Structure

```
bmc-ferrocast/
├── api/
│   └── detect.js       ← Vercel serverless function (Roboflow proxy)
├── public/
│   └── index.html      ← Frontend UI
├── vercel.json         ← Vercel routing config
└── package.json
```

## Deploy to Vercel

### 1. Push to GitHub

```bash
git init
git add .
git commit -m "Initial commit — BMC Ferrocast Filter Detection"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/bmc-ferrocast.git
git push -u origin main
```

### 2. Import on Vercel

1. Go to [vercel.com](https://vercel.com) → **Add New Project**
2. Import your GitHub repo
3. Click **Deploy** (no build settings needed)

### 3. Add Environment Variable

After deploy, go to your project on Vercel:

**Settings → Environment Variables → Add**

| Name | Value |
|------|-------|
| `ROBOFLOW_API_KEY` | `W3JaMDUJgegvylcX7n4Y` |

Then **Redeploy** once from the Deployments tab.

---

Your app will be live at `https://bmc-ferrocast.vercel.app` (or similar).
