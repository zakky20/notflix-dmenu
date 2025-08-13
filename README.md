<h1 align="center">NOTFLIX</h1>
<p align="center">f@#k netflix use notflix a tool which search magnet links and stream it with peerflix</p>

##
<p align="center">
<img src="./notflix.gif" alt="Video Preview" width="500px">
</p>

> Watch this video to understand - [bugswriter's notflix](https://youtu.be/FbE19_omaWY)

### How does this work?

This is a dmenu script. It searches 1337x and gets the magnet link for which media u choose.
After this it uses [webtorrent-cli](https://github.com/webtorrent/webtorrent-cli) to stream the video with mpv from the magnet link.
For scraping script it uses simple gnu utils like sed, awk, paste, grep, cut.

## Requirements

* [webtorrent-cli](https://github.com/webtorrent/webtorrent-cli) - A tool to stream torrent. `sudo npm install webtorrent-cli -g` or `paru -S webtorrent-cli` / `yay -S webtorrent-cli` for Arch Linux Users

## Installation

### cURL
cURL **notflix** to your **$PATH** and give execute permissions.

```sh
--- If you are using sudo ---
sudo curl -sL "https://raw.githubusercontent.com/zakky20/notflix-dmenu/master/notflix" -o /usr/local/bin/notflix
sudo chmod +x /usr/local/bin/notflix

--- If you are using doas instead of sudo ---
doas curl -sL "https://raw.githubusercontent.com/zakky20/notflix-dmenu/master/notflix" -o /usr/local/bin/notflix
doas chmod +x /usr/local/bin/notflix
```
- To update, just do `curl` again, no need to `chmod` anymore.
- To uninstall, simply remove `notflix` from your **$PATH**, for example `sudo rm -f /usr/local/bin/notflix.

## License
This project is licensed under [GPL-3.0](https://raw.githubusercontent.com/Illumina/licenses/master/gpl-3.0.txt).
