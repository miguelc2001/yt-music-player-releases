# YT Music Player

A lightweight, Spotify-style desktop player for your YouTube music, built with Tauri 2 and Svelte 5.
It uses only official Google APIs: the YouTube Data API v3 for your library and search, and the
YouTube IFrame Player for playback.

This repository only hosts the Windows installer. The source code is private.

## Download

**[Download the latest installer](https://github.com/miguelc2001/yt-music-player-releases/releases/latest/download/YT-Music-Player-setup.exe)** (Windows 10/11, x64)

Or see all versions on the [Releases page](https://github.com/miguelc2001/yt-music-player-releases/releases).

## Invite-only beta

The app is in an invite-only beta. Google only lets accounts on the app's test-user list sign in,
so you'll need to be added before you can use it. Email
[miguelcorreia.dev@gmail.com](mailto:miguelcorreia.dev@gmail.com) with the Google account you use
for YouTube Music.

When you sign in, Google shows a warning that the app isn't verified. Choose **Continue**.

## Installing

The installer isn't code-signed yet, so Windows SmartScreen may show "Windows protected your PC".
Click **More info**, then **Run anyway**.

## Features

- Sign in with your Google account; your playlists and Liked Songs show up in the sidebar
- Library sidebar, home, playlist pages tinted from the cover art, search, now-playing panel
- Queue with play next / add to queue, shuffle, repeat, seek and volume
- Like songs and add them to your playlists
- Media keys work even when the app isn't focused
- Small installer that uses the system WebView2 instead of bundling Chromium

## Limits of the official API

- Searches are limited to roughly 100 a day across all users, and results are cached for 24 hours.
- Only playlists you own and your liked songs are available. Saved albums, followed artists and
  radio aren't exposed by the official API.
- Some videos don't allow playback outside youtube.com; the player skips them.
