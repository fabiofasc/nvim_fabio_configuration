# Neovim Configuration

This repository contains a custom Neovim configuration that integrates several powerful plugins, including LazyVim, Telescope, LSP Zero, inc-rename, Primeagen's refactoring plugin, and Treesitter. This setup is designed for efficient code navigation, refactoring, and enhanced development workflow in Neovim.

## Features

- **LazyVim**: A modular and fast setup for Neovim, designed to easily manage plugin configurations.
- **Telescope**: Fuzzy finder for searching files, content, and more.
- **LSP Zero**: A simplified way to configure Neovim's built-in Language Server Protocol (LSP) support.
- **inc-rename**: Interactive renaming for LSP, allowing you to see the rename changes live.
- **Refactoring (ThePrimeagen)**: Advanced refactoring tools to quickly refactor code in multiple languages.
- **Treesitter**: Syntax highlighting and code parsing for improved performance and development experience.

## Requirements

- **Neovim** 0.9 or later

## Installation

1. Clone this repository into your Neovim configuration directory and start nvim

## Key Features and Usage

LazyVim

LazyVim provides a modular approach to managing plugins and Neovim configuration. It allows for easier plugin management and customization. By default, this configuration comes with several productivity plugins and settings already enabled.
Telescope

Telescope is used for fuzzy finding and searching through your project files, buffers, and other content. The following are the primary commands to use:

    <leader>ff: Fuzzy find files in the project.
    <leader>fg: Live grep through files.
    <leader>fb: Find buffers.
    <leader>fh: Find help documents.

LSP Zero

LSP Zero simplifies the configuration of Neovim's LSP functionality. You get built-in autocompletion, go-to-definition, diagnostics, and more.

Common LSP commands:

    gd: Go to definition.
    gr: Go to references.
    K: Show hover documentation.
    <leader>rn: Rename symbol (with inc-rename support).
    <leader>ca: Code actions.

inc-rename

This plugin allows live preview of renaming symbols across the project. The default keybinding is:

    <leader>rn: Start renaming the symbol under the cursor and see the changes in real-time.

Primeagen's Refactoring Plugin

This plugin offers advanced refactoring options for various programming languages. You can refactor your code easily with a set of commands:

    <leader>re: Extract function from the selected code.
    <leader>rv: Extract variable.
    <leader>ri: Inline a variable.

Treesitter

Treesitter provides better syntax highlighting and code parsing for Neovim, improving the overall development experience. It is automatically set up to handle various programming languages in this configuration.

:TSUpdate

Customization

You can modify the configuration further by editing the files in the lua directory. Here are some common configuration files:

    lua/plugins.lua: Manage installed plugins.
    lua/lsp.lua: Configure LSP-related settings.
    lua/telescope.lua: Configure Telescope settings.

Troubleshooting

If you encounter any issues, you can try the following steps:

    Sync Plugins: Run :Lazy sync to ensure all plugins are installed and up-to-date.
    Check Logs: Errors or warnings are often logged in :messages or inside ~/.config/nvim/lazy-lock.json.
    Help: Use :help <plugin-name> to access Neovim's built-in help for any plugin or feature.
