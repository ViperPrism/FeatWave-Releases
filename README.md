# FeatWave

**One chat bot for Twitch, Kick, YouTube and Velora.tv.** See every chat in one place, show alerts and chat on stream, run points with a store and chat games, giveaways with a spinning wheel and polls, block spam bots, take song requests and clips, read messages aloud, and control it all from a Stream Deck or your phone. One app on your PC does it all.

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

## 🚀 First-time setup (a few minutes)

FeatWave opens with a short **setup guide** on the **Connections** page. You can open it again any time from **Settings > Setup guide**.

1. **Twitch:** just click **Log in with Twitch** and approve. There are no keys to set up.
2. **Kick:** click **"How to get my Kick keys"** and follow the steps (about 5 minutes). Paste the keys under Advanced settings, click **Save keys**, then **Log in with Kick**.
3. **YouTube** (optional): click **"How to get my YouTube keys"**. You make a free Google app (about 10 minutes, no credit card), then click **Log in with YouTube**.
4. **Velora.tv** (optional): the same idea, with the Velora guide.
5. Go to the **Dashboard**. Every chat shows up there.

Only stream on one platform? That's fine, just connect that one.

Your keys and logins are saved **only on your PC**. FeatWave never sends them anywhere except to the platforms themselves.

---

## ✨ What FeatWave can do

| Feature | Twitch | Kick | YouTube | Velora |
|---|:---:|:---:|:---:|:---:|
| Combined chat with platform badges, name colors and badge pictures | ✅ | ✅ | ✅ | ✅ |
| Emotes as pictures, animated ones move (incl. 7TV, BTTV, FFZ) | ✅ | ✅ | - | - |
| Send messages to one or every chat | ✅ | ✅ | ✅ | ✅ |
| Commands with sounds + replies, cooldowns, once per stream, groups and search | ✅ | ✅ | ✅ | ✅ |
| **Personal commands**: a viewer's own sound, by command and/or on their first chat | ✅ | ✅ | ✅ | ✅ |
| **`!commands`** shows each viewer only the commands they can use | ✅ | ✅ | ✅ | ✅ |
| **Make, edit, pause and delete channel point rewards** from FeatWave | ✅ | ✅ | - | - |
| Channel point rewards → sounds, messages, song requests, text to speech | ✅ | ✅ | - | ✅ |
| **Song requests** (`!sr`) on Spotify (Premium) or YouTube (free), plus a Now Playing box for OBS | ✅ | ✅ | ✅ | ✅ |
| **Points + leaderboard**: earn for watching, chatting and events, `!points`, `!leaderboard`, `!watchtime`, `!link` accounts, OBS leaderboard, import from StreamElements | ✅ | ✅ * | ✅ * | ✅ * |
| **Points store** (`!shop`, `!redeem`) and **chat games** (`!gamble`, `!slots`, `!duel`, `!heist`) | ✅ | ✅ | ✅ | ✅ |
| **`!clip`**: `!clip 30`, `!clip 60` (5-60 seconds), link posted in chat, optional Discord post | ✅ | ✅ *** | ✅ *** | ✅ *** |
| **Alerts**: sound, GIF/picture/video and text on stream, plus a thank-you in chat | ✅ | ✅ ** | ✅ | ✅ |
| What the alerts cover | follows, subs, gifts, raids, bits, Hype Trains | follows, subs, gifts, hosts, Kicks | members, milestones, gifted memberships, Super Chats | follows, subs, gifts, raids, Volts |
| **Stream info**: change your title and category on all at once (or different on each) | ✅ | ✅ | ✅ (while live) | ✅ |
| **Viewer list**: grouped by streamer, mods, VIPs, subs and viewers | ✅ | ✅ * | - | - |
| Click a name: **viewer card**, delete / timeout / ban | ✅ | ✅ | ✅ | ✅ |
| **Moderation filters**: banned words/phrases (sees through tricks), bot-spam list, link blocking with `!permit`, undo | ✅ | ✅ | ✅ | ✅ |
| **Giveaways** (`!join`, spinning wheel on stream) and **polls** | ✅ | ✅ | ✅ | ✅ |
| Timers, shoutouts (`!so @name`), counters (`!death`), quotes (`!quote`) | ✅ | ✅ | ✅ | ✅ |
| **Chat on stream**: every chat together in one OBS box | ✅ | ✅ | ✅ | ✅ |
| **Stream summary**, end-of-stream **credits roll**, **Discord going-live posts** | ✅ | ✅ | ✅ | ✅ |

**Also:** hotkeys, Stream Deck and a **phone remote** (big buttons and a chat box on your phone); **viewer cards** with points, watch time, messages and your private notes; **import commands and timers** from StreamElements or Mix It Up; text size (Ctrl + / Ctrl -); backup and restore of your whole setup.

\* Kick, YouTube and Velora don't share who's watching, so on those "watching" points go to people who chatted in the last 15 minutes (and the Kick viewer list shows people who have chatted).

\*\* Kick doesn't send follows to desktop apps yet, so FeatWave shows new Kick followers as "Someone followed!", or instantly with names if you connect StreamElements (Connections page).

\*\*\* Only Twitch lets apps make clips, so `!clip` from Kick, YouTube or Velora chat clips your **Twitch** stream. When you multistream, that's the same moment. Twitch has to be live.

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

On FeatWave's **Hotkeys & Stream Deck** page, click **Copy link** next to any control. In the Stream Deck app, drag **System > Website** onto a button, paste the link into **URL**, and tick **GET request in background**. Touch Portal, Loupedeck and anything that can open a link work the same way. No Stream Deck? Set a keyboard hotkey on the same page. Hotkeys work even while you're in a game.

**📱 Phone remote:** on the same page, switch on **Phone remote**, click **Show QR code** and scan it with your phone's camera. Your phone must be on the same Wi-Fi as your PC. You get big buttons for everything on that page, plus a box to send a message to every chat. Never show the QR code on stream: anyone with the link can press your buttons. **New link** makes the old one stop working.

---

## ⚠️ Known limits (no need to report these)

- Kick chat uses the same live feed as Kick's own website. If Kick changes it, Kick chat may stop until a FeatWave update.
- Twitch only lets the app that made a reward edit it. FeatWave can play sounds and messages for rewards made on the website or by other apps (like Mix It Up), but to edit one in FeatWave, delete it there and make it again with **+ New Reward**.
- Spotify song requests need Spotify Premium (Spotify's rule). YouTube song requests are free; typing song names (instead of links) needs a free YouTube API key.
- First-chat sounds play on a viewer's first message - Kick doesn't tell apps when someone just opens your stream.
- Kick doesn't share its badge pictures, so FeatWave draws simple ones. You can pick your own in **Settings**.
- Updated from an older version? **Log in to Twitch once more** (Connections page). New features like `!clip` and Hype Train alerts need new Twitch permissions.
- **YouTube:** each Google app gets a free daily allowance from YouTube. FeatWave uses it sparingly and warns in the Log if you get close. If it runs out, YouTube chat pauses until midnight Pacific time. YouTube doesn't tell apps about new subscribers or raids in real time, and its chat messages are 200 characters max (FeatWave splits longer replies).
- **YouTube login every 7 days?** Set your Google app to **In production** (the YouTube key guide shows where).
- **Velora:** making or editing Velora channel point rewards inside FeatWave, Velora emotes as pictures and a Velora viewer list aren't possible yet.
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
