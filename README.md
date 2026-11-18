<!-- markdownlint-disable MD033 MD041 -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="playlet-app/src/images/vector/logo-dark.svg"/>
    <img src="playlet-app/src/images/vector/logo-light.svg" alt="BlueTube Logo" width="480"/>
  </picture>
  <br/><br/>
  <a href="https://github.com/Kovee98/bluetube/actions/workflows/release-assets.yml">
    <img alt="Build Status" src="https://img.shields.io/github/actions/workflow/status/Kovee98/bluetube/release-assets.yml"/>
  </a>
  <a href="https://github.com/Kovee98/bluetube/releases">
    <img alt="Current Release" src="https://img.shields.io/github/release/Kovee98/bluetube.svg"/>
  </a>
  <a href="https://hosted.weblate.org/engage/playlet/">
    <img src="https://hosted.weblate.org/widget/playlet/svg-badge.svg" alt="Translation status" />
  </a>
  <a href="/LICENSE">
    <img alt="AGPL-3.0 license" src="https://img.shields.io/github/license/iBicha/playlet.svg"/>
  </a>
  <a href="https://github.com/iBicha/playlet/wiki">
    <img alt="Channel Stats" src="https://img.shields.io/badge/%F0%9F%93%88-channel_stats-blue"/>
  </a>
</p>

# BlueTube

BlueTube is an unofficial YouTube client for Roku, forked from
[Playlet by iBicha and contributors](https://github.com/iBicha/playlet).
It is not affiliated with YouTube or Google.

## What's new since Playlet

- **Subscriptions on Roku and in the browser companion.** Sign in with a Roku
  profile, then open **Subscriptions** to see a combined **All** feed or switch to
  a single channel. Use **Refresh** to check for new uploads.
- **See what changed and pick up where you left off.** Blue dots mark channels
  with unseen uploads and clear when you open the channel. The channel list
  prioritizes recent uploads, with a small boost for channels you watch often.
  When watch history is available, video cards show resume progress.
- **BlueTube branding and releases.** The Roku tile, splash screen, navigation,
  and browser companion have a new blue look. Updates come from
  [BlueTube releases](https://github.com/Kovee98/bluetube/releases). Package
  filenames still use `playlet`, and compatible saved library URLs are migrated
  on startup without clearing profiles or settings.


## Screenshots

### BlueTube on Roku and in the browser

The browser screenshots use demo data. The Roku splash shows the new branding.

| All subscriptions: new-upload dots and watch progress | Channel view: videos from just one subscription |
| --- | --- |
| ![BlueTube subscriptions with a combined feed, blue dots, and watch progress](docs/screenshots/bluetube-subscriptions.png) | ![BlueTube subscriptions filtered to Trail Journal](docs/screenshots/bluetube-subscription-channel.png) |

| BlueTube's Roku splash screen | SponsorBlock settings in the browser companion |
| --- | --- |
| ![BlueTube splash screen with a blue play icon and wordmark](playlet-app/src/images/splash-screen_fhd.jpg) | ![SponsorBlock settings for enabling skips, notifications, and categories](docs/screenshots/bluetube-sponsorblock.png) |

### Features inherited from Playlet

These screenshots show the original Playlet styling; the features are still
available in BlueTube.

| Browse and search | Bookmarks and playlists |
| --- | --- |
| ![Roku search results](docs/screenshots/search.jpg) | ![Saved bookmarks on Roku](docs/screenshots/bookmarks.jpg) |

| Playback queue and picture-in-picture | Phone remote and casting |
| --- | --- |
| ![Roku playback queue with the current video in picture-in-picture](docs/screenshots/queue-pic-in-pic.jpg) | ![Phone browser controls for casting a video to Roku](docs/screenshots/webapp-cast.png) |

| YouTube and Invidious profiles | Invidious backend settings |
| --- | --- |
| ![Roku profile selector](docs/screenshots/profiles.jpg) | ![Roku Invidious instance settings](docs/screenshots/invidious-settings.jpg) |

See the [full screenshot gallery](./docs/screenshots/README.md) for more Roku and
browser views.

## Installation

BlueTube is currently distributed by sideloading, not through its own Roku Store
listing. Download `playlet-app.zip` from this fork's
[latest release](https://github.com/Kovee98/bluetube/releases/latest) and upload it
through your Roku's Development Application Installer. After the BlueTube rebrand,
install this app package once to update the Roku home-screen name and artwork;
library-only updates cannot change the installed app's manifest or splash images.

Roku supports one sideloaded app at a time; another sideload replaces it. See the
[upstream sideloading guide](https://github.com/iBicha/playlet/discussions/371)
and [distribution notes](./docs/README.md#bluetube-branding-and-roku-distribution).

## Features

- 🔥 No Ads (Not now, not ever)
- 🕵️ No Tracking
- 🛡️ Privacy driven (supports [Invidious](https://invidious.io/) backend)
- 🙋 User accounts (supports YouTube and Invidious accounts)
- ⚔️ [SponsorBlock](https://sponsor.ajay.app/) integration (skips undesirable sections in videos)
- 📱 Browse, search, and cast from phone using the YouTube app or the browser
- 🔮 Picture-in-picture mode
- ⚡ Fast! [Check out how we compare with the official YouTube app](https://youtu.be/qmSvA-QQW20)
- 🔤 Translated using [Weblate](https://hosted.weblate.org/projects/playlet/playlet/)

### Cast from phone

- Open "Remote" tab in BlueTube
  - Scan QR Code with Phone, and use the browser; OR
  - Use the YouTube app to connect using the same Wi-Fi; OR
  - Use the `Link with TV code` to connect

## Development

For BlueTube development, please see the [documentation](./docs/README.md).
The historical upstream notes below retain their original attribution to Playlet.

## Analytics and telemetry

Roku collects usage data, and you can find the data made available to Playlet in the [Wiki](https://github.com/iBicha/playlet/wiki).
Playlet could run on variaty of devices, with different capabilities and screen sizes, and different Invidious instances, in addition to the experimentation YouTube does based on account and/or ip.
This is why it was necessary to collect telemetry/diagnostics data, in order to capture issues and fix them. However, you can disable this feature in the settings.
But it's not enough, it's important to report any issues you encouter using Playlet, so they can be addressed.

## Why Playlet

```none
playlet - noun
play•let /ˈplālət/
: a short play
```

**Playlet** is about keeping the time you spend on YouTube short and useful. It values your time, so it does not show you ads, and allows you to skip sponsored sections and other irrelevant information that's designed to monitize you and/or waste your time.

There's a cliché about how a lot of open source software is **`"Made with ♡"`**. This project in particular is **not**.<br/>
**Playlet** was created out of **spite**, because I believe I have watched enough back-to-back, unskippable YouTube ads for a lifetime.

By removing all the bloat, the ads, the tracking, we could end up with an even faster app than the official one.

In any case, I hope you find **Playlet** useful, and pleasant to use.

## Disclaimer

**Playlet** does not serve or distribute any material from unauthorized sources.<br/>
**Playlet** is simply a frontend to other systems (such as [Invidious](https://github.com/iv-org/invidious)), bringing the watching experience to the TV, as opposed to the existing frontends that are web and mobile focused.<br/>
**Playlet** authors acknowledge that all trademarks and registered trademarks mentioned in this repository and related pages are the property of their respective owners. The use of these trademarks or trade names is for identification purposes only and does not imply any endorsement, affiliation, or sponsorship by the trademark owner.

<!-- markdownlint-configure-file {"MD024": { "siblings_only": true } } -->
