# Share Hub for "Himar al-Shu'ara" (حمار الشعراء)

A standalone, modern, glassmorphic social sharing dashboard designed to help users share the **"Himar al-Shu'ara"** poem site with prefilled multi-line formatting across multiple messaging and social media platforms.

Website URL: https://benjelloun.dev/hmittou

---

## Features

1. **Multi-Platform Support**:
   * **WhatsApp**: Prefilled Arabic text and URL, with WhatsApp-only markdown bold for the title.
   * **Telegram**: Prefilled clean Arabic text plus a separate URL parameter, without markdown stars.
   * **X (Twitter)**: Clean Arabic text plus a separate URL parameter, without markdown stars.
   * **LinkedIn / Facebook**: URL sharing with title/summary or quote where supported, plus automatic clean-text copy before opening as a reliable fallback.
   * **Clipboard Copy**: One-click clean text copying with no markdown stars.
   * **Web Share API**: Native mobile sharing for iOS and Android using clean text plus URL.

2. **Aesthetics & UX**:
   * Beautiful modern glassmorphism UI.
   * Native Dark / Light mode switcher with local memory persistence.
   * Live chat bubble preview simulator displaying exactly what is being shared.
   * Platform-aware notes explaining markdown, clean text, and copy fallback behavior.
   * Fluid hover scales and transition animations.

3. **Analytics Integration**:
   * Optional **UTM Tracking Builders** to toggle campaigns and attribute visits (e.g. `?utm_source=twitter`).

---

## Local Development & Testing

You can open `index.html` directly in any web browser, or host it locally using a simple HTTP server:

```bash
# Python 3
python3 -m http.server 8000

# Node.js
npx serve
```

---

## Automatic Deployment with GitHub Actions (GitHub Pages)

To host this repository on GitHub Pages using modern, secure GitHub Actions (no credentials needed), we have configured a deployment workflow in `.github/workflows/deploy.yml`.

### How to set it up:
1. Create a new repository on GitHub (e.g. `share-hub`).
2. Go to your Repository **Settings** -> **Pages**.
3. Under **Build and deployment** -> **Source**, select **GitHub Actions** (instead of Deploy from a branch).
4. Push this repository to GitHub:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
   git branch -M main
   git push -u origin main
   ```
5. The GitHub Action will trigger automatically and host your site within a minute!
