# FeatWave

**One chat bot for Kick and Twitch.** See both chats in one place, show alerts and chat on stream, run points and a leaderboard, giveaways with a spinning wheel and polls, block spam bots, take song requests, read messages aloud, control it all from a Stream Deck - from one app on your PC.

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

FeatWave opens with a short **setup guide** (you can open it again any time from **Settings > Setup guide**), on the **Connections** page.

1. **Get your app keys.** Click **"How to get my Kick keys"** and follow the steps, then do the same for Twitch. Each guide has an "Open developer page" button and a Copy button for the address you need to paste.
2. **Paste your keys** into the boxes and click **Save keys**.
3. Click **Log in with Kick** and **Log in with Twitch** and approve in your browser. FeatWave connects straight away.
4. Head to the **Dashboard** - your chat from both platforms shows up there.

Your keys and logins are saved **only on your PC**. FeatWave never sends them anywhere except to Kick and Twitch.

---

## ✨ What FeatWave can do

| Feature | Kick | Twitch |
|---|:---:|:---:|
| Combined chat with platform badges | ✅ | ✅ |
| Emotes as pictures, animated ones move (incl. 7TV, BTTV, FFZ) | ✅ | ✅ |
| Name colors + badge pictures (hover for details) | ✅ | ✅ |
| Your name highlighted when mentioned · chat pauses under your mouse | ✅ | ✅ |
| Send messages to one or both chats | ✅ | ✅ |
| Commands - with or without `!`, sounds + replies, cooldowns, once per stream | ✅ | ✅ |
| **Personal commands** - a viewer's own sound, by command and/or on their first chat | ✅ | ✅ |
| **Make, edit, pause and delete channel point rewards** from FeatWave | ✅ | ✅ |
| Channel point rewards → sounds, messages, song requests, text to speech | ✅ | ✅ |
| **Song requests** (`!sr` or channel points) on Spotify (Premium) or YouTube (free, with a backup playlist), plus a Now Playing box for OBS | ✅ | ✅ |
| **Text to speech** channel point rewards - natural voices, length and voice per reward, blocked words, skip button | ✅ | ✅ |
| First-time chatter sound for everyone else | ✅ | ✅ |
| Timers (automatic messages, only while live) | ✅ | ✅ |
| Events feed - follows, subs, gifts, raids/hosts, bits, Kicks, redemptions | ✅ ** | ✅ |
| **Stream info** - change your title and category on both at once (or different on each) | ✅ | ✅ |
| **Alerts** - sound, GIF/picture/video + text on stream, thank-you in chat | ✅ | ✅ |
| **Viewer list** - grouped by streamer, mods, VIPs, subs, viewers | ✅ * | ✅ |
| Moderation - click a name to delete / timeout / ban | ✅ | ✅ |
| **Chat on stream** - both chats together in one OBS box | ✅ | ✅ |
| **Points + leaderboard** - earn for watching/chatting/events, `!points`, `!leaderboard`, `!watchtime`, `!link` accounts, commands that cost points, OBS leaderboard, import from StreamElements | ✅ * | ✅ |
| **Giveaways** - `!join`, subs-only option, timer, redraw, spinning wheel on stream | ✅ | ✅ |
| **Polls** - viewers type the number, live results in OBS | ✅ | ✅ |
| **Moderation filters** - banned words/phrases (sees through tricks), bot-spam list, link blocking with `!permit`, undo | ✅ | ✅ |
| **Shoutouts** (`!so @name`), **counters** (`!death`), **quotes** (`!quote`) | ✅ | ✅ |
| **Hotkeys & Stream Deck** - skip songs/TTS, giveaways, polls, your commands... | ✅ | ✅ |
| **Stream summary** + end-of-stream **credits roll** for OBS | ✅ | ✅ |
| **Discord going-live posts** (and stream summary) | ✅ | ✅ |
| Text size (Settings, or Ctrl + / Ctrl -) | ✅ | ✅ |
| Backup & restore your whole setup | ✅ | ✅ |

\* Kick only shares a viewer count, so the Kick viewer list shows people who have chatted, and on Kick "watching" points go to people who chatted in the last 15 minutes.

\*\* Kick doesn't send follows to desktop apps yet, so FeatWave shows new Kick followers as "Someone followed!" - or instantly with names if you connect StreamElements (Connections page).

---

## 🔔 Showing alerts on stream (OBS)

1. Set up your alerts on FeatWave's **Alerts** page (each platform has its own).
2. In OBS, add a **Browser Source**:
   - **URL:** `http://localhost:8790/alerts` (the Alerts page has a Copy button)
   - **Width:** 1920 · **Height:** 1080 (or your canvas size)
3. Click **Test** on any alert in FeatWave to see it in OBS.

FeatWave has to be open for alerts to show.

**More things for OBS** (each one is another Browser Source - the address and a Copy button are on its page):

| What | Address | Where in FeatWave |
|---|---|---|
| Both chats on stream | `http://localhost:8790/chat` | Alerts |
| Giveaway / wheel of names | `http://localhost:8790/wheel` | Giveaways & Polls |
| Poll | `http://localhost:8790/poll` | Giveaways & Polls |
| Points leaderboard | `http://localhost:8790/leaderboard` | Points |
| Credits roll | `http://localhost:8790/credits` | Stream Summary |
| Now playing | `http://localhost:8790/nowplaying` | Song Requests |

---

## 🎛 Stream Deck (no hotkeys needed)

On FeatWave's **Hotkeys & Stream Deck** page, click **Copy link** next to any control. In the Stream Deck app, drag **System > Website** onto a button, paste the link into **URL**, and tick **GET request in background**. Touch Portal, Loupedeck and anything that can open a link work the same way. No Stream Deck? Set a keyboard hotkey on the same page - they work even while you're in a game.

---

## ⚠️ Known limits (no need to report these)

- Kick chat uses the same live feed as Kick's own website. If Kick changes it, Kick chat may stop until a FeatWave update.
- Twitch only lets the app that made a reward edit it. FeatWave can play sounds and messages for rewards made on the website or by other apps (like Mix It Up), but to edit one in FeatWave, delete it there and make it again with **+ New Reward**.
- Spotify song requests need Spotify Premium (Spotify's rule). YouTube song requests are free; typing song names (instead of links) needs a free YouTube API key.
- First-chat sounds play on a viewer's first message - Kick doesn't tell apps when someone just opens your stream.
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
- **Updating:** from v1.0.7 on, click the green **Update** button in FeatWave's sidebar - it installs the new version and reopens by itself. (Or replace `FeatWave.exe` with the new one yourself.) Your settings stay.
- **New PC?** Settings → **Save a backup**, then on the new PC: Settings → **Restore from a backup**, and log in again.
- **Uninstall:** delete `FeatWave.exe`, and the folder above if you want your settings gone too.
