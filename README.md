<p align="center">
    <img src="./img/logo.png">
</p>

`phetch` is a terminal client designed to help you quickly navigate the gophersphere: use arrow keys to move around, press a number to jump to a link, or just start typing - phetch is always in incremental search mode when viewing a gopher menu.

## features

- <1MB executable for linux and mac
- technicolor design (based on [GILD](https://github.com/dvkt/gild))
- no nonsense keyboard navigation
- supports gopher searches, text and menu pages, and downloads
- save your favorite gopherholes with bookmarks
- opt-in history tracking

## usage

    phetch                           launch and show start page
    phetch <gopher-url>              open gopherhole at url
    phetch -r, --raw <gopher-url>    print raw gopher response
    phetch -h, --help                show this screen
    phetch -v, --version             show phetch version

    Once you've launched phetch, use `ctrl-h` to view the on-line help.

## installation

Binaries for Linux, Mac, and Raspberry Pi are available at https://github.com/dvkt/phetch/releases:

- [phetch-linux-x86_64.tar.gz](https://github.com/dvkt/phetch/releases/download/v0.1.3/phetch-linux-x86_64.tar.gz)
- [phetch-linux-armv7.tar.gz (RPi)](https://github.com/dvkt/phetch/releases/download/v0.1.3/phetch-linux-armv7.tar.gz)
- [phetch-macos.zip](https://github.com/dvkt/phetch/releases/download/v0.1.3/phetch-macos.zip)

Just unzip/untar the `phetch` program into your $PATH and get going!

## development

    cargo run -- <gopher-url>

## gifcast

[![asciicast](./img/start-play.png)](http://dvkt.io/phetchcast/v0.1.0.gif)

## screenies

![DOS Archive](./img/dos.png)

![Menu View](./img/menu-view.png)

![Text View](./img/text-view.png)

## todo

- [ ] activate search mode with / or i
- [ ] de-activate search mode with ESC
- [ ] ENTER on non-match is an error
- [ ] show "SEARCH MODE" indicator in bottom right?
- [ ] update help
- [ ] add credits page
- [ ] telnet: gopher://bitreich.org/1/lawn/bbs

## bugs

- [ ] gopher://1436.ninja/1/twit.cgi ("iWritten and performed by Nathaniel" weirdness)

## future features

- [ ] Toggle bookmarks instead of just appending to the file
- [ ] Bookmarks save the title of the current page
- [ ] Incremental search in Text views
- [ ] Linked gopher and http URLs in Text views
- [ ] TLS -- https://dataswamp.org/~solene/2019-03-07-gopher-server-tls.html
- [ ] Fuzzy Find incremental search
