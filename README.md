# Easy IPTV for Windows

Easy IPTV brings the bundled movie and series catalog to a desktop interface with live TV, M3U playlists, favorites, and playback history. It runs without an Android emulator.

## Open the Windows app

The Windows download targets 64-bit Windows 10 and 11.

1. Download **Easy-IPTV-Setup-x64.exe** to your PC.
2. Run the installer and follow the setup prompts.
3. Open **Easy IPTV** from the Start menu.

Open **Live TV** to browse the included playlist sources. Select **Add playlist** to load channels from an M3U URL or a local `.m3u` file. Favorites and playback history are stored on the device. An internet connection is needed to watch online content.

This edition uses the APK's bundled movie and show library. It omits the Android version's online Discover screen and XMLTV program guide.

## Host the web app with GitHub Pages

1. Extract the web ZIP and add its contents to the root of a GitHub repository. Keep `assets` and `vendor` in their original folders.
2. In the repository, open **Settings** → **Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**. Select your default branch and **/(root)**, then save.
4. Open the site URL shown under **Pages**. In Microsoft Edge, select **Apps** → **Install this site as an app** from the browser menu. In Chrome, use the install icon in the address bar or the install option in the browser menu.

In the hosted app, playlist URLs and streams fetched by the player need HTTPS and browser-compatible CORS headers. The Windows app supports additional streams by fetching them through the desktop runtime. Stream availability and codec support also depend on the provider and device.

The bundled HLS player is distributed under its [license](vendor/hls-LICENSE.txt). Catalog entries list their original sources.
