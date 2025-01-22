# NeoTerm

This simple project allows you to use NeoVide
as a traditional terminal emulator.

It works by running NeoVide with specific instructions to execute
a lua configuration that opens a terminal window
directly instead of your typical neovim config.

## Prerequisites

The following prerequisites are required for this project to work:

- [Neovim](https://neovim.io/)
- [NeoVide](https://neovide.dev/)

This should work on any OS/platform that can run both Neovim and NeoVide as it
simply uses a basic neovim configuration to direct neovide's behavior.

## Installation

Clone this repository to your local machine:

```bash
git clone https://github.com/rootiest/neoterm ~/.config/neoterm
```

## Configuration

The default configuration should work out of the box.
You can add/change it by editing the [neoterm.lua](neoterm.lua) file.

## Usage

Start Neovide in NeoTerm mode by running:

```bash
neovide -- -u ~/.config/neoterm/neoterm.lua
```

## Shortcuts

You can create a shortcut to make executing this command easier.

In Linux GUIs you can run the following:

```bash
ln -s ~/.config/neoterm/NeoTerm.desktop ~/.local/share/applications/NeoTerm.desktop
```

The desktop file can be found here: [NeoTerm.desktop](NeoTerm.desktop)

This will add an entry to your application menu that you can click to
open the terminal emulator with NeoVide.

Or to create an alias in your shell:

```bash
alias neoterm="neovide -- -u '~/.config/neoterm/neoterm.lua'"
```

This allows you to run `neoterm` from the command line to open
the terminal emulator.

On other platforms you can use the traditional methods to create
a shortcut to run:  
`neovide -- -u '~/.config/neoterm/neoterm.lua'`

## Extras

[Rootiest Iosevka Font](https://github.com/rootiest/rootiest-iosevka) -
A custom Iosevka font that is designed by developers, for developers.

## Thanks

Special thanks to Reddit user d3bug64 who wrote the original
structure that I used as a basis for this project.

## 🛠️ Contributing

If you find any issues or have suggestions for improvement,
feel free to open a GitHub issue or send a pull request.
We welcome contributions!

### 🐛 Filing an Issue

Be sure to include the following information when reporting bugs:

1. The output of `nvim --version`.
2. Error messages from Neovim or NeoVide (if any).
3. Steps to reproduce the issue.

### 🚀 PR Submission Guidelines

1. Fork the repository.
2. Create a new branch for your feature or fix.
3. Make your changes, add or update tests, and confirm everything works.
4. Submit a **pull request** with a clear description of the changes made.

## License

This repository is licensed under the [MIT License](LICENSE).  
You are free to use, modify, and distribute this project in your own work.
