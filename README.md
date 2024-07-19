# Worthant's Neovim configuration

## 🛠️ Installation

Generally, there are **2 ways** of installing anything into `.config/`

### 1. Clone repo anywhere you want, and create a soft link there

#### Clone the repository

```shell
git clone https://github.com/worthant/nvim.git <your_path>
```

#### Go into ~/.config and create a symbolic link

```shell
cd ~/.config
ln -s <path_to_cloned_repo> nvim
```

### 2. Backup your files and just clone the repo into `.config/`

#### Make a backup of your current nvim and shared folder

```shell
mv ~/.config/nvim ~/.config/nvim.bak
mv ~/.local/share/nvim ~/.local/share/nvim.bak
```

#### Clone the repository

```shell
git clone https://github.com/worthant/nvim.git ~/.config/nvim
```

## Usage

### Start Neovim

```shell
nvim
```

### Mappings

#### Custom

| Action           | Mappings      |
| ---------------- | ------------- |
| Glow Markdown    | `Leader + gw` |
| Preview Markdown | `Leader + md` |

#### Terminal

| Action              | Mappings      |
| ------------------- | ------------- |
| Horizontal terminal | `Leader + th` |
| Vertical terminal   | `Leader + tv` |
| Toggle any terminal | `1`           |

#### Sessions

| Action       | Mappings     |
| ------------ | ------------ |
| All sessions | `Leader + r` |

#### Colorscheme

| Action        | Mappings      |
| ------------- | ------------- |
| Select scheme | `Leader + ft` |

## TODOs:

- [x] Merge `base` & `user` configs into monolithic config
- [x] Create a separate repo for mantaining merged config
- [ ] Popup astronvim's notifications are annoying as hell - move them to the
      background or remove completely
- [ ] Add all configs for lsp's, there shouldn't be any errors
- [x] Setup formatter(black) and linter(ruff) for `Python`, using null-ls plugin
- [ ] Setup formatter and linter correctly (typescript, javascript, c)
  - Note: they shouldn't interfere with eachother. Now javascript is getting
    formatted by clang and other bs xD
- [x] Add lsp for java
- [x] Add xml formatter (`lemminx`)
- [ ] Add custom mappings for compiling cpp files using my `cmp` script
- [ ] Add custom mappings for neatly opening a terminal (**<leader>th can't
      close terminal - map to cntrl k and then close**)
- [x] Add custom mappings for markdown preview and glow
- [ ] Add support for clojure (lsp, debug, e.t.c.)
- [ ] Add debugger for cpp, learn how to use it
- [ ] fix `Themery` plugin for changing themes
- [x] add confiluration for null_ls and prettier formatters
- [x] add [multi-cursor plugin](https://github.com/smoka7/multicursors.nvim) for
      my setup
- [ ] Try `Neorg`
- [x] add preview plugins for markdown
  - [x] `markdown-preview`
  - [x] `glow`
- [x] Use those for a while and customise what i feel is needed
- [x] add `wakatime` plugin
- [x] add `lazygit`
- [x] add `bottom`
- [x] add lsp servers for js, ts, html, css, twcss
- [x] configure highlighting & personal theme
- [x] add config for clangd lsp server (need for `cpp`)