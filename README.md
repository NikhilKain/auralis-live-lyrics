<a id="top"></a>
<div align="center">

<img src="docs/auralis_logo.png" width="240" alt="Auralis logo">

# 🎵 AURALIS

<img src="https://readme-typing-svg.demolab.com/?font=JetBrains+Mono&weight=600&size=20&duration=3000&pause=1200&color=5B4FCF&center=true&vCenter=true&width=680&lines=Floating%2C+time-synced+lyrics+for+any+music+app;Read+along.+Sing+along.+Never+switch+apps.;No+account+%C2%B7+No+ads+%C2%B7+Just+lyrics" alt="typing tagline" width="680" height="40">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:5B4FCF,100:C9B6FF&height=90&section=header&animation=fadeIn" width="100%" height="90" alt="divider">

[![Get it on Google Play](https://img.shields.io/badge/Google_Play-Download-5B4FCF?style=for-the-badge&logo=googleplay&logoColor=white&labelColor=0d1117)](https://play.google.com/store/apps/details?id=com.vythera.auralis)
[![Android](https://img.shields.io/badge/Android-8.0+-5B4FCF?style=for-the-badge&logo=android&logoColor=white&labelColor=0d1117)](#)
[![Version](https://img.shields.io/badge/Version-1.0.1-5B4FCF?style=for-the-badge&labelColor=0d1117)](#)
[![Price](https://img.shields.io/badge/Price-Free-5B4FCF?style=for-the-badge&labelColor=0d1117)](#)

<br/>

[![About](https://img.shields.io/badge/About-5B4FCF?style=for-the-badge)](#about)
[![Features](https://img.shields.io/badge/Features-C9B6FF?style=for-the-badge&labelColor=5B4FCF)](#features)
[![Privacy](https://img.shields.io/badge/Privacy-5B4FCF?style=for-the-badge)](#privacy)
[![Screenshots](https://img.shields.io/badge/Screenshots-C9B6FF?style=for-the-badge&labelColor=5B4FCF)](#screenshots)
[![Under the Hood](https://img.shields.io/badge/Under_the_Hood-5B4FCF?style=for-the-badge)](#under-the-hood)
[![Support](https://img.shields.io/badge/Support-C9B6FF?style=for-the-badge&labelColor=5B4FCF)](#support)

</div>

---

<a id="about"></a>
## 🎧 What is Auralis?

Play a song in almost any music player and Auralis detects it, fetches the matching **time-synced lyrics**, and shows them in a sleek **floating pill** that lives above your other apps. Tap to expand it into a full card, and the lyrics scroll line-by-line, perfectly in step with the music.

No account. No ads. Just lyrics, everywhere.

<a id="features"></a>
## ✨ Features

<table>
<tr>
<td width="50%" valign="top">

**🎤 Live, time-synced lyrics**
Scroll in real time with the song.

**🫧 Floats over any app**
A draggable pill that hovers above your other apps, with a foreground service keeping it alive while you play.

**🃏 Pill or big card**
Two overlay sizes to start in — a compact pill or a big draggable card — plus a tap-to-expand bar for a quick glance without going full-screen.

**🔦 Line-by-line highlighting**
Always know exactly where you are.

</td>
<td width="50%" valign="top">

**⏱️ Per-song sync memory**
Nudge the timing (Sync) or scroll speed (Pace) once — Auralis remembers it per track.

**🎨 Fully customizable**
Background, text, and accent colors with a live preview while you pick, plus size, corner roundness, and position.

**⏯️ Quick controls**
Play, pause, next, previous, and fine sync adjustment from the pill itself.

**📄 Bring your own lyrics**
Import a `.lrc` or `.txt` for any track the sources can't find.

</td>
</tr>
</table>

## 🔎 The lyrics engine

Auralis doesn't rely on a single provider. When a song starts, it queries **LrcLib, KuGou, and NetEase** in parallel for time-synced lyrics, and keeps whichever result's duration lines up best with the actual track. If nothing synced turns up, it falls back to **Lyrics.ovh** for plain text. iTunes is queried separately, purely to fill in a track duration when the player doesn't report one, so matching stays accurate. Results are cached on-device so a song you've already looked up never needs a re-fetch.

<a id="privacy"></a>
## 🔐 Privacy

Auralis needs two one-time permissions:

| Permission | Why |
|---|---|
| **Notification access** | Used *only* to detect the currently playing song (title + artist) to look up matching lyrics. Auralis never reads your personal notifications. |
| **Display over other apps** | So the lyrics overlay can float on top. |

Only the song title and artist ever leave your device — to fetch lyrics from the sources above. Auralis also sends anonymous, non-identifying usage analytics (feature counts, lyric-match status, source name) to help fix bugs — never lyric text, song titles, or artist names. Auralis collects no personal information and never sells your data.

<a id="screenshots"></a>
## 📱 Screenshots

<div align="center">

<img src="docs/s1.png" width="200" height="400" alt="Big karaoke-style view"> <img src="docs/s2.png" width="200" height="400" alt="Perfectly in sync, line-by-line"> <img src="docs/s3.png" width="200" height="400" alt="Lyrics that float over any app"> <img src="docs/s4.png" width="200" height="400" alt="Home screen">

</div>

## 📲 Get it

<div align="center">

[![Download Auralis on Google Play](https://img.shields.io/badge/Download_Auralis-Google_Play-5B4FCF?style=for-the-badge&logo=googleplay&logoColor=white&labelColor=0d1117)](https://play.google.com/store/apps/details?id=com.vythera.auralis)

Requires Android 8.0 (Oreo) or newer.

</div>

<a id="under-the-hood"></a>
## 🛠 Under the hood

<div align="center">

<img src="https://skillicons.dev/icons?i=kotlin,androidstudio,git,github,gradle&theme=dark" alt="tech icons">

</div>

| | |
|---|---|
| Language | Kotlin |
| UI | Jetpack Compose, Material 3 (Expressive-styled) |
| DI | Hilt |
| Data | Room, DataStore |
| Networking | Retrofit + Gson |
| Background | Foreground service (media playback) |
| Min / target / compile SDK | 26 / 36 / 36 |

## 💬 Feedback

Found a bug or have a feature idea? Use **Settings → Help & Support → Send feedback** in the app.

<a id="support"></a>
## 💖 Support

If Auralis is useful to you, sharing it with a friend goes a long way for a one-person project.

### ☕ Buy Me a Coffee

Hey! 👋 I'm Nikhil, an indie Android developer building this project in my free time — lyrics that float over whatever you're already using, without a login or a subscription.

Every contribution goes directly toward new features, bug fixes, performance improvements, and long-term development.

<div align="center">

[![Buy Me a Coffee](https://img.shields.io/badge/☕_Buy_Me_a_Coffee-Support_Development-5B4FCF?style=for-the-badge&labelColor=0d1117)](https://narzo7.gumroad.com/l/nhlevz)

*Thank you for supporting independent development ❤️*

</div>

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:C9B6FF,100:5B4FCF&height=90&section=footer" width="100%" height="90" alt="divider">

*Made by Vythera.*

[⬆ Back to top](#top)

</div>
