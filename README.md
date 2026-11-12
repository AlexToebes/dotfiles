# dotfiles

My dotfiles, managed with [GNU Stow](https://www.gnu.org/software/stow/).

Each top-level folder is a stow package that mirrors the layout of `$HOME`.

## Packages

- `kitty` – [kitty](https://sw.kovidgoyal.net/kitty/) terminal config

## Usage

```bash
brew install stow
git clone <repo-url> ~/dotfiles
cd ~/dotfiles
stow kitty      # symlink a single package
stow */         # or all of them
```

Remove a package's symlinks with `stow -D kitty`.

## Adding a package

Create `<name>/` mirroring the path from `$HOME`, e.g. `nvim/.config/nvim/init.lua`, then run `stow <name>`.
