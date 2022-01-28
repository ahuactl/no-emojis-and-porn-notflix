<h1 align="center">Rofi Notflix</h1>

A rofi fork of notflix.

> Watch BugsWriters video on it - [bugswriter's notflix](https://youtu.be/RFJCL9C46Mc)

### How does this work?

This is a shell script. It scrapes 1337x and gets the magnet link.
After this it uses [webtorrent](https://webtorrent.io/) to stream the video from the magnet link.
For scraping, the script uses simple gnu utils like sed, awk, paste, cut.

## Usage

```console
$ notflix [query]
$ tmpdir=[path] notflix [query]
```

## Requirements

* [webtorrent](https://webtorrent.io/) - A tool to stream torrent. `npm install webtorrent-cli -g` or `yay -S webtorrent-cli` for Arch Users
* [rofi](https://github.com/davatorium/rofi)

## Installation

```console
# curl -sL "https://raw.githubusercontent.com/ahuactl/rofi-notflix/master/notflix" -o /usr/local/bin/notflix
# chmod +x /usr/local/bin/notflix
```
- To update, just do `curl` again, no need to `chmod` anymore.
- To uninstall, simply remove `notflix` from your `$PATH`, for example `sudo rm -f /usr/local/bin/notflix`.

## License
This project is licensed under [GPL-3.0](https://raw.githubusercontent.com/Illumina/licenses/master/gpl-3.0.txt).

