<h1 align="center">NOTFLIX</h1>
<p align="center">f@#k netflix use notflix a tool which search magnet links and stream it with peerflix</p>

##
<p align="center">
<img src="./notflix.gif" alt="Video Preview" width="500px">
</p>

> Watch this video to understand - [bugswriter's notflix](https://youtu.be/FbE19_omaWY)

### How does this work?

This is a shell script. It scape 1337x and get the magnet link.
After this it use [webtorrent-cli](https://github.com/webtorrent/webtorrent-cli) to stream the video with mpv from magnet link.
For scraping script use simple gnu utils like sed, awk, paste, cut.

## Requirements

* [webtorrent-cli](https://github.com/webtorrent/webtorrent-cli) - A tool to stream torrent. `sudo npm install webtorrent-cli -g` or `paru -S webtorrent-cli` for Arch Users

## Installation

### cURL
cURL **notflix** to your **$PATH** and give execute permissions.

```sh
$ sudo curl -sL "https://raw.githubusercontent.com/zakky20/notflix-dmenu/master/notflix" -o /usr/local/bin/notflix
$ sudo chmod +x /usr/local/bin/notflix
```
- To update, just do `curl` again, no need to `chmod` anymore.
- To uninstall, simply remove `notflix` from your **$PATH**, for example `sudo rm -f /usr/local/bin/notflix.

## License
This project is licensed under [GPL-3.0](https://raw.githubusercontent.com/Illumina/licenses/master/gpl-3.0.txt).
