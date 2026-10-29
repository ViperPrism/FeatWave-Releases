# FeatWave

**One chat bot for Kick and Twitch.** See both chats in one place with emotes and badges, show alerts on stream, play sounds from commands and channel points, run timed messages, see who's watching and moderate both chats - from one app on your PC.

> 🧪 **FeatWave is in early testing.** Things may break - that's what testing is for! Please report anything odd (see [Reporting problems](#-reporting-problems)).
>
> 💬 **Join the FeatWave Discord:** https://discord.gg/3GGn86kH4H - help, update news, and bug reports.

---

## ⬇️ Download

1. Go to **[Releases](../../releases)** and download the newest **`FeatWave.exe`**.
2. Save it anywhere you like (Desktop, Documents, a "Streaming" folder...).
3. Double-click it to start.

**"Windows protected your PC"?** That's normal for new apps that haven't paid for a Microsoft signature. Click **More info → Run anyway**.

The first start takes 5-10 seconds while FeatWave unpacks itself.

---

## 🚀 First-time setup (about 10 minutes)

FeatWave opens on the **Connections** page.

1. **Get your app keys.** Click **"How to get my Kick keys"** and follow the steps, then do the same for Twitch. Each guide has an "Open developer page" button and a Copy button for the address you need to paste.
2. **Paste your keys** into the boxes and click **Save keys**.
3. Click **Log in with Kick** and **Log in with Twitch**, approve in your browser, and let FeatWave restart.
4. Head to the **Dashboard** - your chat from both platforms shows up there.

Your keys and logins are saved **only on your PC**. FeatWave never sends them anywhere except to Kick and Twitch.

---

## ✨ What FeatWave can do

| Feature | Kick | Twitch |
|---|:---:|:---:|
| Combined chat with platform badges | ✅ | ✅ |
| Emotes as pictures (incl. 7TV, BTTV, FFZ) | ✅ | ✅ |
| Name colors + badge pictures (hover for details) | ✅ | ✅ |
| Your name highlighted when mentioned · chat pauses under your mouse | ✅ | ✅ |
| Send messages to one or both chats | ✅ | ✅ |
| Commands - with or without `!`, sounds + replies, cooldowns | ✅ | ✅ |
| Channel point rewards → sounds + messages | ✅ | ✅ |
| First-time chatter sounds | ✅ | ✅ |
| Timers (automatic messages, only while live) | ✅ | ✅ |
| Events feed - follows, subs, gifts, raids/hosts, bits, Kicks, redemptions | ✅ | ✅ |
| **Alerts** - sound, GIF/picture/video + text on stream, thank-you in chat | ✅ | ✅ |
| **Viewer list** - grouped by streamer, mods, VIPs, subs, viewers | ✅ * | ✅ |
| Moderation - click a name to delete / timeout / ban | ✅ | ✅ |
| Text size (Settings, or Ctrl + / Ctrl -) | ✅ | ✅ |
| Backup & restore your whole setup | ✅ | ✅ |

\* Kick only shares a viewer count, so the Kick list shows people who have chatted.

---

## 🔔 Showing alerts on stream (OBS)

1. Set up your alerts on FeatWave's **Alerts** page (each platform has its own).
2. In OBS, add a **Browser Source**:
   - **URL:** `http://localhost:8790/alerts` (the Alerts page has a Copy button)
   - **Width:** 1920 · **Height:** 1080 (or your canvas size)
3. Click **Test** on any alert in FeatWave to see it in OBS.

FeatWave has to be open for alerts to show.

---

## ⚠️ Known limits (no need to report these)

- After logging in, logging out or turning a platform on/off, FeatWave **restarts itself** to apply it.
- Kick chat uses the same live feed as Kick's own website. If Kick changes it, Kick chat may stop until a FeatWave update.
- FeatWave can trigger on Twitch rewards made by other apps (like Mix It Up), but can't edit them yet.
- Kick doesn't share its badge pictures, so FeatWave draws simple ones. You can pick your own in **Settings**.
- Updated from an older version? **Log in to Twitch once more** (Connections page) so the viewer list can see your mods and VIPs.
- Windows only for now.

---

## 🐞 Reporting problems

**Easiest:** click **🐞 Report a problem** at the bottom of FeatWave's sidebar. It fills in your version, Windows version and recent activity automatically - you just describe what happened and click **Send on GitHub**.

**No GitHub account?** Click **Copy report** in that same window and paste it in **#bug-reports** on the [FeatWave Discord](https://discord.gg/3GGn86kH4H).

**FeatWave crashed?** Open it again and use **Report a problem** - it attaches the crash details automatically.

Have an idea? Use the same button and pick **"I have an idea"**, or post it in **#ideas** on Discord.

Need help setting up? Ask in **#help** on the [Discord](https://discord.gg/3GGn86kH4H).

---

## 💾 Your settings

- Everything lives in `C:\Users\<you>\AppData\Roaming\FeatWave` - **Settings → Open my FeatWave folder** takes you there.
- **Updating:** just replace `FeatWave.exe` with the new one. Your settings stay.
- **New PC?** Settings → **Save a backup**, then on the new PC: Settings → **Restore from a backup**, and log in again.
- **Uninstall:** delete `FeatWave.exe`, and the folder above if you want your settings gone too.
