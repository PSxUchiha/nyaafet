<h1 align="center">NyaaFet</h1>
<p align="center"> CLi tool which scrapes nyaa for anime magnet links and streams it with peerflix</p>

##
<p align="center">
<img src="./example.gif" alt="Video Preview" width="500px">
</p>


### How does this work?

This is a shell script which scrapes nyaa.si and gets magnet links.  
After this it uses [peerflix](https://github.com/mafintosh/peerflix) to stream the video from magnet link.
For scraping it uses simple gnu utils like sed, awk. 

## Requirements

* [peerflix](https://github.com/mafintosh/peerflix) - A tool to stream torrent. `sudo npm install peerflix -g`

## Installation

### cURL
cURL **nyaafet** to your **$PATH** and give execute permissions.

```sh
$ sudo curl -sL "https://raw.githubusercontent.com/PSxUchiha/nyaafet/master/nyaafet" -o /usr/local/bin/nyaafet
$ sudo chmod +x /usr/local/bin/nyaafet
```
- To update, just do `curl` again, no need to `chmod` anymore.
- To uninstall, simply remove `nyaafet` from your **$PATH**, for example `sudo rm -f /usr/local/bin/nyaafet.

## License
This project is licensed under [GPL-3.0](https://raw.githubusercontent.com/Illumina/licenses/master/gpl-3.0.txt).



