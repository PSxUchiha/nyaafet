# nyaafet

A Bash script for interactively searching [nyaa.iss.ink](https://nyaa.iss.ink) torrents, previewing results, and sending selected magnet links directly to your default torrent client—all from your terminal.

---

## Features

- **Search Nyaa.si**: Enter any query and get the top torrents sorted by seeders.
- **Interactive Selection**: Browse results with [fzf](https://github.com/junegunn/fzf) and see torrent details in a preview pane.
- **Instant Download**: Press Enter to open the magnet link in your default torrent app.
- **Customizable Results**: Use `-n` to set how many results to display (default: 5).
- **Help Option**: Use `-h` or `--help` for usage instructions and examples.

---

## Dependencies

- **bash** (version 4 or higher)
- **curl** (for fetching search results)
- **grep** (with Perl regex support, i.e., GNU grep)
- **fzf** (interactive fuzzy finder; [install instructions](https://github.com/junegunn/fzf#installation))
- **xdg-open** (Linux), **open** (macOS), or **start** (Windows/Git Bash)  
  - Used to open magnet links with your default torrent client

---

## Installation

1. **Clone or download** this script.
2. Make it executable:
```
chmod +x nyaa-search.sh
```
3. Ensure all dependencies are installed and available in your `$PATH`.

---

## Usage

```
./nyaa-search.sh [OPTIONS] SEARCH QUERY
```

- **SEARCH QUERY**: The terms to search for (e.g., `"solo leveling"`).
- **OPTIONS**:
  - `-n NUM`  Number of results to display (default: 5)
  - `-h`, `--help` Show usage instructions

### Examples

- Search for "solo leveling" (top 5 results):
```
./nyaa-search.sh solo leveling
```
- Show top 10 results for "domestic girlfriend":
```
./nyaa-search.sh -n 10 domestic girlfriend
```
- Show help:
```
./nyaa-search.sh --help
```

---

## Interactive Usage

- **Type** to filter results.
- **Arrow keys** to move selection.
- **Preview pane** (right or top) shows torrent title and magnet link.
- **Press Enter** to open the selected magnet link in your default torrent client.

---

## Troubleshooting

- If you see no results, ensure your dependencies are installed and up to date.
- If magnet links do not open, check that `xdg-open` (Linux), `open` (macOS), or `start` (Windows) is available and your torrent client is set as the default handler for magnet links.
- For best results, use GNU grep (with `-P` support).

---

## License

This script is released under the MIT License.

---

## Credits

- [fzf](https://github.com/junegunn/fzf) by Junegunn Choi
- [nyaa.iss.ink](https://nyaa.iss.ink) for torrent search data

---

## License
This project is licensed under [GPL-3.0](https://raw.githubusercontent.com/Illumina/licenses/master/gpl-3.0.txt).



