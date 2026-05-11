# Room Changes Display

A GitHub Pages website showing daily room changes on a school display screen, with a separate editor page for data entry.

## Files

| File | Purpose |
|------|---------|
| `index.html` | Display screen — shown on the TV/monitor |
| `editor.html` | Data entry page — used to update the display |
| `data.json` | Data file — updated automatically by the editor |

---

## One-time Setup (you do this once)

### 1. Create a GitHub repository

1. Go to [github.com](https://github.com) and sign in.
2. Click **New repository**.
3. Name it (e.g. `room-changes`).
4. Set it to **Public** (required for free GitHub Pages).
5. Click **Create repository**.

### 2. Upload the files

Upload `index.html`, `editor.html`, and `data.json` to the repository root.

### 3. Enable GitHub Pages

1. Go to your repository → **Settings** → **Pages**.
2. Under **Source**, select **Deploy from a branch**.
3. Choose **main** branch, **/ (root)** folder.
4. Click **Save**.

Your display will be live at:
`https://<your-username>.github.io/<repo-name>/`

---

## Creating an Access Token (for the editor user)

The editor user needs a GitHub Personal Access Token to publish changes.

1. Go to **GitHub → Settings → Developer settings → Fine-grained personal access tokens**.
2. Click **Generate new token**.
3. Set an expiry (e.g. 1 year).
4. Under **Repository access**, choose **Only select repositories** and pick your repo.
5. Under **Permissions → Repository permissions**, set **Contents** to **Read and Write**.
6. Click **Generate token** and copy it (you only see it once).

---

## Using the Editor

1. Open `https://<your-username>.github.io/<repo-name>/editor.html`
2. Fill in **GitHub Settings** (once only — saved in the browser):
   - GitHub username / org
   - Repository name
   - Personal Access Token
3. Click **Save Settings**.
4. Click **Load Current Data from GitHub** to pull the existing table.
5. Edit the date and rows as needed.
6. Click **Publish to Display Screen**.

The display screen refreshes automatically every 30 seconds.

---

## Display Screen Tips

- Open `index.html` full-screen in a browser (press **F11**) on the display monitor.
- The page refreshes itself every 30 seconds — no manual action needed.
- The clock in the top-right updates every second.
