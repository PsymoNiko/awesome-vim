
<!--
  Awesome Vim - A modern, feature-rich Vim configuration
  https://github.com/PsymoNiko/awesome-vim
-->

# 🚀 Awesome Vim

[![Vim Version](https://img.shields.io/badge/Vim-8.0%2B-019733?logo=vim&logoColor=white)](https://www.vim.org/)
[![Neovim](https://img.shields.io/badge/Neovim-0.5%2B-57A143?logo=neovim&logoColor=white)](https://neovim.io/)
[![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)
[![License: BSD 2-Clause](https://img.shields.io/badge/License-BSD%202--Clause-blue.svg)](https://opensource.org/licenses/BSD-2-Clause)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)
[![Shell Script](https://img.shields.io/badge/installer-bash-4EAA25?logo=gnu-bash&logoColor=white)](./install.sh)

> **A batteries‑included, modern Vim distribution that just works.**  
> Perfect for developers, writers, and terminal lovers who want IDE‑like power without leaving Vim.

![Screenshot Placeholder](https://via.placeholder.com/800x450?text=Add+your+screenshot+here)  
*Replace this with an actual screenshot or an animated GIF of your Vim setup.*


## ✨ Features at a glance

- **🔌 Smart plugin management** – uses [vim-plug](https://github.com/junegunn/vim-plug) for lightning‑fast, parallel updates.
- **💡 LSP‑ready** – seamlessly integrates with `coc.nvim` for autocompletion, go‑to‑definition, and diagnostics.
- **🌲 Beautiful syntax** – improved highlighting and folding via Tree‑sitter (Neovim) or modern syntax plugins (Vim).
- **🔍 Fuzzy finding everywhere** – files, buffers, grep results, commands – with [fzf](https://github.com/junegunn/fzf) and [fzf.vim](https://github.com/junegunn/fzf.vim).
- **📁 Project drawer** – `NERDTree` with git integration.
- **🎨 Gentle on the eyes** – a carefully tuned colorscheme (Gruvbox / OneDark) with airline statusline.
- **🐚 Seamless Git integration** – fugitive.vim shows diffs, blame, and commits.
- **⚡ Blazing fast startup** – all plugins are lazy‑loaded where possible.
- **🖥️ Cross‑platform** – works on Linux, macOS, and Windows (WSL).


## 📦 One‑command installation

```bash
git clone https://github.com/PsymoNiko/awesome-vim.git
cd awesome-vim
chmod +x install.sh
./install.sh
```

The install.sh script will:

· Backup your existing ~/.vimrc and ~/.vim
· Install vim-plug and all plugins
· Install system dependencies (curl, git, fzf, ripgrep, etc.) using your native package manager (apt, dnf, pacman, zypper, brew)
· Set everything up – no manual steps required

Note: After installation, restart Vim (or run :PlugInstall) if needed – the script does this automatically.

🗺️ Keymaps cheat sheet

Mode Shortcut Action
Normal <Leader>ff Fuzzy find files
Normal <Leader>fg Live grep (ripgrep)
Normal <Leader>fb List open buffers
Normal <Leader>fh Search command history
Normal <Leader>e Toggle file explorer (NERDTree)
Normal gd Go to definition (LSP)
Normal K Show hover documentation
Normal gr Show references
Normal [d / ]d Go to previous / next diagnostic
Normal <Leader>ca Code action (fix / refactor)
Insert <C-n> / <C-p> Autocomplete suggestions
Visual J / K Move selected lines up/down
Normal <Leader>gs Git status (fugitive)
Normal <Leader>gc Git commit
Normal <Leader>gp Git push

<Leader> is set to \ (backslash) by default. You can change it in ~/.vimrc.

🧩 Included plugins (selected)

Plugin Description
vim-plug Minimalist plugin manager
coc.nvim LSP client & autocompletion engine
fzf.vim Fuzzy finder integration
NERDTree File explorer
vim-fugitive Git wrapper
vim-airline Lean statusline
gruvbox / onedark.vim Colorschemes
vim-commentary Easy commenting
vim-surround Manage brackets, quotes, tags

See the full list in vim_folder/plugins.vim or directly in your .vimrc after installation.

🛠️ Customisation

All configuration files live in ~/.vim/:

· ~/.vimrc – main entry point (symlinked from vim_folder/vimrc)
· ~/.vim/plugins.vim – plugin list and settings
· ~/.vim/coc-settings.json – LSP language server configs
· ~/.vim/after/ – filetype‑specific overrides

To tweak anything, simply edit these files and restart Vim – or source them with :source %.

🤝 Contributing

Found a bug? Have a cool idea? Open an issue or submit a pull request. All contributions are welcome – from typo fixes to new plugin suggestions.

📄 License

MIT – do whatever you want, just keep the credits.

---

Maintained with ❤️ by @PsymoNiko
If this config saved you time, consider giving it a ⭐ on GitHub!
