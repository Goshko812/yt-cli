# yt-cli

A very *questionably* written Bash script that lets you:

- 🔍 Search YouTube  
- 📋 Select a result interactively in your terminal  
- ▶️ Play it with `mpv` (via `yt-dlp`)  

All using only Bash, `yt-dlp`, `jq`, and `mpv`.  
Why? I dunno. It works.

> There are like... a hundred better ways to do this.  
> But this one exists now. So. Yeah.

## Dependencies

You need:
- `yt-dlp`
- `mpv`
- `jq`

Install them with your package manager:

```bash
# Debian/Ubuntu
sudo apt install yt-dlp mpv jq

# Arch
sudo pacman -S yt-dlp mpv jq

# Fedora
sudo dnf install yt-dlp mpv jq
```

## Installation

Clone the repo and stick the `yt` script somewhere in your `$PATH`. For example:

```bash
git clone https://github.com/Goshko812/yt-cli
cd yt-cli
chmod +x yt

# System-wide install (requires root)
sudo mv yt /usr/local/bin

# OR user-only install (no root)
mkdir -p ~/.local/bin
mv yt ~/.local/bin
# make sure ~/.local/bin is in your $PATH
```

## Usage

```bash
yt lo-fi hip hop
```

Or just run `yt` and it'll ask what you want to search for.
