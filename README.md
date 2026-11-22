# winEufy

**Watch your Eufy Security cameras live on Windows.**

winEufy is a small Windows app that signs in with your Eufy account and shows all your cameras live, side by side, in one dark "control room" window. No phone, no browser, no Home Assistant server needed.

> winEufy is an unofficial, independent app. It is not made by, affiliated with or endorsed by Anker or Eufy.

## Download

Get the latest **winEufy x.y.z.exe** from the Releases page.

It is a portable app: there is nothing to install. Put the `.exe` anywhere you like (for example your desktop) and double-click it.

**Windows warning on first start**
winEufy is not code-signed, so Windows SmartScreen may show *"Windows protected your PC"*. Click **More info** → **Run anyway**. This only happens the first time.

## Requirements

- Windows 10 or 11 (64-bit)
- A Eufy Security account with your cameras on it
- Your PC on a network that can reach your cameras (normally your home network)

## Features

- **All cameras live at once** in a 1, 2×2 or 3×2 grid, or one camera full screen
- **Start all / Stop all** with one click
- **Keyboard navigation**: in full screen or single view, `Space` or `→` goes to the next camera, `Shift+Space` or `←` to the previous one, `Esc` goes back
- **Zoom**: in full screen, drag a rectangle with the left mouse button to zoom in on that area; right-click to zoom out
- **Live-view quality** per camera (Auto, 720p, 1080p, Max, or Ultra 4K on 4K models), on cameras that support changing it
- **Stream info** on every tile: camera name, model, resolution, frame rate, video codec and Wi-Fi signal (can be switched off)
- **Remembers your login** (optional) and your layout
- **Update check**: winEufy tells you when a new version is available

## Privacy

- winEufy talks directly to Eufy's own servers and to your HomeBase or cameras, just like the Eufy app. There is no other server in between.
- Your login details stay on your PC. If you tick **Remember password**, the password is stored encrypted with Windows' own protection, readable only by your Windows account.
- winEufy does not record video and does not collect or send any usage data. The only other connection it makes is the update check, which reads the latest release from this GitHub page.

## Good to know

- **Battery cameras** can take a few seconds to wake up before the picture appears. If a camera does not respond, winEufy retries automatically.
- **H.265 cameras** play directly on most PCs. On a PC without H.265 support, winEufy converts the video, which needs [[FFmpeg](https://ffmpeg.org/)](https://ffmpeg.org) installed.
- **Live-view quality** is a setting on the camera itself, so a change made in winEufy may also show up in the Eufy app.
- Live view only, for now: no recordings, events or two-way audio.

## Built with

- [eufy-sdk](https://github.com/mega-yfue/eufy-sdk): unofficial SDK for the Eufy cloud
- [Electron](https://www.electronjs.org)
- [JMuxer](https://github.com/samirkumardas/jmuxer)
- [FFmpeg](https://ffmpeg.org) (optional)

## Author

Made by **Erik Lenaerts**.
