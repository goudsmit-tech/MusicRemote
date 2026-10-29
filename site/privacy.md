---
title: Privacy
description: Music Remote collects no data. What stays on your Macs, and the one thing that goes to Apple.
---

_Effective 29 October 2026. Music Remote for Mac is made by Goudsmit Technologies._

**In short:** Music Remote collects no personal data, has no accounts, no analytics and no ads, and
sends nothing to us. It talks to your own Macs and receiver on your home network. The only thing
that leaves your network is a lookup of missing album artwork at Apple.

## What stays on your Macs

Music Remote has two parts: the menu bar app, and a helper that runs on the Mac that plays the
music (Settings → This Mac). They talk to each other directly, over your local network. The helper
refuses connections from outside your local network, and requests from web browsers.

What they keep is stored on your own Macs and never sent to us:

- **Settings**: the Macs you connected to (their names, addresses and, for waking them, their
  network hardware addresses), your receiver's address, and your preferences.
- **Access tokens**, only for helpers set up to require one: in your login keychain.
- **Up Next and album artwork**: the helper's queue and a cache of album covers, in its Application
  Support folder, together with a log of what it did.

Deleting the app and these folders removes all of it.

## What goes to Apple

- **Missing artwork.** Music only hands over artwork for songs stored on the Mac. For other songs,
  the helper asks Apple's public iTunes Search service for the cover, by sending the artist,
  album and song title. Apple sees that request, including your IP address, as with any request to
  its servers; [Apple's privacy policy](https://www.apple.com/legal/privacy/) applies. Covers are
  cached so the same album isn't looked up again.
- **Crash reports**, for the Mac App Store version, and only if you chose to share analytics with
  app developers in System Settings → Privacy & Security → Analytics & Improvements. Apple then
  passes crash reports on to us, without information that identifies you.

## On your network

- **Your Macs**: the app finds them with Bonjour, and can wake one with a Wake-on-LAN message.
- **A Yamaha receiver**, if you set one up: the app controls it directly, and can look for it on
  the network.

None of this goes beyond your local network.

## Permissions

macOS asks before Music Remote may:

- **control Music**, on the Mac that plays the music (Automation);
- **find devices on your local network**;
- **show notifications** when the song changes.

You can change these at any time in System Settings → Privacy & Security, and under Notifications.

## Downloads

If you download Music Remote from GitHub or install it with Homebrew, GitHub's privacy statement
covers that download. The Mac App Store version is covered by Apple's privacy policy.

## Children

Music Remote collects no data from anyone, children included.

## Changes and questions

If this policy changes, the new version will be here, with its date. Questions? Open an
[issue on GitHub](https://github.com/goudsmit-tech/MusicRemote/issues) or use the contact button
on [goudsmit.tech](https://goudsmit.tech).
