# DeskDisplay Server

Run the DeskDisplay server on your own computer or Raspberry Pi.

Your DeskDisplay gets its picture from a server. By default that is the Board & Base
server (`api.boardandbase.com`). With this download you can run the same server at
home instead. Your display then keeps working even if the Board & Base server is ever
offline. You can switch back and forth at any time, without a firmware update.

## Download

Go to **[Releases](https://github.com/boardandbase/matrixOS/releases/latest)** and pick:

| You have | Download |
|---|---|
| Windows 10 or 11 (64-bit) | `deskdisplay-server-…-windows-x64.zip`: everything included, nothing to install |
| Raspberry Pi 3/4/5 (64-bit OS), Linux or macOS | `deskdisplay-server-….tar.gz`: needs Python 3.11 or newer |

## Quick start

1. Unzip the download, for example to `C:\DeskDisplay`.
2. Start it: double-click `start.bat` on Windows, or run `sh start.sh` on a Pi, Linux or macOS.
3. The window shows the display server URL, like `ws://192.168.1.20:8000/ws/device`.
4. Open `http://<display-ip>/config`, replace **WebSocket URL** with that URL and
   click **Opslaan & Herstart** (Save & Restart).
5. Choose your apps at `http://<display-ip>/dashboard`.

To switch back, enter `ws://api.boardandbase.com/ws/device` on the same page. Your
apps on the Board & Base server are still there.

The full guide is in `README.md` inside the download and on
[boardandbase.com/docs.html#self-host](https://www.boardandbase.com/docs.html#self-host).

## What works on your own server

- Clocks, weather, pixel art and animations, Spotify, Bambu Lab printer, Home Assistant
  push, and your own Pixlet/Tronbyt-compatible apps
- Your own apps may reach any internet service and devices on your home network
- Crypto, stock, ETF, metal and forex tickers and Pixel Pet need Board & Base's
  market-data service and don't work on your own server
- Firmware updates: switch the display back to the Board & Base server for a few minutes

## License

The DeskDisplay Server is free to run and modify for your own DeskDisplay devices.
It is not open source. See [LICENSE.md](LICENSE.md).

Questions? Email info@boardandbase.com.
