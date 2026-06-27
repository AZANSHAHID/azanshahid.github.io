# How to Put Your Portfolio Live on GitHub Pages
### Step-by-Step Guide for Azan Shahid Latif

---

## STEP 1 — Set Up the Folder on Your Computer

On your computer, create a folder named exactly:
```
azanshahid.github.io
```

Inside that folder, place these files exactly like this:

```
azanshahid.github.io/
├── .github/
│   └── workflows/
│       └── deploy.yml        ← (provided)
├── Images/                   ← your existing Images folder
├── .gitignore                ← (provided)
├── LICENSE                   ← (provided)
├── README.md                 ← (provided)
└── index.html                ← your existing index.html
```

⚠️  The .github folder starts with a dot — make sure it's included.
    On Windows, hidden files/folders are sometimes not visible by default.

---

## STEP 2 — Create the GitHub Repository

1. Go to https://github.com and sign in
2. Click the green "New" button (top left)
3. Set Repository name to exactly:
   ```
   azanshahid.github.io
   ```
4. Set visibility to: ✅ Public
5. Do NOT check "Add a README file" (we already have one)
6. Click "Create repository"

---

## STEP 3 — Push Your Code to GitHub

Open a terminal (Command Prompt / Git Bash on Windows, Terminal on Mac) and run these commands one by one:

```bash
# Navigate into your project folder
cd path/to/azanshahid.github.io

# Initialize git
git init

# Add all files
git add .

# First commit
git commit -m "Initial portfolio launch"

# Connect to your GitHub repo (replace AZANSHAHID with your exact username)
git remote add origin https://github.com/AZANSHAHID/azanshahid.github.io.git

# Push to main branch
git branch -M main
git push -u origin main
```

---

## STEP 4 — Enable GitHub Pages with GitHub Actions

1. Go to your repository on GitHub:
   https://github.com/AZANSHAHID/azanshahid.github.io

2. Click ⚙️ "Settings" (top tab)

3. In the left sidebar, click "Pages"

4. Under "Build and deployment" → Source:
   Change it from "Deploy from a branch" to → "GitHub Actions"

5. That's it! GitHub will now use your deploy.yml workflow.

---

## STEP 5 — Watch It Go Live

1. Go to the "Actions" tab in your repository
2. You'll see a workflow called "Deploy Portfolio to GitHub Pages" running
3. Wait about 1-2 minutes for it to complete (green ✅ means success)
4. Visit your live site at:
   👉 https://azanshahid.github.io

---

## Making Updates in the Future

Whenever you want to update your portfolio, just:

```bash
git add .
git commit -m "Update: describe what you changed"
git push
```

GitHub Actions will automatically redeploy your site within ~1 minute.

---

## Troubleshooting

| Problem | Fix |
|---|---|
| Images not showing | Make sure the Images folder is uploaded too — not just index.html |
| Actions tab shows red ✗ | Go to Settings → Pages → make sure Source is set to "GitHub Actions" |
| Site shows 404 | Wait 2-3 minutes after first deploy, it can take time to propagate |
| .github folder missing | On Windows, enable "Show hidden items" in File Explorer |
