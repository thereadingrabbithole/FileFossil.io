# Deploying FileFossil.io on GitHub Pages

Here's how to deploy your static FileFossil.io website using GitHub Pages.

---

## 📦 1. Create a GitHub Repository

- Go to [GitHub](https://github.com/)
- Click `+ New Repository`
- Name it something like `filefossil-site`
- Set it to **Public**
- Click `Create Repository`

---

## 🖥️ 2. Upload the Site

Option 1 – Drag & Drop:
- On your new repo page, click `Add file > Upload files`
- Drag all contents of this folder (not the zip itself) into the uploader
- Click `Commit changes`

Option 2 – Git (if you prefer terminal):
```bash
git clone https://github.com/yourusername/filefossil-site.git
cd filefossil-site
# Copy all contents of unzipped site into this folder
git add .
git commit -m "Initial site upload"
git push origin main
```

---

## 🌐 3. Enable GitHub Pages

- Go to `Settings > Pages`
- Under **Source**, choose `Deploy from a branch`
- Select `main` branch and `/root` folder
- Click `Save`

Your site will be live shortly at:
```
https://yourusername.github.io/filefossil-site/
```

To use a custom domain like filefossil.io:
- Go to GitHub Pages > Custom domain
- Enter `filefossil.io` and click **Save**
- Update your DNS provider with an `A` record pointing to GitHub's Pages IPs
  (docs: https://docs.github.com/en/pages/configuring-a-custom-domain)

---

## ✅ Done!
Google will start crawling your site within days. You’re live. You’re fossilised.

