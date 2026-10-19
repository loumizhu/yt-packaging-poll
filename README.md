# YouTube Title Polling System (Discord Webhook)

A clean, authentic YouTube-styled page designed to split-test video titles with people you know before publishing.

---

## 🚀 How to Set Up (1 Minute)

### 1. Get Your Discord Webhook URL
1. Open Discord on your desktop or mobile.
2. In your private server, right-click any channel (or click channel settings ⚙️).
3. Go to **Integrations** > **Webhooks** > **New Webhook**.
4. Name it `YouTube Title Poll` and click **Copy Webhook URL**.

### 2. Paste It Into [`index.html`](file:///e:/%28%28_atWork_%29%29/Ytube_Channel/tools/title_tester_poll/index.html)
Open [`index.html`](file:///e:/%28%28_atWork_%29%29/Ytube_Channel/tools/title_tester_poll/index.html) and paste your webhook on line 351:

```javascript
const DISCORD_WEBHOOK_URL = "https://discord.com/api/webhooks/YOUR/ACTUAL/WEBHOOK/URL";
```

That is all. Whenever anyone clicks a thumbnail, Discord will immediately send you a notification with:
- The exact title they chose
- The decision speed (how many seconds they took to click)
- Their name (if included in the URL)

---

## 🌐 Deploy to GitHub Pages (Unlisted / Private)

1. Create a repository on GitHub (give it an unlisted name like `packaging-study-81`).
2. Upload [`index.html`](file:///e:/%28%28_atWork_%29%29/Ytube_Channel/tools/title_tester_poll/index.html) to the repository.
3. In GitHub repo **Settings** > **Pages**:
   - Source: **Deploy from a branch**
   - Branch: **main** / **root**
   - Click **Save**.
4. Your polling link will be:
   ```text
   https://<your-username>.github.io/<repo-name>/
   ```

---

## 🔗 How to Track Who Voted

You can personalize the link for friends or contacts by adding `?voter=Name`:
```text
https://<your-username>.github.io/<repo-name>/?voter=Mike
https://<your-username>.github.io/<repo-name>/?voter=Sarah
```
When they vote, the Discord ping will show `Voter: Mike` or `Voter: Sarah`.
