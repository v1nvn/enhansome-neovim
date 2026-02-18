# Awesome Neovim [![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re) with stars

<a href="https://neovim.io/"><img src="https://neovim.io/logos/neovim-mark-flat.png" align="right" width="144"/></a>

> A collection of awesome Neovim plugins. Mostly targeting Neovim specific features.
> This means Vim-compatible plugins are not listed here.

[Neovim](https://neovim.io/) is a Vim-based text editor engineered for extensibility and usability, to encourage new applications and contributions.
It has some [builtin plugins](https://neovim.io/doc/user/plugins.html#plugins) as well as a rich API for many more to be developed.

## Contents

* [Plugin Manager](#plugin-manager)
* [LSP](#lsp)
  * [LSP Installer](#lsp-installer)
  * [Diagnostics](#diagnostics)
* [Completion](#completion)
* [AI](#ai)
* [Programming Languages Support](#programming-languages-support)
  * [Golang](#golang)
  * [YAML](#yaml)
  * [Web Development](#web-development)
  * [Markdown and LaTeX](#markdown-and-latex)
  * [PHP](#php)
  * [Powershell](#powershell)
  * [Assembly](#assembly)
* [Language](#language)
* [Syntax](#syntax)
* [Snippet](#snippet)
* [Register](#register)
* [Marks](#marks)
* [Search](#search)
* [Fuzzy Finder](#fuzzy-finder)
* [File Explorer](#file-explorer)
* [Project](#project)
* [Buffers](#buffers)
* [Color](#color)
* [Colorscheme](#colorscheme)
  * [Colorscheme Creation](#colorscheme-creation)
  * [Colorscheme Switchers](#colorscheme-switchers)
* [Bars and Lines](#bars-and-lines)
  * [Statusline](#statusline)
  * [Tabline](#tabline)
  * [Cursorline](#cursorline)
* [Startup](#startup)
* [Icon](#icon)
* [Media](#media)
* [Note Taking](#note-taking)
* [Utility](#utility)
  * [CSV Files](#csv-files)
* [Animation](#animation)
* [Terminal Integration](#terminal-integration)
* [Debugging](#debugging)
  * [Quickfix](#quickfix)
* [Deployment](#deployment)
* [Test](#test)
* [Code Runner](#code-runner)
* [Neovim Lua Development](#neovim-lua-development)
* [Fennel](#fennel)
* [Dependency Management](#dependency-management)
* [Git](#git)
  * [GitHub](#github)
  * [GitLab](#gitlab)
* [Motion](#motion)
  * [Tree-sitter Based](#tree-sitter-based)
* [Keybinding](#keybinding)
* [Mouse](#mouse)
* [Scrolling](#scrolling)
  * [Scrollbar](#scrollbar)
* [Editing Support](#editing-support)
  * [Comment](#comment)
  * [Folding](#folding)
* [Formatting](#formatting)
  * [Indent](#indent)
* [Command Line](#command-line)
* [Session](#session)
* [Remote Development](#remote-development)
* [Live Preview](#live-preview)
* [Split and Window](#split-and-window)
  * [Tmux](#tmux)
* [Game](#game)
  * [Competitive Programming](#competitive-programming)
* [Workflow](#workflow)
  * [Stats Tracking](#stats-tracking)
  * [Automation](#automation)
* [Database](#database)
* [Preconfigured Configuration](#preconfigured-configuration)
* [External](#external)
  * [Version Manager](#version-manager)
  * [Plugin Template](#plugin-template)
  * [OS-specific](#os-specific)
* [Wishlist](#wishlist)
* [UI](#ui)
* [Starter Templates](#starter-templates)
* [Vim](#vim)
* [Resource](#resource)

## Plugin Manager

* [savq/paq-nvim](https://github.com/savq/paq-nvim) ⭐ 713 | 🐛 5 | 🌐 Lua | 📅 2025-03-30 - Package manager written in Lua.
* [lewis6991/pckr.nvim](https://github.com/lewis6991/pckr.nvim) ⭐ 342 | 🐛 8 | 🌐 Lua | 📅 2025-09-25 - Spiritual successor of `wbthomason/packer.nvim`.

<!--lint disable double-link -->

* [NTBBloodbath/cheovim](https://github.com/NTBBloodbath/cheovim) ⭐ 343 | 🐛 8 | 🌐 Lua | 📅 2023-08-01 - A configuration switcher written in Lua. Inspired by [chemacs](https://github.com/plexus/chemacs) ⭐ 660 | 🐛 12 | 🌐 Emacs Lisp | 📅 2021-01-04.

<!--lint enable double-link -->

* [folke/lazy.nvim](https://github.com/folke/lazy.nvim) ⭐ 20,284 | 🐛 50 | 🌐 Lua | 📅 2025-12-17 - A modern plugin manager, featuring a graphical interface, async execution, a lockfile and more.
  * [cosmicbuffalo/super\_lazy.nvim](https://github.com/cosmicbuffalo/super_lazy.nvim) ⭐ 2 | 🐛 0 | 🌐 Lua | 📅 2026-02-09 - An extension to `folke`'s `lazy.nvim`, enables use of multiple lockfiles for large teams that want to combine shared/personal Neovim configurations.
* [nvim-mini/mini.nvim#mini.deps](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-deps.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` for managing other plugins. Uses Git and built-in packages to install, update, clean, and snapshot plugins.
* [lumen-oss/rocks.nvim](https://github.com/lumen-oss/rocks.nvim) ⭐ 1,007 | 🐛 55 | 🌐 Lua | 📅 2026-02-08 - A modern approach to plugin management using Luarocks, inspired by Cargo.
* [alex-popov-tech/store.nvim](https://github.com/alex-popov-tech/store.nvim) ⭐ 318 | 🐛 0 | 🌐 Lua | 📅 2026-02-03 - Plugins discovery tool with hourly updated database, and one-key installation for `lazy.nvim` and `vim.pack`.
* [zuqini/zpack.nvim](https://github.com/zuqini/zpack.nvim) ⭐ 69 | 🐛 0 | 🌐 Lua | 📅 2026-01-15 - A thin layer on top of `vim.pack` to support lazy-loading and `lazy.nvim`'s declarative spec.
* [wsdjeg/nvim-plug](https://github.com/wsdjeg/nvim-plug) ⭐ 30 | 🐛 3 | 🌐 Lua | 📅 2026-02-18 - Asynchronous plugin manager written in Lua.
* [piersolenski/plugin-addict.nvim](https://github.com/piersolenski/plugin-addict.nvim) ⭐ 12 | 🐛 0 | 🌐 Lua | 📅 2025-11-03 - A stupidly simple way to quickly install plugins.
* [OriginCoderPulse/synapse.nvim](https://github.com/OriginCoderPulse/synapse.nvim) ⭐ 4 | 🐛 0 | 🌐 Lua | 📅 2025-12-09 - A modern, lightweight plugin manager with beautiful UI, intelligent dependency management, tag/branch support, and post-install command execution.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## LSP

**(requires Neovim 0.5)**

* [Dan7h3x/signup.nvim](https://github.com/Dan7h3x/signup.nvim) ⭐ 61 | 🐛 0 | 🌐 Lua | 📅 2026-01-27 - a little smart `lsp_signature` helper with awesome features.
* [romus204/referencer.nvim](https://github.com/romus204/referencer.nvim) ⭐ 33 | 🐛 1 | 🌐 Lua | 📅 2025-11-19 - Lightweight, asynchronous that uses the LSP to show references to functions, methods, types and other.

<!--lint disable awesome-spell-check-->

* [neovim/nvim-lspconfig](https://github.com/neovim/nvim-lspconfig) ⭐ 13,361 | 🐛 34 | 🌐 Lua | 📅 2026-02-12 - Quickstart configurations for the LSP client.

<!--lint enable awesome-spell-check-->

* [nvimdev/lspsaga.nvim](https://github.com/nvimdev/lspsaga.nvim) ⭐ 3,747 | 🐛 99 | 🌐 Lua | 📅 2025-06-25 - A light-weight LSP plugin based on the built-in LSP with a highly performant UI.
* [mfussenegger/nvim-lint](https://github.com/mfussenegger/nvim-lint) ⭐ 2,648 | 🐛 44 | 🌐 Lua | 📅 2026-02-16 - An asynchronous linter plugin, complementary to the built-in Language Server Protocol support.
* [j-hui/fidget.nvim](https://github.com/j-hui/fidget.nvim) ⭐ 2,478 | 🐛 19 | 🌐 Lua | 📅 2026-01-13 - Standalone UI for LSP progress.
* [ray-x/lsp\_signature.nvim](https://github.com/ray-x/lsp_signature.nvim) ⭐ 2,328 | 🐛 90 | 🌐 Lua | 📅 2026-01-28 - LSP signature hint when you type.
* [stevearc/aerial.nvim](https://github.com/stevearc/aerial.nvim) ⭐ 2,222 | 🐛 74 | 🌐 Lua | 📅 2026-01-18 - A code outline window for skimming and quick navigation.
* [onsails/lspkind.nvim](https://github.com/onsails/lspkind.nvim) ⭐ 1,662 | 🐛 15 | 🌐 Lua | 📅 2026-01-29 - The plugin adds VSCode-like icons to LSP completions.
* [ray-x/navigator.lua](https://github.com/ray-x/navigator.lua) ⭐ 1,386 | 🐛 23 | 🌐 Lua | 📅 2025-11-10 - Learn existing code quickly and navigate code like a breeze. A swiss army knife makes exploring LSP and Tree-sitter symbols a piece of cake.
* [rmagatti/goto-preview](https://github.com/rmagatti/goto-preview) ⭐ 1,022 | 🐛 10 | 🌐 Lua | 📅 2025-12-26 - Previewing native LSP's goto definition calls in floating windows.
* [b0o/SchemaStore.nvim](https://github.com/b0o/SchemaStore.nvim) ⭐ 972 | 🐛 11 | 🌐 Lua | 📅 2026-02-17 - Provide access to the [SchemaStore](https://github.com/SchemaStore/schemastore) ⭐ 3,646 | 🐛 101 | 🌐 JavaScript | 📅 2026-02-17 catalog.
* [hedyhli/outline.nvim](https://github.com/hedyhli/outline.nvim) ⭐ 956 | 🐛 31 | 🌐 Lua | 📅 2026-01-31 - A significantly enhanced and refactored fork of `symbols-outline.nvim`.
* [SmiteshP/nvim-navbuddy](https://github.com/SmiteshP/nvim-navbuddy) ⭐ 881 | 🐛 32 | 🌐 Lua | 📅 2025-05-01 - A simple popup display that provides breadcrumbs like navigation features using LSP.
* [kosayoda/nvim-lightbulb](https://github.com/kosayoda/nvim-lightbulb) ⭐ 872 | 🐛 8 | 🌐 Lua | 📅 2025-03-29 - The plugin shows a lightbulb in the sign column whenever a `textDocument/codeAction` is available at the current cursor position.
* [smjonas/inc-rename.nvim](https://github.com/smjonas/inc-rename.nvim) ⭐ 823 | 🐛 8 | 🌐 Lua | 📅 2026-02-15 - Provides an incremental LSP rename command based on the command-preview feature.
* [nvim-lua/lsp-status.nvim](https://github.com/nvim-lua/lsp-status.nvim) ⭐ 658 | 🐛 26 | 🌐 Lua | 📅 2022-08-31 - This is a plugin/library for generating statusline components from the built-in LSP client.
* [aznhe21/actions-preview.nvim](https://github.com/aznhe21/actions-preview.nvim) ⭐ 504 | 🐛 11 | 🌐 Lua | 📅 2025-10-03 - Fully customizable previewer for LSP code actions.
* [jubnzv/virtual-types.nvim](https://github.com/jubnzv/virtual-types.nvim) ⭐ 414 | 🐛 2 | 🌐 Lua | 📅 2023-04-07 - Show type annotations as virtual text.
* [ojroques/nvim-lspfuzzy](https://github.com/ojroques/nvim-lspfuzzy) ⭐ 342 | 🐛 0 | 🌐 Lua | 📅 2025-08-17 - A small plugin to make the LSP client use FZF.
* [tamago324/nlsp-settings.nvim](https://github.com/tamago324/nlsp-settings.nvim) ⭐ 336 | 🐛 10 | 🌐 Lua | 📅 2026-02-17 - Setup LSP with JSON or YAML files.
* [gfanto/fzf-lsp.nvim](https://github.com/gfanto/fzf-lsp.nvim) ⭐ 240 | 🐛 12 | 🌐 Lua | 📅 2024-08-07 - Enable the power of FZF fuzzy search for the built-in LSP.
* [marilari88/twoslash-queries.nvim](https://github.com/marilari88/twoslash-queries.nvim) ⭐ 170 | 🐛 3 | 🌐 Lua | 📅 2025-09-26 - Provide inline virtual text displaying TypeScript types for the inspected variables.
* [jakewvincent/texmagic.nvim](https://github.com/jakewvincent/texmagic.nvim) ⭐ 57 | 🐛 4 | 🌐 Lua | 📅 2024-02-23 - Enhance the lspconfig settings for Texlab by defining any number of custom LaTeX build engines and selecting them with magic comments.

<!--lint disable double-link-->

* [scalameta/nvim-metals](https://github.com/scalameta/nvim-metals) ⭐ 547 | 🐛 22 | 🌐 Lua | 📅 2026-01-16 - Provides a better experience while using [Metals](https://scalameta.org/metals/), the Scala Language Server, using the built-in LSP support.

<!--lint enable double-link-->

* [nvimtools/none-ls.nvim](https://github.com/nvimtools/none-ls.nvim) ⭐ 3,215 | 🐛 8 | 🌐 Lua | 📅 2026-02-16 - Null-ls.nvim reloaded / Use Neovim as a language server to inject LSP diagnostics, code actions, and more via Lua.
* [mrcjkb/rustaceanvim](https://github.com/mrcjkb/rustaceanvim) ⭐ 2,837 | 🐛 18 | 🌐 Lua | 📅 2026-02-16 - A heavily modified fork of rust-tools.nvim that does not require a `setup` call and does not depend on nvim-lspconfig.
* [rachartier/tiny-inline-diagnostic.nvim](https://github.com/rachartier/tiny-inline-diagnostic.nvim) ⭐ 1,571 | 🐛 0 | 🌐 Lua | 📅 2026-01-17 - Display prettier diagnostic messages. Display one line diagnostic messages where the cursor is, with icons and colors.
* [mfussenegger/nvim-jdtls](https://github.com/mfussenegger/nvim-jdtls) ⭐ 1,437 | 🐛 1 | 🌐 Lua | 📅 2026-02-10 - Extensions for the built-in LSP support for the Eclipse JDT Language Server.
* [DNLHC/glance.nvim](https://github.com/DNLHC/glance.nvim) ⭐ 863 | 🐛 17 | 🌐 Lua | 📅 2025-06-16 - A pretty window for previewing, navigating and editing your LSP locations.
* [jmbuhr/otter.nvim](https://github.com/jmbuhr/otter.nvim) ⭐ 837 | 🐛 16 | 🌐 Lua | 📅 2026-02-14 - Provides LSP features and a nvim-cmp completion source for languages embedded in other documents.
* [mrcjkb/haskell-tools.nvim](https://github.com/mrcjkb/haskell-tools.nvim) ⭐ 571 | 🐛 22 | 🌐 Lua | 📅 2026-02-15 - Seamless integration for Haskell development tools like `haskell-language-server` and Hoogle.
* [p00f/clangd\_extensions.nvim](https://github.com/p00f/clangd_extensions.nvim) ⭐ 571 | 🐛 8 | 🌐 Lua | 📅 2026-01-13 - Off-spec `clangd` features for the built-in LSP client.
* [zeioth/garbage-day.nvim](https://github.com/Zeioth/garbage-day.nvim) ⭐ 493 | 🐛 4 | 🌐 Lua | 📅 2025-09-16 - Garbage collector that stops inactive LSP clients to free RAM.
* [Wansmer/symbol-usage.nvim](https://github.com/Wansmer/symbol-usage.nvim) ⭐ 474 | 🐛 3 | 🌐 Lua | 📅 2025-05-03 - Display references, definitions and implementations of document symbols.
* [rachartier/tiny-code-action.nvim](https://github.com/rachartier/tiny-code-action.nvim) ⭐ 446 | 🐛 0 | 🌐 Lua | 📅 2026-02-13 - Provides a simple way to run and visualize code actions with Telescope.
* [soulis-1256/eagle.nvim](https://github.com/soulis-1256/eagle.nvim) ⭐ 343 | 🐛 0 | 🌐 Lua | 📅 2026-02-09 - Mouse-hover LSP hints.
* [VidocqH/lsp-lens.nvim](https://github.com/VidocqH/lsp-lens.nvim) ⭐ 307 | 🐛 20 | 🌐 Lua | 📅 2024-08-09 - Display function references above function definition like IDEA codelens.
* [creativenull/efmls-configs-nvim](https://github.com/creativenull/efmls-configs-nvim) ⭐ 305 | 🐛 1 | 🌐 Lua | 📅 2026-01-13 - An unofficial collection of linters and formatters configured for efm-langserver to work with built-in LSP.
* [jinzhongjia/LspUI.nvim](https://github.com/jinzhongjia/LspUI.nvim) ⭐ 275 | 🐛 1 | 🌐 Lua | 📅 2026-02-16 - A modern and useful UI that wraps LSP operations.
* [Fildo7525/pretty\_hover](https://github.com/Fildo7525/pretty_hover) ⭐ 240 | 🐛 2 | 🌐 Lua | 📅 2026-01-11 - Highly customizable hover formatter, extendable to blink.cmp. As native hover supports multiple LSP servers.
* [junnplus/lsp-setup.nvim](https://github.com/junnplus/lsp-setup.nvim) ⭐ 236 | 🐛 1 | 🌐 Lua | 📅 2025-05-15 - A simple wrapper for `nvim-lspconfig` and `mason-lspconfig` to easily setup LSP servers.
* [linrongbin16/lsp-progress.nvim](https://github.com/linrongbin16/lsp-progress.nvim) ⭐ 234 | 🐛 0 | 🌐 Lua | 📅 2026-02-02 - A performant LSP progress status.
* [hinell/lsp-timeout.nvim](https://github.com/hinell/lsp-timeout.nvim) ⭐ 231 | 🐛 0 | 🌐 Lua | 📅 2025-04-04 - Automatically start/stop idle/unused LSP servers; keeps RAM usage low.
* [chrisgrieser/nvim-lsp-endhints](https://github.com/chrisgrieser/nvim-lsp-endhints) ⭐ 231 | 🐛 0 | 🌐 Lua | 📅 2026-02-06 - Display LSP inlay hints at the end of the line, rather than within the line.
* [barreiroleo/ltex\_extra.nvim](https://github.com/barreiroleo/ltex_extra.nvim) ⭐ 182 | 🐛 11 | 🌐 Lua | 📅 2025-11-01 - LTeX LSP extension providing external file handling (rules and dictionaries).
* [amrbashir/nvim-docs-view](https://github.com/amrbashir/nvim-docs-view) ⭐ 177 | 🐛 0 | 🌐 Lua | 📅 2025-08-12 - Display LSP hover documentation in a side panel.
* [alexpasmantier/pymple.nvim](https://github.com/alexpasmantier/pymple.nvim) ⭐ 143 | 🐛 4 | 🌐 Lua | 📅 2025-12-20 - Refactor Python imports on file move/rename.
* [vxpm/ferris.nvim](https://github.com/vxpm/ferris.nvim) ⭐ 120 | 🐛 1 | 🌐 Lua | 📅 2025-08-04 - Interact with Rust-Analyzer's LSP extensions.
* [creativenull/diagnosticls-configs-nvim](https://github.com/creativenull/diagnosticls-configs-nvim) ⭐ 92 | 🐛 2 | 🌐 Lua | 📅 2025-11-12 - An unofficial collection of linters and formatters configured for diagnostic-languageserver to work with built-in LSP.
* [lopi-py/luau-lsp.nvim](https://github.com/lopi-py/luau-lsp.nvim) ⭐ 88 | 🐛 0 | 🌐 Lua | 📅 2026-02-07 - A luau-lsp extension to improve your experience.
* [stevanmilic/nvim-lspimport](https://github.com/stevanmilic/nvim-lspimport) ⭐ 80 | 🐛 7 | 🌐 Lua | 📅 2024-07-20 - Automatically resolves imports for undefined terms. Useful with `pyright` language server.
* [yarospace/dev-tools.nvim](https://github.com/yarospace/dev-tools.nvim) ⭐ 80 | 🐛 0 | 🌐 Lua | 📅 2025-11-01 - In-process LSP server for custom code actions, enhanced actions picker, community actions library and a convenient interface to create your own actions.
* [ranjithshegde/ccls.nvim](https://github.com/ranjithshegde/ccls.nvim) ⭐ 77 | 🐛 4 | 🌐 Lua | 📅 2025-01-09 - Use off-spec extensions of ccls LSP and browse AST.
* [esmuellert/nvim-eslint](https://github.com/esmuellert/nvim-eslint) ⭐ 77 | 🐛 3 | 🌐 Python | 📅 2026-02-14 - Bundle VSCode ESLint language server and utilize the native LSP client to provide a all-in-one ESLint experience.
* [Kasama/nvim-custom-diagnostic-highlight](https://github.com/Kasama/nvim-custom-diagnostic-highlight) ⭐ 62 | 🐛 0 | 🌐 Lua | 📅 2023-05-09 - Inline diagnostics popup-highlight much like `coc-nvim` but based on `vim.diagnostic`.
* [mawkler/refjump.nvim](https://github.com/mawkler/refjump.nvim) ⭐ 57 | 🐛 2 | 🌐 Lua | 📅 2025-12-23 - Jump to next/previous LSP reference for item under cursor with `]r`/`[r`.
* [LukasPietzschmann/boo.nvim](https://github.com/LukasPietzschmann/boo.nvim) ⭐ 37 | 🐛 4 | 🌐 Lua | 📅 2024-06-27 - Quickly pop-up some LSP-powered information of the thing your cursor is on.
* [chrisgrieser/nvim-dr-lsp](https://github.com/chrisgrieser/nvim-dr-lsp) ⚠️ Archived - Status line component showing the number of LSP definition and reference of the token under the cursor.
* [chojs23/ts-bridge](https://github.com/chojs23/ts-bridge) ⭐ 31 | 🐛 0 | 🌐 Rust | 📅 2026-01-06 - TypeScript language server shim that bridges the built-in LSP client with `tsserver`.
* [zeioth/none-ls-autoload.nvim](https://github.com/zeioth/none-ls-autoload.nvim) ⭐ 26 | 🐛 0 | 🌐 Lua | 📅 2025-06-24 - Auto-load/Auto-unload none-ls sources installed with mason. It supports built-in sources and external sources.
* [SunnyTamang/neodoc.nvim](https://github.com/SunnyTamang/neodoc.nvim) ⭐ 12 | 🐛 1 | 🌐 Lua | 📅 2025-06-26 - DocString generator that helps writing function/classes docstrings in formats like `google`, `numpy`, `sphinx` with live preview.
* [idanarye/nvim-buffls](https://github.com/idanarye/nvim-buffls) ⭐ 11 | 🐛 1 | 🌐 Lua | 📅 2025-07-20 - Add LSP functionality to specific buffers.
* [akioweh/lsp-document-highlight.nvim](https://github.com/akioweh/lsp-document-highlight.nvim) ⭐ 6 | 🐛 0 | 🌐 Lua | 📅 2026-01-10 - Instantaneous LSP symbol reference highlighting under the cursor.

### LSP Installer

* [mason-org/mason.nvim](https://github.com/mason-org/mason.nvim) ⭐ 10,039 | 🐛 268 | 🌐 Lua | 📅 2026-01-07 - Portable package manager that runs everywhere Neovim runs. Easily install and manage LSP servers, DAP servers, linters, and formatters.

### Diagnostics

* [folke/trouble.nvim](https://github.com/folke/trouble.nvim) ⭐ 6,674 | 🐛 17 | 🌐 Lua | 📅 2025-10-31 - A pretty diagnostics list to help you solve all the trouble your code is causing.
* [piersolenski/wtf.nvim](https://github.com/piersolenski/wtf.nvim) ⭐ 579 | 🐛 1 | 🌐 Lua | 📅 2026-02-02 - AI powered diagnostic debugging, helps explain complex errors and offers custom tailored solutions.
* [artemave/workspace-diagnostics.nvim](https://github.com/artemave/workspace-diagnostics.nvim) ⭐ 242 | 🐛 2 | 🌐 Lua | 📅 2025-05-25 - Populate diagnostics for all projects files, not just the opened ones.
* [chrisgrieser/nvim-rulebook](https://github.com/chrisgrieser/nvim-rulebook) ⭐ 109 | 🐛 0 | 🌐 Lua | 📅 2026-02-06 - Add inline-comments to ignore rules, or lookup rule documentation online.
* [sontungexpt/better-diagnostic-virtual-text](https://github.com/sontungexpt/better-diagnostic-virtual-text) ⭐ 95 | 🐛 3 | 🌐 Lua | 📅 2024-07-27 - Enhances the display of virtual text for diagnostics. This function aims to provide a more user-friendly and informative presentation of diagnostic messages directly within the editor.
* [\~whynothugo/lsp\_lines.nvim](https://git.sr.ht/~whynothugo/lsp_lines.nvim) - Render diagnostics using virtual lines on top of the real line of code.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Completion

* [hrsh7th/nvim-cmp](https://github.com/hrsh7th/nvim-cmp) ⭐ 9,328 | 🐛 298 | 🌐 Lua | 📅 2026-01-23 - Completion engine written in Lua, successor of `nvim-compe`.
  * [hrsh7th/cmp-nvim-lsp](https://github.com/hrsh7th/cmp-nvim-lsp) ⭐ 1,489 | 🐛 29 | 🌐 Lua | 📅 2025-11-13 - `nvim-cmp` source for the built-in LSP client.
  * [saadparwaiz1/cmp\_luasnip](https://github.com/saadparwaiz1/cmp_luasnip) ⭐ 776 | 🐛 11 | 🌐 Lua | 📅 2024-11-04 - `nvim-cmp` source for `LuaSnip`.
  * [hrsh7th/cmp-path](https://github.com/hrsh7th/cmp-path) ⭐ 685 | 🐛 38 | 🌐 Lua | 📅 2025-07-30 - `nvim-cmp` source for filesystem paths.
  * [hrsh7th/cmp-nvim-lsp-signature-help](https://github.com/hrsh7th/cmp-nvim-lsp-signature-help) ⭐ 677 | 🐛 25 | 🌐 Lua | 📅 2025-11-14 - `nvim-cmp` source for displaying function signatures from an LSP client.
  * [hrsh7th/cmp-buffer](https://github.com/hrsh7th/cmp-buffer) ⭐ 667 | 🐛 37 | 🌐 Lua | 📅 2025-04-01 - `nvim-cmp` source for buffer words.
  * [hrsh7th/cmp-cmdline](https://github.com/hrsh7th/cmp-cmdline) ⭐ 613 | 🐛 66 | 🌐 Lua | 📅 2025-05-18 - `nvim-cmp` source for cmdline completion.
  * [petertriho/cmp-git](https://github.com/petertriho/cmp-git) ⭐ 416 | 🐛 12 | 🌐 Lua | 📅 2025-04-30 - `nvim-cmp` source for `git`.
  * [hrsh7th/cmp-nvim-lua](https://github.com/hrsh7th/cmp-nvim-lua) ⭐ 325 | 🐛 3 | 🌐 Lua | 📅 2025-11-14 - `nvim-cmp` source for the Neovim Lua API.
  * [lukas-reineke/cmp-under-comparator](https://github.com/lukas-reineke/cmp-under-comparator) ⭐ 189 | 🐛 0 | 🌐 Lua | 📅 2022-03-04 - `nvim-cmp` function for better sorting.
  * [SergioRibera/cmp-dotenv](https://github.com/SergioRibera/cmp-dotenv) ⭐ 92 | 🐛 3 | 🌐 Lua | 📅 2024-06-05 - `nvim-cmp` source for environment variables (from system and `.env` files).
* [nvim-mini/mini.nvim#mini.completion](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-completion.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` for asynchronous two-stage completion. Supports showing completion item info and independent function signature.
* [saghen/blink.cmp](https://github.com/saghen/blink.cmp) ⭐ 5,944 | 🐛 146 | 🌐 Lua | 📅 2026-02-16 - Really fast completion with LSP and snippet support, along with signature help, cmdline completion, and autobracket support (based on semantic tokens).
  * [saghen/blink.compat](https://github.com/saghen/blink.compat) ⭐ 212 | 🐛 3 | 🌐 Lua | 📅 2025-05-28 - Compatibility layer for using `nvim-cmp` sources on `blink.cmp`.
  * [mikavilpas/blink-ripgrep.nvim](https://github.com/mikavilpas/blink-ripgrep.nvim) ⭐ 111 | 🐛 3 | 🌐 Lua | 📅 2026-02-17 - `blink.cmp` source for `ripgrep` / `git grep`.
  * [Kasier-Yang/blink-cmp-avante](https://github.com/Kaiser-Yang/blink-cmp-avante) ⭐ 105 | 🐛 3 | 🌐 Lua | 📅 2025-07-24 - `blink-cmp` source for Avante.
  * [Kaiser-Yang/blink-cmp-git](https://github.com/Kaiser-Yang/blink-cmp-git) ⭐ 86 | 🐛 6 | 🌐 Lua | 📅 2025-10-09 - `blink.cmp` source for Git.
  * [moyiz/blink-emoji.nvim](https://github.com/moyiz/blink-emoji.nvim) ⭐ 70 | 🐛 1 | 🌐 Lua | 📅 2025-10-22 - `blink.cmp` source for GitHub Markdown emojis.
  * [xieyonn/blink-cmp-dat-word](https://github.com/xieyonn/blink-cmp-dat-word) ⭐ 33 | 🐛 0 | 🌐 Lua | 📅 2026-02-13 - `blink.cmp` source for dictionary.
  * [disrupted/blink-cmp-conventional-commits](https://github.com/disrupted/blink-cmp-conventional-commits) ⭐ 30 | 🐛 0 | 🌐 Lua | 📅 2026-02-04 - `blink.cmp` source for [Conventional Commits](https://www.conventionalcommits.org/).
  * [bydlw98/blink-cmp-env](https://github.com/bydlw98/blink-cmp-env) ⭐ 21 | 🐛 0 | 🌐 Lua | 📅 2025-09-13 - `blink.cmp` source for environment variables.
  * [erooke/blink-cmp-latex](https://github.com/erooke/blink-cmp-latex) ⭐ 11 | 🐛 1 | 🌐 Lua | 📅 2025-05-30 - `blink.cmp` source for LaTeX.
  * [mgalliou/blink-cmp-tmux](https://github.com/mgalliou/blink-cmp-tmux) ⭐ 10 | 🐛 0 | 🌐 Lua | 📅 2026-02-11 - `blink.cmp` source for [tmux](https://github.com/tmux/tmux) ⭐ 41,853 | 🐛 45 | 🌐 C | 📅 2026-02-17.
  * [krissen/blink-cmp-bibtex](https://github.com/krissen/blink-cmp-bibtex) ⭐ 9 | 🐛 0 | 🌐 Lua | 📅 2026-01-17 - `blink.cmp` source for BibTeX citation files.
  * [bydlw98/blink-cmp-sshconfig](https://github.com/bydlw98/blink-cmp-sshconfig) ⭐ 6 | 🐛 0 | 🌐 Python | 📅 2025-09-13 - `blink.cmp` source for `sshconfig` files.
* [zbirenbaum/copilot.lua](https://github.com/zbirenbaum/copilot.lua) ⭐ 3,961 | 🐛 32 | 🌐 Lua | 📅 2026-02-15 - Fully featured Lua replacement for [GitHub/copilot.vim](https://github.com/github/copilot.vim) ⭐ 11,360 | 🐛 48 | 🌐 Vim Script | 📅 2026-01-09.
* [ms-jpq/coq\_nvim](https://github.com/ms-jpq/coq_nvim) ⭐ 3,776 | 🐛 186 | 🌐 Python | 📅 2026-01-06 - Fast as FUCK completion. SQLite, concurrent scheduler, hundreds of hours of optimization.
* [brianaung/compl.nvim](https://github.com/brianaung/compl.nvim) ⭐ 48 | 🐛 0 | 🌐 Lua | 📅 2025-06-10 - A minimal and dependency-free auto-completion built on top of Vim's ins-completion mechanism.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## AI

* [yetone/avante.nvim](https://github.com/yetone/avante.nvim) ⭐ 17,378 | 🐛 71 | 🌐 Lua | 📅 2026-02-16 - Chat with your code as if you are in Cursor AI IDE.
* [olimorris/codecompanion.nvim](https://github.com/olimorris/codecompanion.nvim) ⭐ 6,153 | 🐛 23 | 🌐 Lua | 📅 2026-02-17 - Copilot Chat like experience, complete with inline assistant. Supports Anthropic, Gemini, Ollama and OpenAI.
* [jackMort/ChatGPT.nvim](https://github.com/jackMort/ChatGPT.nvim) ⭐ 4,014 | 🐛 112 | 🌐 Lua | 📅 2026-01-13 - Effortless Natural Language Generation with OpenAI's ChatGPT API.
* [CopilotC-Nvim/CopilotChat.nvim](https://github.com/CopilotC-Nvim/CopilotChat.nvim) ⭐ 3,557 | 🐛 19 | 🌐 Lua | 📅 2026-02-12 - A chat interface for GitHub Copilot that allows you to directly ask and receive answers to coding-related questions.
* [nickjvandyke/opencode.nvim](https://github.com/nickjvandyke/opencode.nvim) ⭐ 2,566 | 🐛 18 | 🌐 Lua | 📅 2026-02-17 - OpenCode AI assistant integration.
* [David-Kunz/gen.nvim](https://github.com/David-Kunz/gen.nvim) ⭐ 1,513 | 🐛 25 | 🌐 Lua | 📅 2025-05-03 - Generate text using LLMs (via Ollama) with customizable prompts.
* [Robitx/gp.nvim](https://github.com/Robitx/gp.nvim) ⭐ 1,304 | 🐛 70 | 🌐 Lua | 📅 2025-08-11 - ChatGPT like sessions and instructable text/code operations in your favorite editor.
* [Exafunction/windsurf.nvim](https://github.com/Exafunction/windsurf.nvim) ⭐ 1,251 | 🐛 116 | 🌐 Lua | 📅 2025-04-30 - Free, ultrafast Copilot alternative. Supports LSP and Tree-sitter.
* [milanglacier/minuet-ai.nvim](https://github.com/milanglacier/minuet-ai.nvim) ⭐ 1,014 | 🐛 14 | 🌐 Lua | 📅 2026-02-03 - Minuet offers code completion from LLM providers including OpenAI (compatible), Gemini, Claude, Ollama, Deepseek and more providers, with support for nvim-cmp, blink.cmp and virtual-text frontend.
* [Davidyz/VectorCode](https://github.com/davidyz/vectorcode) ⭐ 799 | 🐛 14 | 🌐 Python | 📅 2025-12-26 - Supercharge your LLM experience with repository-level RAG.
* [dense-analysis/neural](https://github.com/dense-analysis/neural) ⭐ 510 | 🐛 19 | 🌐 Vim Script | 📅 2025-07-22 - Integrate LLMs for generating code, interacting with chat bots, and more.
* [Kurama622/llm.nvim](https://github.com/Kurama622/llm.nvim) ⭐ 460 | 🐛 3 | 🌐 Lua | 📅 2026-02-16 - Free large language model (LLM) support, provides commands to interact with LLM.
* [dlants/magenta.nvim](https://github.com/dlants/magenta.nvim) ⭐ 425 | 🐛 29 | 🌐 TypeScript | 📅 2026-02-18 - Leverage coding assistants for chat and code generation. Provides tools for the AI/LLM agent to explore and edit your code, like Aider, Cursor and Windsurf.
* [gsuuon/model.nvim](https://github.com/gsuuon/model.nvim) ⭐ 396 | 🐛 14 | 🌐 Lua | 📅 2025-07-23 - Integrate LLMs via a prompt builder interface. Multi-providers including OpenAI (+ compatibles), `PaLM`, `Hugging Face`, and local engines like `llamacpp`.
* [GeorgesAlkhouri/nvim-aider](https://github.com/GeorgesAlkhouri/nvim-aider) ⭐ 370 | 🐛 5 | 🌐 Lua | 📅 2025-10-28 - Seamlessly integrate Aider for an AI-assisted coding experience.
* [azorng/goose.nvim](https://github.com/azorng/goose.nvim) ⭐ 304 | 🐛 4 | 🌐 Lua | 📅 2026-01-07 - Seamless integration with [goose](https://block.github.io/goose) - work with a powerful AI agent without leaving your editor.
* [jpmcb/nvim-llama](https://github.com/jpmcb/nvim-llama) ⭐ 275 | 🐛 9 | 🌐 Python | 📅 2025-03-09 - LLM (LLaMA 2 and `llama.cpp`) wrappers.
* [tzachar/cmp-ai](https://github.com/tzachar/cmp-ai) ⭐ 270 | 🐛 5 | 🌐 Lua | 📅 2026-02-08 - This is a general purpose AI source for nvim-cmp, easily adapted to any REST API supporting remote code completion.
* [milanglacier/yarepl.nvim#aider-extensions](https://github.com/milanglacier/yarepl.nvim/blob/main/extensions/README.md) ⭐ 247 | 🐛 2 | 🌐 Lua | 📅 2026-02-04 - Integration with [aider-chat](https://aider.chat), a TUI AI coding assistant.
* [kiddos/gemini.nvim](https://github.com/kiddos/gemini.nvim) ⭐ 243 | 🐛 9 | 🌐 Lua | 📅 2025-11-29 - Bindings to Google Gemini API.
* [carlos-algms/agentic.nvim](https://github.com/carlos-algms/agentic.nvim) ⭐ 206 | 🐛 12 | 🌐 Lua | 📅 2026-02-17 - Chat interface for AI ACP providers such as Claude, Gemini, Codex, OpenCode and Cursor.
* [mozanunal/sllm.nvim](https://github.com/mozanunal/sllm.nvim) ⭐ 106 | 🐛 11 | 🌐 Lua | 📅 2026-02-08 - In-editor chat powered by Simon Willison's LLM CLI: stream replies in a Markdown buffer, manage rich context (files, URLs, selections, diagnostics, shell outputs), switch models interactively, and even see token-usage stats.
* [Aaronik/GPTModels.nvim](https://github.com/Aaronik/GPTModels.nvim) ⭐ 73 | 🐛 1 | 🌐 Lua | 📅 2025-06-26 - GPTModels - a stable, clean, multi model, window based LLM AI tool.
* [CamdenClark/flyboy](https://github.com/CamdenClark/flyboy) ⭐ 46 | 🐛 1 | 🌐 Lua | 📅 2023-10-31 - Simple interaction with ChatGPT in a Markdown buffer. Supports GPT-4 and Azure OpenAI.
* [Flemma-Dev/flemma.nvim](https://github.com/Flemma-Dev/flemma.nvim) ⭐ 44 | 🐛 0 | 🌐 Lua | 📅 2026-02-17 - A first-class AI workspace.
* [you-n-g/simplegpt.nvim](https://github.com/you-n-g/simplegpt.nvim) ⭐ 32 | 🐛 1 | 🌐 Lua | 📅 2026-01-29 - Provide a simple yet flexible way to construct and send questions to ChatGPT.
* [3v0k4/exit.nvim](https://github.com/3v0k4/exit.nvim) ⭐ 18 | 🐛 3 | 🌐 Lua | 📅 2024-12-19 - Prompt LLMs (large language models) to write Vim commands.
* [k2589/LLuMinate.nvim](https://github.com/k2589/lluminate.nvim) ⭐ 17 | 🐛 0 | 🌐 Lua | 📅 2024-10-11 - Enrich context for LLM with LSP hover added to clipboard.
* [chatvim/chatvim.nvim](https://github.com/chatvim/chatvim.nvim) ⭐ 13 | 🐛 0 | 🌐 Lua | 📅 2025-10-02 - Chat with Markdown files using AI models from xAI, OpenAI and Anthropic.
* [ishiooon/codex.nvim](https://github.com/ishiooon/codex.nvim) ⭐ 13 | 🐛 0 | 🌐 Lua | 📅 2026-01-30 - Codex IDE integration, no API key required.
* [heilgar/nochat.nvim](https://github.com/heilgar/nochat.nvim) ⭐ 11 | 🐛 0 | 🌐 Lua | 📅 2025-03-13 - Cursor-like effortless natural language generation with multiple AI providers including Ollama, Anthropic (Claude), and ChatGPT.
* [blob42/codegpt-ng.nvim](https://github.com/blob42/codegpt-ng.nvim) ⭐ 9 | 🐛 0 | 🌐 Lua | 📅 2025-12-04 - Minimalist command based AI coding with a powerful template system. Supports Ollama, OpenAI and more.
* [julwrites/llm-nvim](https://github.com/julwrites/llm-nvim) ⭐ 8 | 🐛 4 | 🌐 Lua | 📅 2025-12-31 - Comprehensive integration with the [LLM](https://github.com/simonw/llm) ⭐ 11,162 | 🐛 557 | 🌐 Python | 📅 2026-02-07 tool.
* [3ZsForInsomnia/token-count.nvim](https://github.com/3ZsForInsomnia/token-count.nvim) ⭐ 8 | 🐛 0 | 🌐 Lua | 📅 2025-12-22 - Shows the token count for the current buffer, with integrations for Lualine and NeoTree.
* [3ZsForInsomnia/code-companion-picker](https://github.com/3ZsForInsomnia/code-companion-picker) ⭐ 7 | 🐛 1 | 🌐 Lua | 📅 2025-10-20 - Telescope and Snacks picker integrations for previewing CodeCompanion prompts.
* [nishu-murmu/cursor-inline](https://github.com/nishu-murmu/cursor-inline) ⭐ 6 | 🐛 0 | 🌐 Lua | 📅 2026-01-23 - Cursor-style inline AI editing. Select code, describe the change, and get an inline, highlighted edit you can accept or reject—similar to Cursor inline workflow.
* [3ZsForInsomnia/vs-code-companion](https://github.com/3ZsForInsomnia/vs-code-companion) ⭐ 5 | 🐛 3 | 🌐 Lua | 📅 2025-10-22 - Tool for importing VSCode's Markdown prompts into CodeCompanion.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Programming Languages Support

* [nvim-java/nvim-java](https://github.com/nvim-java/nvim-java) ⭐ 1,568 | 🐛 32 | 🌐 Lua | 📅 2026-02-05 - Everything you need for a painless Java experience.
* [nvim-flutter/flutter-tools.nvim](https://github.com/nvim-flutter/flutter-tools.nvim) ⭐ 1,347 | 🐛 31 | 🌐 Lua | 📅 2026-01-14 - Build Flutter and Dart applications using the native LSP.
* [chomosuke/typst-preview.nvim](https://github.com/chomosuke/typst-preview.nvim) ⭐ 834 | 🐛 14 | 🌐 Lua | 📅 2025-12-31 - Preview Typst documents in the browser, instant update on each keystroke, and cross jump between code and preview.
* [dmmulroy/tsc.nvim](https://github.com/dmmulroy/tsc.nvim) ⭐ 532 | 🐛 7 | 🌐 Lua | 📅 2026-01-14 - Asynchronous project-wide TypeScript type-checking using the TypeScript compiler (`tsc`) with results loaded into a quickfix list.
* [quarto-dev/quarto-nvim](https://github.com/quarto-dev/quarto-nvim) ⭐ 494 | 🐛 6 | 🌐 Lua | 📅 2026-01-29 - Tools for working with [Quarto](https://quarto.org/) documents.
* [Julian/lean.nvim](https://github.com/Julian/lean.nvim) ⭐ 476 | 🐛 32 | 🌐 Lua | 📅 2026-02-17 - Support for the [Lean Theorem Prover](https://leanprover.github.io/).
* [dmmulroy/ts-error-translator.nvim](https://github.com/dmmulroy/ts-error-translator.nvim) ⭐ 417 | 🐛 1 | 🌐 Lua | 📅 2026-01-03 - A port of Matt Pocock's `ts-error-translator` for VSCode for turning messy and confusing TypeScript errors into plain English.
* [gennaro-tedesco/nvim-jqx](https://github.com/gennaro-tedesco/nvim-jqx) ⭐ 330 | 🐛 2 | 🌐 Lua | 📅 2024-05-31 - Interactive interface for JSON files.
* [iabdelkareem/csharp.nvim](https://github.com/iabdelkareem/csharp.nvim) ⭐ 271 | 🐛 15 | 🌐 Lua | 📅 2024-08-25 - Enhances the development experience for .NET developers.
* [AckslD/swenv.nvim](https://github.com/AckslD/swenv.nvim) ⭐ 246 | 🐛 13 | 🌐 Lua | 📅 2025-02-09 - Tiny plugin to quickly switch Python virtual environments without restarting.
* [nanotee/sqls.nvim](https://github.com/nanotee/sqls.nvim) ⭐ 244 | 🐛 11 | 🌐 Lua | 📅 2025-09-02 - SQL database connection plugin + LSP client.
* [apyra/nvim-unity.nvim](https://github.com/apyra/nvim-unity) ⭐ 93 | 🐛 9 | 🌐 C# | 📅 2026-01-24 - Use Neovim as your default Unity editor with full LSP support via OmniSharp.
* [kiyoon/python-import.nvim](https://github.com/kiyoon/python-import.nvim) ⭐ 60 | 🐛 0 | 🌐 Python | 📅 2025-08-12 - Add Python import statements with Tree-sitter, LSP, and more.
* [niuiic/typst-preview.nvim](https://github.com/niuiic/typst-preview.nvim) ⭐ 48 | 🐛 1 | 🌐 Lua | 📅 2025-05-19 - Preview Typst documents, respond to file changes.
* [neolooong/whichpy.nvim](https://github.com/neolooong/whichpy.nvim) ⭐ 34 | 🐛 1 | 🌐 Lua | 📅 2026-02-04 - Switch Python interpreter without restarting LSP.
* [kiyoon/haskell-scope-highlighting.nvim](https://github.com/kiyoon/haskell-scope-highlighting.nvim) ⭐ 29 | 🐛 0 | 🌐 Lua | 📅 2025-12-20 - Haskell syntax highlighting which considers variable scopes. Inspired from "Context Coloring" by prof. Douglas Crockford.
* [brendalf/mix.nvim](https://github.com/brendalf/mix.nvim) ⭐ 28 | 🐛 0 | 🌐 Lua | 📅 2022-08-22 - Mix (from Elixir) wrapper plugin.
* [alessio-vivaldelli/java-creator-nvim](https://github.com/alessio-vivaldelli/java-creator-nvim) ⭐ 24 | 🐛 0 | 🌐 Lua | 📅 2026-02-07 - Interactive Java file creator with automatic package detection, supporting classes, interfaces, enums, records and abstract classes.
* [atomicptr/defold.nvim](https://github.com/atomicptr/defold.nvim) ⭐ 18 | 🐛 6 | 🌐 Rust | 📅 2026-02-04 - Batteries-included development environment for the Defold game engine.
* [onlyati/quadlet-lsp.nvim](https://github.com/onlyati/quadlet-lsp.nvim) ⭐ 12 | 🐛 0 | 🌐 Lua | 📅 2025-12-10 - Provides completion, hover and other language server features for Podman Quadlet files.
* [leblocks/hopcsharp.nvim](https://github.com/leblocks/hopcsharp.nvim) ⭐ 10 | 🐛 7 | 🌐 Lua | 📅 2026-02-14 - Provides LSP-less navigation and type-hierarchy information in C# repositories.
* [chuwy/ucm.nvim](https://github.com/chuwy/ucm.nvim) ⭐ 6 | 🐛 2 | 🌐 Lua | 📅 2023-08-23 - Navigating [Unison](https://unison-lang.org/) projects.

### Golang

* [ray-x/go.nvim](https://github.com/ray-x/go.nvim) ⭐ 2,601 | 🐛 97 | 🌐 Lua | 📅 2026-02-03 - Golang plugin based on LSP and Tree-sitter.
* [olexsmir/gopher.nvim](https://github.com/olexsmir/gopher.nvim/) ⭐ 415 | 🐛 7 | 🌐 Lua | 📅 2025-12-08 - Plugin for making Golang development easiest.
* [fredrikaverpil/godoc.nvim](https://github.com/fredrikaverpil/godoc.nvim) ⭐ 173 | 🐛 0 | 🌐 Lua | 📅 2025-12-19 - Fuzzy search Go packages/symbols and view docs.
* [crispgm/nvim-go](https://github.com/crispgm/nvim-go) ⭐ 153 | 🐛 3 | 🌐 Lua | 📅 2025-08-19 - A minimal implementation of Golang development plugin.
* [maxandron/goplements.nvim](https://github.com/maxandron/goplements.nvim) ⭐ 87 | 🐛 3 | 🌐 Lua | 📅 2025-12-15 - Visualize Go struct and interface implementations.
* [rafaelsq/nvim-goc.lua](https://github.com/rafaelsq/nvim-goc.lua) ⭐ 55 | 🐛 0 | 🌐 Lua | 📅 2025-11-14 - Highlight your buffer with Golang Code Coverage.
* [crusj/structrue-go.nvim](https://github.com/crusj/structrue-go.nvim) ⭐ 48 | 🐛 1 | 🌐 Lua | 📅 2022-09-29 - A better structured display of Golang symbols information.
* [crusj/hierarchy-tree-go.nvim](https://github.com/crusj/hierarchy-tree-go.nvim) ⭐ 35 | 🐛 1 | 🌐 Lua | 📅 2022-12-01 - Golang integration with `callHierarchy` UI tree.
* [Snikimonkd/cmp-go-pkgs](https://github.com/Snikimonkd/cmp-go-pkgs) ⭐ 31 | 🐛 3 | 🌐 Lua | 📅 2025-01-07 - Cmp source for Go packages names.
* [yanskun/gotests.nvim](https://github.com/yanskun/gotests.nvim) ⭐ 28 | 🐛 1 | 🌐 Lua | 📅 2024-07-11 - Make Go tests easy with [gotests](https://github.com/cweill/gotests) ⭐ 5,277 | 🐛 38 | 🌐 Go | 📅 2025-10-30.
* [romus204/go-tagger.nvim](https://github.com/romus204/go-tagger.nvim) ⭐ 19 | 🐛 0 | 🌐 Lua | 📅 2026-02-15 - A lightweight plugin to manage struct field tags in Go files.
* [Yu-Leo/gosigns.nvim](https://github.com/Yu-Leo/gosigns.nvim) ⭐ 4 | 🐛 0 | 🌐 Lua | 📅 2025-03-08 - Visualize some Go hints: struct, interface, and methods implementations; go comments.
* [Yu-Leo/cmp-go-pkgs](https://github.com/Yu-Leo/cmp-go-pkgs) ⭐ 4 | 🐛 0 | 🌐 Lua | 📅 2025-03-04 - Cmp source providing the names of Go packages to import.

### YAML

* [cuducos.me/yaml.nvim](https://tangled.org/cuducos.me/yaml.nvim) - Utils to work with YAML files.
* [mosheavni/yaml-companion.nvim](https://github.com/mosheavni/yaml-companion.nvim) ⭐ 10 | 🐛 1 | 🌐 Lua | 📅 2026-01-21 - Automatic schema detection and selection for YAML files with `yaml-language-server`, including built-in Kubernetes support.

### Web Development

* [rest-nvim/rest.nvim](https://github.com/rest-nvim/rest.nvim) ⭐ 2,003 | 🐛 44 | 🌐 Lua | 📅 2025-12-27 - A fast HTTP client written in Lua.
* [mistweaverco/kulala.nvim](https://github.com/mistweaverco/kulala.nvim) ⭐ 1,896 | 🐛 11 | 🌐 Lua | 📅 2026-02-11 - A minimal HTTP-client interface.
* [cjodo/convert.nvim](https://github.com/cjodo/convert.nvim) ⭐ 55 | 🐛 0 | 🌐 Lua | 📅 2026-01-16 - Helps with CSS unit conversions.
* [yelog/i18n.nvim](https://github.com/yelog/i18n.nvim) ⭐ 54 | 🐛 2 | 🌐 Lua | 📅 2026-01-25 - Internationalization (i18n) management with LSP support for `Vue`, `React`, `Java` and more.
* [lima1909/resty.nvim](https://github.com/lima1909/resty.nvim) ⭐ 52 | 🐛 3 | 🌐 Lua | 📅 2025-08-17 - Fast and easy-to-use HTTP-Rest-Client.
* [Kenzo-Wada/boundary.nvim](https://github.com/Kenzo-Wada/boundary.nvim) ⭐ 26 | 🐛 0 | 🌐 Lua | 📅 2025-10-28 - Display `'use client'` markers inline in your JSX code to visualize client component boundaries.
* [mawkler/jsx-element.nvim](https://github.com/mawkler/jsx-element.nvim) ⭐ 24 | 🐛 1 | 🌐 Lua | 📅 2025-03-14 - JSX/TSX text-objects and motions.
* [heilgar/nvim-http-client](https://github.com/heilgar/nvim-http-client) ⭐ 21 | 🐛 0 | 🌐 Lua | 📅 2025-10-06 - Easy to use HTTP client with IntelliJ (JetBrains) HTTP client syntax compatibility.
* [abidibo/nvim-httpyac](https://github.com/abidibo/nvim-httpyac) ⭐ 14 | 🐛 0 | 🌐 Lua | 📅 2026-01-20 - Provides integration with `httpYac`.
* [BibekBhusal0/nvim-shadcn](https://github.com/BibekBhusal0/nvim-shadcn) ⭐ 11 | 🐛 0 | 🌐 Lua | 📅 2026-02-14 - Easily add Shadcn UI components with telescope.
* [farias-hecdin/CSSVarViewer](https://github.com/farias-hecdin/CSSVarViewer) ⭐ 10 | 🐛 1 | 🌐 Lua | 📅 2024-10-01 - Easily visualize the content of your CSS variables in a virtual text.
* [rodrigoscc/nurl.nvim](https://github.com/rodrigoscc/nurl.nvim) ⭐ 9 | 🐛 0 | 🌐 Lua | 📅 2026-02-13 - HTTP client with requests defined in pure Lua.
* [farias-hecdin/CSSVarHighlight](https://github.com/farias-hecdin/CSSVarHighlight) ⭐ 6 | 🐛 0 | 🌐 Lua | 📅 2024-09-24 - Quickly highlight the color you defined in your CSS variables with the help of `mini.hipatterns`.
* [azratul/expose-localhost.nvim](https://github.com/azratul/expose-localhost.nvim) ⭐ 6 | 🐛 0 | 🌐 Lua | 📅 2025-03-28 - Expose your local server to the internet with cloudflared or ngrok.
* [tednguyendev/recent\_rails.nvim](https://github.com/tednguyendev/recent_rails.nvim) ⭐ 3 | 🐛 0 | 🌐 Lua | 📅 2026-01-18 - Telescope picker for recent Rails actions, views, and errors.

### Markdown and LaTeX

* [iamcco/markdown-preview.nvim](https://github.com/iamcco/markdown-preview.nvim) ⭐ 7,698 | 🐛 257 | 🌐 JavaScript | 📅 2024-07-23 - Preview Markdown on your modern browser with synchronised scrolling and flexible configuration.
* [MeanderingProgrammer/render-markdown.nvim](https://github.com/MeanderingProgrammer/render-markdown.nvim) ⭐ 4,131 | 🐛 8 | 🌐 Lua | 📅 2026-02-03 - Improve viewing Markdown files directly.
* [OXY2DEV/markview.nvim](https://github.com/OXY2DEV/markview.nvim) ⭐ 3,273 | 🐛 3 | 🌐 Lua | 📅 2026-02-02 - A hackable Markdown, Typst, LaTeX, HTML (inline) and YAML renderer.
* [toppair/peek.nvim](https://github.com/toppair/peek.nvim) ⭐ 837 | 🐛 37 | 🌐 TypeScript | 📅 2024-08-20 - Preview Markdown in a webview window.
* [frabjous/knap](https://github.com/frabjous/knap) ⭐ 380 | 🐛 8 | 🌐 Lua | 📅 2024-10-22 - Plugin for creating automatic updating-as-you-type previews for Markdown, LaTeX and other documents.
* [kdheepak/panvimdoc](https://github.com/kdheepak/panvimdoc) ⭐ 309 | 🐛 9 | 🌐 CSS | 📅 2025-09-26 - A pandoc to vimdoc GitHub action.
* [Zeioth/markmap.nvim](https://github.com/Zeioth/markmap.nvim) ⭐ 236 | 🐛 2 | 🌐 Lua | 📅 2025-11-11 - Visualize your Markdown as mindmaps.
* [tadmccorkle/markdown.nvim](https://github.com/tadmccorkle/markdown.nvim) ⭐ 228 | 🐛 8 | 🌐 Lua | 📅 2025-12-22 - Configurable tools for Markdown files, including inline-style, link, and navigation keymaps, table of contents, improved list editing, and more.
* [jubnzv/mdeval.nvim](https://github.com/jubnzv/mdeval.nvim) ⭐ 219 | 🐛 4 | 🌐 Lua | 📅 2024-11-30 - Evaluate code blocks inside Markdown documents.
* [Thiago4532/mdmath.nvim](https://github.com/Thiago4532/mdmath.nvim) ⭐ 204 | 🐛 13 | 🌐 Lua | 📅 2024-12-27 - A Markdown equation previewer, using Kitty Graphics Protocol.
* [YousefHadder/markdown-plus.nvim](https://github.com/YousefHadder/markdown-plus.nvim) ⭐ 189 | 🐛 9 | 🌐 Lua | 📅 2026-02-08 - Provides a full editing experience for Markdown files which includes support for lists, links, TOC, and more with simple and fast keymaps.
* [jghauser/follow-md-links.nvim](https://github.com/jghauser/follow-md-links.nvim) ⭐ 167 | 🐛 7 | 🌐 Lua | 📅 2025-09-01 - Press enter to follow internal Markdown links.
* [Myzel394/easytables.nvim](https://github.com/Myzel394/easytables.nvim) ⭐ 136 | 🐛 2 | 🌐 Lua | 📅 2025-11-02 - Easily insert and edit Markdown tables with a live preview and useful helpers.
* [nvim-telescope/telescope-bibtex.nvim](https://github.com/nvim-telescope/telescope-bibtex.nvim) ⭐ 132 | 🐛 16 | 🌐 Lua | 📅 2024-03-28 - Telescope extension to search and paste BibTeX entries into your TeX files.
* [davidgranstrom/nvim-markdown-preview](https://github.com/davidgranstrom/nvim-markdown-preview) ⭐ 111 | 🐛 11 | 🌐 CSS | 📅 2023-07-11 - Markdown preview in the browser using pandoc and live-server through the job-control API.
* [Kicamon/markdown-table-mode.nvim](https://github.com/Kicamon/markdown-table-mode.nvim) ⭐ 96 | 🐛 6 | 🌐 Lua | 📅 2025-07-13 - Markdown format plugin like vim-table-mode but write in Lua.
* [SCJangra/table-nvim](https://github.com/SCJangra/table-nvim) ⭐ 69 | 🐛 1 | 🌐 Lua | 📅 2025-11-24 - A Markdown table editor that formats the table as you type.
* [OXY2DEV/markdoc.nvim](https://github.com/OXY2DEV/markdoc.nvim) ⭐ 51 | 🐛 1 | 🌐 Lua | 📅 2025-11-14 - Tree-sitter based `markdown -> vimdoc` converter.
* [mpas/marp-nvim](https://github.com/mpas/marp-nvim) ⭐ 50 | 🐛 0 | 🌐 Lua | 📅 2024-07-31 - Present using Markdown with [Marp](https://marp.app/).
* [richardbizik/nvim-toc](https://github.com/richardbizik/nvim-toc) ⭐ 46 | 🐛 0 | 🌐 Lua | 📅 2026-01-06 - Easily generate table of contents for Markdown files.
* [jghauser/auto-pandoc.nvim](https://github.com/jghauser/auto-pandoc.nvim) ⭐ 40 | 🐛 1 | 🌐 Nix | 📅 2025-08-31 - Easy pandoc conversion leveraging YAML blocks.
* [yaocccc/nvim-hl-mdcodeblock.lua](https://github.com/yaocccc/nvim-hl-mdcodeblock.lua) ⭐ 34 | 🐛 0 | 🌐 Lua | 📅 2023-04-29 - Highlight Markdown codeblock using Tree-sitter.
* [Nedra1998/nvim-mdlink](https://github.com/Nedra1998/nvim-mdlink) ⭐ 32 | 🐛 1 | 🌐 Lua | 📅 2024-12-24 - Simplify creating and following Markdown links.
* [kiran94/edit-markdown-table.nvim](https://github.com/kiran94/edit-markdown-table.nvim) ⭐ 28 | 🐛 0 | 🌐 Lua | 📅 2023-05-28 - Edit Markdown Tables using Tree-sitter.
* [jbyuki/carrot.nvim](https://github.com/jbyuki/carrot.nvim) ⭐ 27 | 🐛 0 | 🌐 Lua | 📅 2025-06-01 - Markdown evaluator Lua code blocks.
* [Prgebish/sigil.nvim](https://github.com/Prgebish/sigil.nvim) ⭐ 27 | 🐛 0 | 🌐 Lua | 📅 2026-02-15 - Implementation of Emacs' `prettify-symbols-mode` to visually replace text patterns with Unicode symbols while editing LaTeX and Typst files.
* [nfrid/markdown-togglecheck](https://github.com/nfrid/markdown-togglecheck) ⭐ 23 | 🐛 1 | 🌐 Lua | 📅 2023-09-04 - Toggle task list check boxes using Tree-sitter.
* [ChuufMaster/markdown-toc](https://github.com/ChuufMaster/markdown-toc) ⭐ 17 | 🐛 1 | 🌐 Lua | 📅 2025-05-28 - Generate TOC in any Markdown file from any other Markdown file with customisable levels of headings and affordances for emojis and ensuring that it works on GitHub using relative paths.
* [timantipov/md-table-tidy.nvim](https://github.com/timantipov/md-table-tidy.nvim) ⭐ 15 | 🐛 1 | 🌐 Lua | 📅 2026-01-19 - Simple Markdown tables formatting.
* [tttol/md-outline.nvim](https://github.com/tttol/md-outline.nvim) ⭐ 4 | 🐛 3 | 🌐 Lua | 📅 2025-11-10 - Automatically displays an outline for Markdown files.
* [rogue-87/inlyne.nvim](https://github.com/rogue-87/inlyne.nvim) ⭐ 3 | 🐛 0 | 🌐 Lua | 📅 2026-02-05 - Wrapper for [inlyne](https://github.com/Inlyne-Project/inlyne) ⭐ 1,258 | 🐛 56 | 🌐 Rust | 📅 2025-12-19 Markdown viewer.

### PHP

* [gbprod/phpactor.nvim](https://github.com/gbprod/phpactor.nvim) ⭐ 93 | 🐛 2 | 🌐 Lua | 📅 2026-01-07 - Lua version of [phpactor](https://github.com/phpactor/phpactor) ⭐ 1,804 | 🐛 294 | 🌐 PHP | 📅 2026-01-29.
* [ta-tikoma/php.easy.nvim](https://github.com/ta-tikoma/php.easy.nvim) ⭐ 22 | 🐛 1 | 🌐 Lua | 📅 2025-12-04 - Methods of assistance in PHP development: create classes, constants, methods, properties; simple copying and deleting of an entity.

### Powershell

* [TheLeoP/powershell.nvim](https://github.com/TheLeoP/powershell.nvim) ⭐ 75 | 🐛 0 | 🌐 Lua | 📅 2026-01-23 - First class powershell editor integration. Includes LSP, debugging (requires nvim-dap) and $psEditor API support.

### Assembly

* [Who5673/who5673-nasm](https://github.com/Who5673/who5673-nasm) ⭐ 6 | 🐛 0 | 🌐 Lua | 📅 2026-01-05 - Helps people program Netwide Assembler language faster and more convenient using snippets.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Language

* [potamides/pantran.nvim](https://github.com/potamides/pantran.nvim) ⭐ 326 | 🐛 9 | 🌐 Lua | 📅 2025-04-07 - Translate your text with an interactive translation window.
* [niuiic/translate.nvim](https://github.com/niuiic/translate.nvim) ⭐ 42 | 🐛 0 | 🌐 Lua | 📅 2024-11-17 - Invoke any translation engine via shell command.
* [kiyoon/Korean-IME.nvim](https://github.com/kiyoon/Korean-IME.nvim) ⭐ 30 | 🐛 1 | 🌐 Lua | 📅 2026-01-28 - OS-independent Korean input method that converts English inputs to Korean in-place.
* [bennorichters/taal.nvim](https://github.com/bennorichters/taal.nvim) ⭐ 19 | 🐛 0 | 🌐 Lua | 📅 2026-02-12 - Improve grammar and spelling errors in multiple languages using LLMs.
* [sontungexpt/vietnamese.nvim](https://github.com/sontungexpt/vietnamese.nvim) ⭐ 15 | 🐛 0 | 🌐 Lua | 📅 2026-01-02 - A Vietnamese input method engine with native support to type Vietnamese in insert mode.
* [acidsugarx/babel.nvim](https://github.com/acidsugarx/babel.nvim) ⭐ 11 | 🐛 2 | 🌐 Lua | 📅 2025-12-07 - Translate text using Google Translate with async support, float display, and multi-picker integration.
* [tanloong/interlaced.nvim](https://github.com/tanloong/interlaced.nvim) ⭐ 10 | 🐛 0 | 🌐 Lua | 📅 2025-07-21 - Help align bilingual parallel texts.
* [noir4y/comment-translate.nvim](https://github.com/noir4y/comment-translate.nvim) ⭐ 8 | 🐛 0 | 🌐 Lua | 📅 2026-02-15 - Translate code comments and strings using online as well as local LLMs or external translators.
* [walkersumida/deepl.nvim](https://github.com/walkersumida/deepl.nvim) ⭐ 6 | 🐛 0 | 🌐 Lua | 📅 2025-11-22 - Translates text using the DeepL API with multiple output modes (float, replace, append).
* [doodleEsc/translator.nvim](https://github.com/doodleEsc/translator.nvim) ⭐ 5 | 🐛 0 | 🌐 Lua | 📅 2025-09-01 - A powerful AI-powered translation plugin, leveraging OpenAI's GPT models to provide high-quality translations with natural language understanding.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Syntax

* [nvim-treesitter/nvim-treesitter](https://github.com/nvim-treesitter/nvim-treesitter) ⭐ 13,268 | 🐛 267 | 🌐 Tree-sitter Query | 📅 2026-02-17 - Tree-sitter configurations and abstraction layer.
* [nvim-mini/mini.nvim#mini.surround](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-surround.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` for working with text surroundings (add, delete, replace, find, highlight). Supports dot-repeat, different search methods, "last"/"next" extended mappings, Tree-sitter integration, and more.
* [kylechui/nvim-surround](https://github.com/kylechui/nvim-surround) ⭐ 4,108 | 🐛 9 | 🌐 Lua | 📅 2025-12-14 - A plugin for adding/changing/deleting surrounding delimiter pairs.
* [nvim-treesitter/nvim-treesitter-textobjects](https://github.com/nvim-treesitter/nvim-treesitter-textobjects) ⭐ 2,673 | 🐛 110 | 🌐 Tree-sitter Query | 📅 2026-01-28 - Create your own textobjects using Tree-sitter queries.
* [RRethy/nvim-treesitter-textsubjects](https://github.com/RRethy/nvim-treesitter-textsubjects) ⭐ 564 | 🐛 6 | 🌐 Tree-sitter Query | 📅 2025-08-14 - Location and syntax aware text objects which *do what you mean*.
* [m-demare/hlargs.nvim](https://github.com/m-demare/hlargs.nvim) ⭐ 559 | 🐛 8 | 🌐 Lua | 📅 2025-09-23 - Highlight arguments' definitions and usages, using Tree-sitter.
* [IndianBoy42/tree-sitter-just](https://github.com/IndianBoy42/tree-sitter-just) ⭐ 180 | 🐛 4 | 🌐 Just | 📅 2026-02-09 - Tree-sitter grammar for [Justfiles](https://github.com/casey/just) ⭐ 31,383 | 🐛 386 | 🌐 Rust | 📅 2026-02-16.
* [LhKipp/nvim-nu](https://github.com/LhKipp/nvim-nu) ⭐ 159 | 🐛 4 | 🌐 Lua | 📅 2024-12-10 - Basic editor support for the nushell language.
* [fei6409/log-highlight.nvim](https://github.com/fei6409/log-highlight.nvim) ⭐ 151 | 🐛 0 | 🌐 Vim Script | 📅 2026-02-14 - Generic log syntax highlighting and log filetype management support.
* [MeanderingProgrammer/treesitter-modules.nvim](https://github.com/MeanderingProgrammer/treesitter-modules.nvim) ⭐ 149 | 🐛 0 | 🌐 Lua | 📅 2026-02-05 - Original modules from nvim-treesitter master branch.
* [calops/hmts.nvim](https://github.com/calops/hmts.nvim) ⭐ 90 | 🐛 13 | 🌐 Lua | 📅 2025-06-11 - Tree-sitter queries for Home Manager Nix files.
* [desdic/agrolens.nvim](https://github.com/desdic/agrolens.nvim) ⭐ 68 | 🐛 0 | 🌐 Lua | 📅 2026-01-04 - Navigate via Tree-sitter nodes using Telescope or FZF.
* [BibekBhusal0/tree-hierarchy.nvim](https://github.com/BibekBhusal0/tree-hierarchy.nvim) ⭐ 12 | 🐛 0 | 🌐 Lua | 📅 2026-01-10 - Edit text and nevigate based on Tree-sitter.
* [Hdoc1509/gh-actions.nvim](https://github.com/Hdoc1509/gh-actions.nvim) ⭐ 8 | 🐛 0 | 🌐 Lua | 📅 2025-12-16 - Tree-sitter grammar and LSP query configuration for GitHub Actions.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Snippet

* [nvim-mini/mini.nvim#mini.snippets](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-snippets.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` to manage and expand snippets. Supports LSP snippet syntax, flexible loaders, fuzzy prefix matching, interactive selection, snippet session with rich visualization, and more.
* [L3MON4D3/LuaSnip](https://github.com/L3MON4D3/LuaSnip) ⭐ 4,272 | 🐛 129 | 🌐 Lua | 📅 2026-01-19 - A snippet engine written in Lua.
* [rafamadriz/friendly-snippets](https://github.com/rafamadriz/friendly-snippets) ⭐ 2,649 | 🐛 66 | 🌐 Lua | 📅 2026-01-23 - Set of preconfigured snippets for different languages.
* [chrisgrieser/nvim-scissors](https://github.com/chrisgrieser/nvim-scissors) ⭐ 563 | 🐛 0 | 🌐 Lua | 📅 2026-02-06 - Automagical editing and creation of snippets.
* [dcampos/nvim-snippy](https://github.com/dcampos/nvim-snippy) ⭐ 340 | 🐛 8 | 🌐 Lua | 📅 2025-09-21 - Snippet plugin written in Lua with support for [vim-snippets](https://github.com/honza/vim-snippets) ⭐ 4,873 | 🐛 85 | 🌐 Vim Snippet | 📅 2025-10-28.
* [ellisonleao/carbon-now.nvim](https://github.com/ellisonleao/carbon-now.nvim) ⭐ 192 | 🐛 1 | 🌐 Lua | 📅 2025-11-05 - Create beautiful code snippets from the terminal.
* [smjonas/snippet-converter.nvim](https://github.com/smjonas/snippet-converter.nvim) ⭐ 182 | 🐛 6 | 🌐 Lua | 📅 2023-09-21 - Convert snippets between the most common snippet formats and modify them using a few lines of Lua code.
* [cvigilv/esqueleto.nvim](https://github.com/cvigilv/esqueleto.nvim) ⭐ 107 | 🐛 5 | 🌐 Lua | 📅 2025-07-09 - Simple templates to use when creating new files.
* [TobinPalmer/rayso.nvim](https://github.com/TobinPalmer/rayso.nvim) ⭐ 82 | 🐛 0 | 🌐 Lua | 📅 2025-11-15 - Create code snippets using [ray.so](https://ray.so).
* [mrcjkb/haskell-snippets.nvim](https://github.com/mrcjkb/haskell-snippets.nvim) ⭐ 33 | 🐛 5 | 🌐 Lua | 📅 2025-11-24 - Haskell snippets for LuaSnip, powered by Tree-sitter and LSP.
* [guilherme-puida/tesoura.nvim](https://github.com/guilherme-puida/tesoura.nvim) ⭐ 27 | 🐛 0 | 🌐 Lua | 📅 2024-06-04 - A flexible snippet system using the native snippet API.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Register

* [acksld/nvim-neoclip.lua](https://github.com/AckslD/nvim-neoclip.lua) ⭐ 1,119 | 🐛 28 | 🌐 Lua | 📅 2025-02-09 - Clipboard manager with telescope integration.
* [tversteeg/registers.nvim](https://github.com/tversteeg/registers.nvim) ⭐ 615 | 🐛 11 | 🌐 Lua | 📅 2025-11-20 - Non-obtrusive minimal preview of Vim registers.
* [gennaro-tedesco/nvim-peekup](https://github.com/gennaro-tedesco/nvim-peekup) ⭐ 328 | 🐛 1 | 🌐 Lua | 📅 2023-02-23 - Dynamically interact with Vim registers.
* [bfredl/nvim-miniyank](https://github.com/bfredl/nvim-miniyank) ⭐ 238 | 🐛 12 | 🌐 Lua | 📅 2023-11-06 - The killring-alike plugin with no default mappings.
* [tenxsoydev/karen-yank.nvim](https://github.com/tenxsoydev/karen-yank.nvim) ⭐ 91 | 🐛 1 | 🌐 Lua | 📅 2023-07-29 - More intentional register handling with delete, cut and yank mappings.
* [kr40/nvim-macros](https://github.com/kr40/nvim-macros) ⭐ 72 | 🐛 1 | 🌐 Lua | 📅 2024-02-16 - Easy way to save and load Macros, with backup and formatting options.
* [desdic/macrothis.nvim](https://github.com/desdic/macrothis.nvim) ⭐ 33 | 🐛 0 | 🌐 Lua | 📅 2025-02-12 - Save and load macros/registers.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Marks

* [ThePrimeagen/harpoon](https://github.com/ThePrimeagen/harpoon/tree/harpoon2) ⭐ 8,896 | 🐛 150 | 🌐 Lua | 📅 2025-10-31 - A per project, auto updating and editable marks utility for fast file navigation.
* [chentoast/marks.nvim](https://github.com/chentoast/marks.nvim) ⭐ 1,140 | 🐛 56 | 🌐 Lua | 📅 2025-05-13 - A better user experience for viewing and interacting with Vim marks.
* [otavioschwanck/arrow.nvim](https://github.com/otavioschwanck/arrow.nvim) ⭐ 726 | 🐛 34 | 🌐 Lua | 📅 2025-11-28 - Like harpoon, but with a different UX, single keybinding needed and statusline support.
* [cbochs/grapple.nvim](https://github.com/cbochs/grapple.nvim) ⭐ 686 | 🐛 24 | 🌐 Lua | 📅 2024-09-29 - Provides tagging, cursor tracking, and immediate navigation to important project files.
* [LintaoAmons/bookmarks.nvim](https://github.com/LintaoAmons/bookmarks.nvim) ⭐ 283 | 🐛 17 | 🌐 Lua | 📅 2025-10-24 - Your new bookmarks option: simple yet powerful.
* [LeonHeidelbach/trailblazer.nvim](https://github.com/LeonHeidelbach/trailblazer.nvim) ⭐ 281 | 🐛 4 | 🌐 Lua | 📅 2025-02-04 - TrailBlazer introduces a stack based mark system that enables a completely new dynamic and super fast workflow using project wide marks.
* [tomasky/bookmarks.nvim](https://github.com/tomasky/bookmarks.nvim) ⭐ 183 | 🐛 13 | 🌐 Lua | 📅 2024-06-18 - Bookmarks with global file storage, written in Lua.
* [EvWilson/spelunk.nvim](https://github.com/EvWilson/spelunk.nvim) ⭐ 146 | 🐛 0 | 🌐 Lua | 📅 2025-12-04 - Create and manage bookmarks as stacks with a friendly UI.
* [fnune/recall.nvim](https://github.com/fnune/recall.nvim) ⭐ 89 | 🐛 2 | 🌐 Lua | 📅 2025-12-16 - Recall refines the use of marks by focusing on global marks, streamlining their usage and enhancing their visibility and navigability.
* [ofirgall/open.nvim](https://github.com/ofirgall/open.nvim) ⭐ 69 | 🐛 1 | 🌐 Lua | 📅 2023-07-06 - Open the current word with custom openers, GitHub shorthand for example.
* [tristone13th/lspmark.nvim](https://github.com/tristone13th/lspmark.nvim) ⭐ 57 | 🐛 3 | 🌐 Lua | 📅 2025-07-16 - Sane project-wise bookmarks with persistent storage based on LSP.
* [2KAbhishek/markit.nvim](https://github.com/2KAbhishek/markit.nvim) ⭐ 53 | 🐛 0 | 🌐 Lua | 📅 2025-10-09 - Improved global marks and project wide bookmarks, to quickly navigate files.
* [dimtion/guttermarks.nvim](https://github.com/dimtion/guttermarks.nvim) ⭐ 44 | 🐛 0 | 🌐 Lua | 📅 2026-02-14 - Display marks in the buffer gutter.
* [walkersumida/fusen.nvim](https://github.com/walkersumida/fusen.nvim) ⭐ 36 | 🐛 0 | 🌐 Lua | 📅 2026-02-02 - Sticky note bookmarks, per Git branch with hover annotations and Telescope integration.
* [desdic/marlin.nvim](https://github.com/desdic/marlin.nvim) ⭐ 31 | 🐛 0 | 🌐 Lua | 📅 2025-05-28 - Like harpoon, but with key differences like project path, split support, no UI.
* [heilgar/bookmarks.nvim](https://github.com/heilgar/bookmarks.nvim) ⭐ 25 | 🐛 1 | 🌐 Lua | 📅 2025-12-01 - Manage line bookmarks with Telescope integration and SQLite storage.
* [niuiic/track.nvim](https://github.com/niuiic/track.nvim) ⭐ 25 | 🐛 0 | 🌐 Lua | 📅 2024-11-18 - Enhanced mark with description. Track the thought process of reading source code.
* [zongben/navimark.nvim](https://github.com/zongben/navimark.nvim) ⭐ 20 | 🐛 0 | 🌐 Lua | 📅 2025-09-17 - An easy and powerful bookmark manager with telescope.
* [markgandolfo/dartboard.nvim](https://github.com/markgandolfo/dartboard.nvim) ⭐ 15 | 🐛 0 | 🌐 Lua | 📅 2025-06-08 - Mark files and quickly access them, inspired by Harpoon and Lasso.
* [y3owk1n/warp.nvim](https://github.com/y3owk1n/warp.nvim) ⭐ 14 | 🐛 0 | 🌐 Lua | 📅 2025-12-14 - Simple harpoon alternative that focuses on marking and navigating between files.
* [mohseenrm/marko.nvim](https://github.com/mohseenrm/marko.nvim) ⭐ 11 | 🐛 0 | 🌐 Lua | 📅 2025-12-01 - Behind the scenes, global marks management for different projects.
* [Beargruug/skipper.nvim](https://github.com/Beargruug/skipper.nvim/) ⭐ 7 | 🐛 0 | 🌐 Lua | 📅 2026-02-11 - Jump between functions in a file with ease.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Search

* [nvim-pack/nvim-spectre](https://github.com/nvim-pack/nvim-spectre) ⭐ 2,367 | 🐛 13 | 🌐 Lua | 📅 2025-05-19 - Search and replace panel.
* [MagicDuck/grug-far.nvim](https://github.com/MagicDuck/grug-far.nvim) ⭐ 1,771 | 🐛 3 | 🌐 Lua | 📅 2026-02-02 - Buffer-based live search and replace with full power of `rg` flags. Grug like!
* [kevinhwang91/nvim-hlslens](https://github.com/kevinhwang91/nvim-hlslens) ⭐ 894 | 🐛 9 | 🌐 Lua | 📅 2026-01-11 - Helps you better glance searched information, seamlessly jump matched instances.
* [AckslD/muren.nvim](https://github.com/AckslD/muren.nvim/) ⭐ 363 | 🐛 13 | 🌐 Lua | 📅 2025-02-09 - Multiple replacements through interactive UI.
* [chrisgrieser/nvim-rip-substitute](https://github.com/chrisgrieser/nvim-rip-substitute) ⭐ 305 | 🐛 1 | 🌐 Lua | 📅 2026-02-06 - Search and replace in the current buffer or workspace with incremental preview, a convenient UI, and modern regex syntax.
* [ray-x/sad.nvim](https://github.com/ray-x/sad.nvim) ⭐ 204 | 🐛 4 | 🌐 Lua | 📅 2025-05-01 - Space Age seD integration. Batch file edit tool, a wrapper for [sad](https://github.com/ms-jpq/sad) ⭐ 2,002 | 🐛 28 | 🌐 Rust | 📅 2025-09-30
* [FabianWirth/search.nvim](https://github.com/FabianWirth/search.nvim) ⭐ 187 | 🐛 7 | 🌐 Lua | 📅 2024-05-21 - Tabs for different Telescope pickers.
* [prochri/telescope-all-recent.nvim](https://github.com/prochri/telescope-all-recent.nvim) ⭐ 149 | 🐛 1 | 🌐 Lua | 📅 2025-03-19 - Frequency and recency sorter for any Telescope picker.
* [2KAbhishek/seeker.nvim](https://github.com/2KAbhishek/seeker.nvim) ⭐ 121 | 🐛 2 | 🌐 Lua | 📅 2026-02-13 - Progressive file seeker built on top of `snacks.nvim`.
* [mangelozzi/rgflow.nvim](https://github.com/mangelozzi/rgflow.nvim) ⭐ 106 | 🐛 0 | 🌐 Lua | 📅 2025-08-11 - Quickly get RipGrep results into an editable Quickfix list, while learning RipGrep's CLI.
* [rktjmp/highlight-current-n.nvim](https://github.com/rktjmp/highlight-current-n.nvim) ⭐ 92 | 🐛 0 | 🌐 Fennel | 📅 2023-06-26 - Highlights the current /, ? or \* match under your cursor when pressing n or N and gets out of the way afterwards.
* [nvimdev/hlsearch.nvim](https://github.com/nvimdev/hlsearch.nvim) ⭐ 79 | 🐛 0 | 🌐 Lua | 📅 2024-01-10 - Auto remove search highlight and rehighlight when using n or N.
* [polirritmico/telescope-lazy-plugins.nvim](https://github.com/polirritmico/telescope-lazy-plugins.nvim) ⭐ 73 | 🐛 0 | 🌐 Lua | 📅 2025-02-15 - A Telescope picker to quickly access plugins configurations from the lazy.nvim spec.
* [wurli/visimatch.nvim](https://github.com/wurli/visimatch.nvim) ⭐ 72 | 🐛 5 | 🌐 Lua | 📅 2025-09-25 - Adds highlights to any text matching the current selection in visual mode.
* [s1n7ax/nvim-search-and-replace](https://github.com/s1n7ax/nvim-search-and-replace) ⭐ 69 | 🐛 1 | 🌐 Lua | 📅 2022-09-06 - Search and replace in multiple files at the same time from the current working directory.
* [backdround/improved-search.nvim](https://github.com/backdround/improved-search.nvim) ⭐ 61 | 🐛 0 | 🌐 Lua | 📅 2023-12-21 - Add search abilities.
* [duane9/nvim-rg](https://github.com/duane9/nvim-rg) ⭐ 44 | 🐛 1 | 🌐 Vim Script | 📅 2025-11-18 - Run RipGrep asynchronously and see results in a quickfix window.
* [wsdjeg/flygrep.nvim](https://github.com/wsdjeg/flygrep.nvim) ⭐ 18 | 🐛 1 | 🌐 Lua | 📅 2026-01-11 - Search text in a floating window asynchronously.
* [bravoecho/brook.nvim](https://github.com/bravoecho/brook.nvim) ⭐ 10 | 🐛 0 | 🌐 Lua | 📅 2026-02-14 - Responsive, shell-safe ripgrep search for the quickfix list, with native n/N navigation.
* [mahyarmirrashed/search-and-replace.nvim](https://github.com/mahyarmirrashed/search-and-replace.nvim) ⭐ 8 | 🐛 0 | 🌐 Lua | 📅 2025-07-04 - Simple, effective, search and replace functionality for the pragmatic engineer.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Fuzzy Finder

* [nvim-telescope/telescope.nvim](https://github.com/nvim-telescope/telescope.nvim) ⭐ 19,068 | 🐛 482 | 🌐 Lua | 📅 2026-02-16 - Telescope.nvim is a highly [extendable](https://github.com/nvim-telescope/telescope.nvim/wiki/Extensions) ⭐ 19,068 | 🐛 482 | 🌐 Lua | 📅 2026-02-16 A highly extensible fuzzy finder over lists.
* [nvim-mini/mini.nvim#mini.fuzzy](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-fuzzy.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` with functions to perform fuzzy matching of one string to others along with fast Telescope sorter.
* [nvim-mini/mini.nvim#mini.pick](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-pick.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` with general purpose interactive non-blocking picker that has one window design, toggleable preview, flexible and fast default match, and much more.
* [nvim-mini/mini.nvim#mini.extra](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-extra.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` with extra functionality for its modules. Contains 20+ 'mini.pick' pickers, 'mini.ai' textobjects, and more.
* [folke/snacks.nvim#picker](https://github.com/folke/snacks.nvim/blob/main/docs/picker.md) ⭐ 7,082 | 🐛 95 | 🌐 Lua | 📅 2025-11-18 - A modern fuzzy-finder to navigate the Neovim universe.
* [ibhagwan/fzf-lua](https://github.com/ibhagwan/fzf-lua) ⭐ 4,066 | 🐛 9 | 🌐 Lua | 📅 2026-02-17 - The Lua version of `fzf.vim`, high-performance and fully async, supports `nvim-web-devicons`, Git indicators, LSP, quickfix/location lists and more. Also supports [`skim`](https://github.com/lotabout/skim) ⭐ 6,569 | 🐛 24 | 🌐 Rust | 📅 2026-02-17 as its fzf binary.
* [dmtrKovalenko/fff.nvim](https://github.com/dmtrKovalenko/fff.nvim) ⭐ 1,398 | 🐛 51 | 🌐 Rust | 📅 2026-02-17 - Fuzzy file picker with a standalone native implementation of file indexing and typo resistant fuzzy matcher. Includes all the QOL features, file previews (and images), frecency sorting, last query matching, proximity, Git status bonuses and much more.
* [nvim-telescope/telescope-media-files.nvim](https://github.com/nvim-telescope/telescope-media-files.nvim) ⭐ 523 | 🐛 35 | 🌐 Lua | 📅 2024-03-30 - Preview images, pdf, epub, video, and fonts using Telescope.
* [camspiers/snap](https://github.com/camspiers/snap) ⭐ 508 | 🐛 28 | 🌐 Fennel | 📅 2025-03-06 - An extensible fuzzy finder. Similar to Telescope, and optimized for performance, especially when grepping in large codebases.
* [bassamsdata/namu.nvim](https://github.com/bassamsdata/namu.nvim) ⭐ 414 | 🐛 5 | 🌐 Lua | 📅 2026-02-17 - Flexible and sleek fuzzy picker, LSP symbol navigator, and more.
* [axkirillov/easypick.nvim](https://github.com/axkirillov/easypick.nvim) ⭐ 406 | 🐛 4 | 🌐 Lua | 📅 2025-04-26 - Easypick lets you easily create Telescope pickers from arbitrary console commands.
* [jvgrootveld/telescope-zoxide](https://github.com/jvgrootveld/telescope-zoxide) ⭐ 367 | 🐛 8 | 🌐 Lua | 📅 2024-08-28 - Telescope integration for [zoxide](https://github.com/ajeetdsouza/zoxide) ⭐ 33,434 | 🐛 153 | 🌐 Rust | 📅 2026-02-07, a smart directory picker that tracks your usage.
* [vijaymarupudi/nvim-fzf](https://github.com/vijaymarupudi/nvim-fzf) ⭐ 349 | 🐛 3 | 🌐 Lua | 📅 2024-10-21 - A Lua API for using FZF. Allows for full asynchronicity for UI speed and usability.
* [linrongbin16/fzfx.nvim](https://github.com/linrongbin16/fzfx.nvim) ⚠️ Archived - A fuzzy finder that updates on every keystroke.
* [fdschmidt93/telescope-egrepify.nvim](https://github.com/fdschmidt93/telescope-egrepify.nvim) ⭐ 140 | 🐛 10 | 🌐 Lua | 📅 2025-12-21 - Telescope plugin for better `rg` flags in `live_grep`.
* [crispgm/telescope-heading.nvim](https://github.com/crispgm/telescope-heading.nvim) ⭐ 139 | 🐛 5 | 🌐 Lua | 📅 2024-06-11 - Telescope extension to switch between headings of AsciiDoc, Markdown, Vimdoc, etc.
* [wsdjeg/picker.nvim](https://github.com/wsdjeg/picker.nvim) ⭐ 39 | 🐛 1 | 🌐 Lua | 📅 2026-02-14 - Simple fuzzy finder, including files, ctags outline, and more.
* [juniorsundar/refer.nvim](https://github.com/juniorsundar/refer.nvim) ⭐ 31 | 🐛 1 | 🌐 Lua | 📅 2026-02-14 - A minimalist picker that doesn't get in your way.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## File Explorer

* [nvim-mini/mini.nvim#mini.files](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-files.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` providing file explorer with column view capable of manipulating file system by editing text. Can create/delete/rename/copy/move files/directories inside and across directories.
* [nvim-tree/nvim-tree.lua](https://github.com/nvim-tree/nvim-tree.lua) ⭐ 8,373 | 🐛 101 | 🌐 Lua | 📅 2026-02-17 - A simple and fast file explorer tree.
* [stevearc/oil.nvim](https://github.com/stevearc/oil.nvim) ⭐ 6,255 | 🐛 122 | 🌐 Lua | 📅 2026-01-17 - Edit your filesystem like a buffer.
* [nvim-neo-tree/neo-tree.nvim](https://github.com/nvim-neo-tree/neo-tree.nvim) ⭐ 5,241 | 🐛 168 | 🌐 Lua | 📅 2026-02-17 - Browse the file system and other tree-like structures in whatever style suits you, including sidebars, floating windows, `netrw` split style, or all of them at once.
* [ms-jpq/chadtree](https://github.com/ms-jpq/chadtree) ⭐ 1,685 | 🐛 93 | 🌐 Python | 📅 2026-02-18 - File manager. Better than NERDTree.
* [mikavilpas/yazi.nvim](https://github.com/mikavilpas/yazi.nvim) ⭐ 1,554 | 🐛 10 | 🌐 Lua | 📅 2026-02-17 - Integration with the Yazi terminal file manager.
* [kevinhwang91/rnvimr](https://github.com/kevinhwang91/rnvimr) ⭐ 842 | 🐛 10 | 🌐 Python | 📅 2026-01-11 - A simple yet amazing file explorer.
* [A7Lavinraj/fyler.nvim](https://github.com/A7Lavinraj/fyler.nvim) ⭐ 663 | 🐛 20 | 🌐 Lua | 📅 2026-02-14 - File manager which can edit file system like a buffer with tree view.
* [luukvbaal/nnn.nvim](https://github.com/luukvbaal/nnn.nvim) ⭐ 450 | 🐛 1 | 🌐 Lua | 📅 2025-04-18 - File explorer powered by [nnn](https://github.com/jarun/nnn) ⭐ 21,274 | 🐛 1 | 🌐 C | 📅 2026-02-14 and Lua.
* [tamago324/lir.nvim](https://github.com/tamago324/lir.nvim) ⭐ 372 | 🐛 12 | 🌐 Lua | 📅 2024-05-26 - Simple file explorer.
* [prichrd/netrw.nvim](https://github.com/prichrd/netrw.nvim) ⭐ 266 | 🐛 3 | 🌐 Lua | 📅 2025-01-19 - Add icons and custom keybindings to netrw.
* [simonmclean/triptych.nvim](https://github.com/simonmclean/triptych.nvim) ⭐ 248 | 🐛 1 | 🌐 Lua | 📅 2025-12-25 - A directory browser inspired by Ranger.
* [SidOfc/carbon.nvim](https://github.com/SidOfc/carbon.nvim) ⭐ 184 | 🐛 1 | 🌐 Lua | 📅 2025-02-04 - The simple directory tree viewer written in Lua.
* [X3eRo0/dired.nvim](https://github.com/X3eRo0/dired.nvim) ⭐ 184 | 🐛 4 | 🌐 Lua | 📅 2026-01-30 - A file browser inspired by Emacs Dired.
* [kelly-lin/ranger.nvim](https://github.com/kelly-lin/ranger.nvim) ⭐ 179 | 🐛 11 | 🌐 Lua | 📅 2024-11-18 - [Ranger](https://github.com/ranger/ranger) ⭐ 16,869 | 🐛 925 | 🌐 Python | 📅 2026-01-22 integration.
* [Xuyuanp/yanil](https://github.com/Xuyuanp/yanil) ⭐ 98 | 🐛 5 | 🌐 Lua | 📅 2026-01-15 - Yet Another Nerdtree In Lua.
* [rolv-apneseth/tfm.nvim](https://github.com/Rolv-Apneseth/tfm.nvim) ⭐ 96 | 🐛 2 | 🌐 Lua | 📅 2026-01-18 - Similar to `fm-nvim`, this provides integration for several popular terminal file managers (including [yazi](https://github.com/sxyazi/yazi) ⭐ 32,797 | 🐛 62 | 🌐 Rust | 📅 2026-02-17).
* [theblob42/drex.nvim](https://github.com/TheBlob42/drex.nvim) ⭐ 95 | 🐛 1 | 🌐 Lua | 📅 2025-05-09 - A simple and configurable file explorer written in Lua.
* [kiran94/s3edit.nvim](https://github.com/kiran94/s3edit.nvim) ⭐ 49 | 🐛 0 | 🌐 Lua | 📅 2025-04-13 - Edit files from Amazon S3.
* [saifulapm/neotree-file-nesting-config](https://github.com/saifulapm/neotree-file-nesting-config) ⭐ 28 | 🐛 0 | 🌐 Lua | 📅 2025-03-06 - Pre-defined file nesting rules for `neo-tree.nvim`.
* [vodchella/hodur.nvim](https://github.com/vodchella/hodur.nvim) ⭐ 21 | 🐛 0 | 🌐 Lua | 📅 2025-11-10 - Allows you to quickly open a file or copy URL located under cursor.
* [Enigama/miss.nvim](https://github.com/Enigama/miss.nvim) ⭐ 11 | 🐛 0 | 🌐 Lua | 📅 2025-08-17 - Simple popup with changed `unsaved` files, allowing you to save and open them. Helps to avoid forgetting to add something to GitHub or similar.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Project

* [nvim-mini/mini.nvim#mini.visits](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-visits.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` to persistently track and reuse file system visits. Allows listing "recent"/"frequent"/"frecent" visits, adding/removing labels to visits and other data.
* [natecraddock/workspaces.nvim](https://github.com/natecraddock/workspaces.nvim) ⭐ 372 | 🐛 8 | 🌐 Lua | 📅 2024-10-08 - Manage workspace directories.
* [GnikDroy/projections.nvim](https://github.com/GnikDroy/projections.nvim) ⭐ 246 | 🐛 8 | 🌐 Lua | 📅 2024-02-05 - Tiny project + session manager.
* [cljoly/telescope-repo.nvim](https://github.com/cljoly/telescope-repo.nvim) ⭐ 238 | 🐛 14 | 🌐 Lua | 📅 2025-01-21 - Telescope picker to jump to any repository (Git or other) on the file system.
* [klen/nvim-config-local](https://github.com/klen/nvim-config-local) ⭐ 177 | 🐛 5 | 🌐 Lua | 📅 2025-01-21 - Secure load local config files from working directories.
* [DrKJeff16/project.nvim](https://github.com/DrKJeff16/project.nvim) ⭐ 137 | 🐛 1 | 🌐 Lua | 📅 2026-02-16 - Project manager with project root detection, documented code and lots of improvements, including `snacks.nvim`, `fzf-lua` and `picker.nvim` support.
* [LintaoAmons/cd-project.nvim](https://github.com/LintaoAmons/cd-project.nvim) ⭐ 126 | 🐛 6 | 🌐 Lua | 📅 2026-01-12 - All you need is just an easier way to `cd` to another project directory.
* [windwp/nvim-projectconfig](https://github.com/windwp/nvim-projectconfig) ⭐ 111 | 🐛 5 | 🌐 Lua | 📅 2024-07-28 - Loads Neovim config depending on the project directory.
* [otavioschwanck/telescope-alternate.nvim](https://github.com/otavioschwanck/telescope-alternate.nvim) ⭐ 106 | 🐛 5 | 🌐 Lua | 📅 2025-07-05 - Alternate between common files using telescope.
* [SalOrak/whaler.nvim](https://github.com/SalOrak/whaler.nvim) ⭐ 73 | 🐛 0 | 🌐 Lua | 📅 2026-01-31 - Telescope extension to move between directories blazingly fast.
* [nyngwang/suave.lua](https://github.com/nyngwang/suave.lua) ⭐ 70 | 🐛 10 | 🌐 Lua | 📅 2025-08-02 - Multi-tabs project session automation.
* [mrjones2014/codesettings.nvim](https://github.com/mrjones2014/codesettings.nvim) ⭐ 54 | 🐛 0 | 🌐 Lua | 📅 2026-02-18 - Easily load project-local settings (like `.vscode/settings.json`) into Neovim 0.11+ native LSP settings.
* [Abstract-IDE/penvim](https://github.com/Abstract-IDE/penvim) ⭐ 51 | 🐛 1 | 🌐 Lua | 📅 2022-07-23 - Project's root directory and documents Indentation detector with project based config loader.
* [desdic/telescope-rooter.nvim](https://github.com/desdic/telescope-rooter.nvim) ⭐ 26 | 🐛 0 | 🌐 Lua | 📅 2024-05-18 - Makes sure to always start telescope (and only telescope) from the project/root directory.
* [wsdjeg/rooter.nvim](https://github.com/wsdjeg/rooter.nvim) ⭐ 21 | 🐛 0 | 🌐 Lua | 📅 2025-12-03 - Change working directory to project root.
* [josephschmitt/pj.nvim](https://github.com/josephschmitt/pj.nvim) ⭐ 21 | 🐛 0 | 🌐 Lua | 📅 2026-02-02 - Automatic project discovery with configurable depth with multiple pickers supported (Snacks, Telescope, fzf-lua).
* [zongben/proot.nvim](https://github.com/zongben/proot.nvim) ⭐ 9 | 🐛 0 | 🌐 Lua | 📅 2025-10-15 - Lightweight project navigator with telescope.
* [LucasTavaresA/headers.nvim](https://github.com/LucasTavaresA/headers.nvim) ⭐ 4 | 🐛 1 | 🌐 Lua | 📅 2025-12-11 - Zero-config header/footer warnings.
* [cosmicbuffalo/root\_swapper.nvim](https://github.com/cosmicbuffalo/root_swapper.nvim) ⭐ 2 | 🐛 0 | 🌐 Lua | 📅 2026-01-08 - Lightweight root swapper that uses `lcd` to swap to the appropriate root directory based on the current buffer.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Buffers

* [famiu/bufdelete.nvim](https://github.com/famiu/bufdelete.nvim) ⚠️ Archived - Delete buffers without losing your window layout.
* [rgroli/other.nvim](https://github.com/rgroli/other.nvim) ⭐ 482 | 🐛 9 | 🌐 Lua | 📅 2025-05-09 - Open alternative files for the current buffer.
* [j-morano/buffer\_manager.nvim](https://github.com/j-morano/buffer_manager.nvim) ⭐ 379 | 🐛 3 | 🌐 Lua | 📅 2026-02-04 - Add one or more buffers, reorder them, save them inside a file or just delete them very easily from a small floating window.
* [chrisgrieser/nvim-early-retirement](https://github.com/chrisgrieser/nvim-early-retirement) ⭐ 246 | 🐛 0 | 🌐 Lua | 📅 2026-02-06 - Send buffers into early retirement by automatically closing them after x minutes of inactivity.
* [axkirillov/hbac.nvim](https://github.com/axkirillov/hbac.nvim) ⭐ 220 | 🐛 0 | 🌐 Lua | 📅 2024-10-09 - Automatically close buffers you are not working on.
* [kazhala/close-buffers.nvim](https://github.com/kazhala/close-buffers.nvim) ⭐ 173 | 🐛 6 | 🌐 Lua | 📅 2023-06-02 - Delete multiple Vim buffers based on different conditions.
* [dzfrias/arena.nvim](https://github.com/dzfrias/arena.nvim) ⭐ 104 | 🐛 3 | 🌐 Lua | 📅 2026-01-13 - A smart (frecency-based) buffer switcher.
* [m-demare/attempt.nvim](https://github.com/m-demare/attempt.nvim) ⭐ 92 | 🐛 2 | 🌐 Lua | 📅 2025-02-04 - Manage and run temporary buffers.
* [ahkohd/buffer-sticks.nvim](https://github.com/ahkohd/buffer-sticks.nvim) ⭐ 78 | 🐛 1 | 🌐 Lua | 📅 2026-02-02 - Cosmetic buffers indicator and picker.
* [backdround/tabscope.nvim](https://github.com/backdround/tabscope.nvim) ⭐ 58 | 🐛 5 | 🌐 Lua | 📅 2023-10-09 - Make tab-local buffers.
* [francescarpi/buffon.nvim](https://github.com/francescarpi/buffon.nvim) ⭐ 29 | 🐛 6 | 🌐 Lua | 📅 2025-08-19 - Buffers navigation, reorganize and close.
* [sQVe/bufignore.nvim](https://github.com/sQVe/bufignore.nvim) ⭐ 17 | 🐛 0 | 🌐 Lua | 📅 2026-01-08 - Unlist hidden buffers matching specified ignore sources.
* [ChuufMaster/buffer-vacuum](https://github.com/ChuufMaster/buffer-vacuum) ⭐ 13 | 🐛 0 | 🌐 Lua | 📅 2025-08-18 - Set a maximum number of buffers to keep open and intelligently delete the oldest buffers over the maximum.
* [wsdjeg/bufdel.nvim](https://github.com/wsdjeg/bufdel.nvim) ⭐ 11 | 🐛 2 | 🌐 Lua | 📅 2026-01-30 - Delete buffers without changing windows layout.
* [mong8se/buffish.nvim](https://github.com/mong8se/buffish.nvim) ⭐ 5 | 🐛 0 | 🌐 Lua | 📅 2025-10-13 - A buffer switcher in the spirit of dirvish or vinegar.
* [BibekBhusal0/bufstack.nvim](https://github.com/BibekBhusal0/bufstack.nvim) ⭐ 5 | 🐛 0 | 🌐 Lua | 📅 2026-02-15 - Track recently visited buffers and reopen recently closed buffers.
* [TheLazyCat00/workspaces-nvim](https://github.com/TheLazyCat00/workspaces-nvim) ⭐ 4 | 🐛 0 | 🌐 Lua | 📅 2026-02-14 - Pin files to specific keys within a project workspace, giving you quick access to your most important files.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Color

* [nvim-mini/mini.nvim#mini.hipatterns](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-hipatterns.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` to highlight patterns in text with configurable highlighters. Works asynchronously with configurable debounce delay.
* [folke/twilight.nvim](https://github.com/folke/twilight.nvim) ⭐ 1,508 | 🐛 0 | 🌐 Lua | 📅 2025-10-28 - Dim inactive portions of the code you're editing using Tree-sitter.
* [catgoose/nvim-colorizer.lua](https://github.com/catgoose/nvim-colorizer.lua) ⭐ 992 | 🐛 18 | 🌐 Lua | 📅 2026-01-31 - A high-performance color highlighter which has no external dependencies.
* [uga-rosa/ccc.nvim](https://github.com/uga-rosa/ccc.nvim) ⭐ 958 | 🐛 11 | 🌐 Lua | 📅 2025-05-06 - Super powerful color picker / colorizer plugin.
* [TaDaa/vimade](https://github.com/TaDaa/vimade) ⭐ 648 | 🐛 6 | 🌐 Lua | 📅 2025-12-14 - Dim, fade, tint, animate, and customize colors in your windows and buffers.
* [nvzone/minty](https://github.com/nvzone/minty) ⭐ 576 | 🐛 2 | 🌐 Lua | 📅 2025-02-28 - Beautifully crafted color tools.
* [xzbdmw/colorful-menu.nvim](https://github.com/xzbdmw/colorful-menu.nvim) ⭐ 441 | 🐛 2 | 🌐 Lua | 📅 2025-11-25 - Colorize your auto completion menu using Tree-sitter.
* [max397574/colortils.nvim](https://github.com/max397574/colortils.nvim) ⭐ 434 | 🐛 8 | 🌐 Lua | 📅 2025-01-10 - Provides utils to work with colors (picker, conversion).
* [rasulomaroff/reactive.nvim](https://github.com/rasulomaroff/reactive.nvim) ⭐ 239 | 🐛 8 | 🌐 Lua | 📅 2025-12-30 - Set global and window-specific highlights or trigger callbacks when modes/operators change or windows are switched.
* [winston0410/range-highlight.nvim](https://github.com/winston0410/range-highlight.nvim) ⭐ 211 | 🐛 3 | 🌐 Lua | 📅 2025-12-10 - An extremely lightweight plugin (\~ 120loc) that highlights ranges you have entered in commandline.
* [miversen33/sunglasses.nvim](https://github.com/miversen33/sunglasses.nvim) ⭐ 158 | 🐛 7 | 🌐 Lua | 📅 2025-01-13 - Dynamic Colorscheme/highlight adjuster on window switching.
* [rachartier/tiny-devicons-auto-colors.nvim](https://github.com/rachartier/tiny-devicons-auto-colors.nvim) ⭐ 128 | 🐛 0 | 🌐 Lua | 📅 2025-01-03 - Automatically updates nvim-web-devicons colors based on your current colorscheme.
* [Mr-LLLLL/interestingwords.nvim](https://github.com/Mr-LLLLL/interestingwords.nvim) ⭐ 52 | 🐛 0 | 🌐 Lua | 📅 2024-08-19 - Highlight multiple word same time and navigate word under cursor with scrolling smoothly, display search count in virualtext.
* [lcheylus/overlength.nvim](https://github.com/lcheylus/overlength.nvim) ⭐ 50 | 🐛 0 | 🌐 Lua | 📅 2025-08-05 - A small plugin to highlight too long lines.
* [moyiz/command-and-cursor.nvim](https://github.com/moyiz/command-and-cursor.nvim) ⭐ 22 | 🐛 0 | 🌐 Lua | 📅 2025-03-30 - Highlight cursor and visual selections when entering command mode.
* [wsdjeg/cpicker.nvim](https://github.com/wsdjeg/cpicker.nvim) ⭐ 8 | 🐛 1 | 🌐 Lua | 📅 2025-12-03 - A lightweight color palette plugin that supports a wide range of color models.
* [3ZsForInsomnia/pacer.nvim](https://github.com/3ZsForInsomnia/pacer.nvim) ⭐ 4 | 🐛 0 | 🌐 Lua | 📅 2025-10-20 - Creates a reading pacer by highlighting one word at a time and dimming all text outside the current paragraph-and-some to help you read faster.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Colorscheme

Each colorscheme will have one or more of the tags listed below. If a tag is missing
then it is not supported:

<!--lint disable awesome-list-item-->

* ***`[TS]`*** - Has Tree-sitter highlighting.
* ***`[LSP]`*** - Has LSP Semantic Tokens support.
* ***`[L/D]`*** - Has both "light" and "dark" variants.
* ***`[Lua]`*** - Is written in Lua.
* ***`[Fnl]`*** - Is written in Fennel.

<!--lint enable awesome-list-item-->

* [folke/tokyonight.nvim](https://github.com/folke/tokyonight.nvim) ⭐ 7,824 | 🐛 15 | 🌐 Lua | 📅 2025-11-05 - ***`[TS][LSP][L/D][Lua]`*** A clean, dark and light theme written in Lua, with support for LSP, Tree-sitter and lots of plugins.
* [sainnhe/everforest](https://github.com/sainnhe/everforest) ⭐ 3,861 | 🐛 7 | 🌐 Vim Script | 📅 2026-01-21 - ***`[TS][LSP][L/D]`*** A green based colorscheme designed to be warm, soft and easy on the eyes.
* [sainnhe/gruvbox-material](https://github.com/sainnhe/gruvbox-material) ⭐ 2,487 | 🐛 8 | 🌐 Vim Script | 📅 2026-01-21 - ***`[TS][LSP]`*** Gruvbox modification with softer contrast and Tree-sitter support.
* [projekt0n/github-nvim-theme](https://github.com/projekt0n/github-nvim-theme) ⭐ 2,420 | 🐛 27 | 🌐 Lua | 📅 2024-12-31 - ***`[TS][LSP][L/D][Lua]`*** A GitHub theme, kitty, alacritty written in Lua. Support built-in LSP and Tree-sitter.
* [navarasu/onedark.nvim](https://github.com/navarasu/onedark.nvim) ⭐ 1,918 | 🐛 55 | 🌐 Lua | 📅 2025-11-24 - ***`[TS][LSP][Lua]`*** A One Dark Theme written in Lua based on Atom's One Dark Theme.
* [sainnhe/sonokai](https://github.com/sainnhe/sonokai) ⭐ 1,916 | 🐛 1 | 🌐 Vim Script | 📅 2026-01-21 - ***`[TS][LSP]`*** High Contrast and Vivid Color Scheme based on Monokai Pro.
* [nyoom-engineering/oxocarbon.nvim](https://github.com/nyoom-engineering/oxocarbon.nvim) ⭐ 1,523 | 🐛 19 | 🌐 Fennel | 📅 2025-09-05 - ***`[TS][LSP][L/D][Lua]`*** A dark and light theme written in Fennel, inspired by IBM Carbon.
* [dracula/vim](https://github.com/dracula/vim) ⭐ 1,376 | 🐛 10 | 🌐 Vim Script | 📅 2025-11-09 - ***`[TS][LSP]`*** Famous beautiful dark powered theme.
* [bluz71/vim-moonfly-colors](https://github.com/bluz71/vim-moonfly-colors) ⭐ 1,247 | 🐛 0 | 🌐 Lua | 📅 2026-01-18 - ***`[TS][LSP][Lua]`*** A dark charcoal colorscheme with Tree-sitter support.
* [mhartington/oceanic-next](https://github.com/mhartington/oceanic-next) ⭐ 1,174 | 🐛 10 | 🌐 Vim Script | 📅 2025-10-10 - ***`[TS][L/D]`*** Oceanic Next theme.
* [marko-cerovac/material.nvim](https://github.com/marko-cerovac/material.nvim) ⭐ 1,072 | 🐛 7 | 🌐 Lua | 📅 2026-01-05 - ***`[TS][LSP][L/D][Lua]`*** Material.nvim is a highly configurable colorscheme written in Lua and based on the material palette.
* [tomasiser/vim-code-dark](https://github.com/tomasiser/vim-code-dark) ⭐ 999 | 🐛 15 | 🌐 Vim Script | 📅 2024-05-21 - ***`[TS]`*** A dark color scheme heavily inspired by the look of the Dark+ scheme of VSCode.
* [sainnhe/edge](https://github.com/sainnhe/edge) ⭐ 992 | 🐛 2 | 🌐 Vim Script | 📅 2026-01-21 - ***`[TS][LSP][L/D]`*** Clean and Elegant Color Scheme inspired by Atom One and Material.
* [AlexvZyl/nordic.nvim](https://github.com/AlexvZyl/nordic.nvim) ⭐ 991 | 🐛 4 | 🌐 Lua | 📅 2026-02-08 - ***`[TS][Lua]`*** Nord theme, but warmer and darker. Supports a variety of plugins and other platforms.
* [shaunsingh/nord.nvim](https://github.com/shaunsingh/nord.nvim) ⭐ 976 | 🐛 33 | 🌐 Lua | 📅 2024-06-25 - ***`[TS][Lua]`*** A colorscheme based off of the Nord Color Palette.
* [Mofiqul/vscode.nvim](https://github.com/Mofiqul/vscode.nvim) ⭐ 948 | 🐛 51 | 🌐 Lua | 📅 2025-12-03 - ***`[TS][L/D][Lua]`*** A Lua port of vim-code-dark colorscheme with VSCode light and dark theme.
* [savq/melange-nvim](https://github.com/savq/melange-nvim) ⭐ 923 | 🐛 12 | 🌐 Lua | 📅 2025-12-10 - ***`[TS][LSP][L/D][Lua]`*** Warm colorscheme written in Lua with support for various terminal emulators.
* [bluz71/vim-nightfly-colors](https://github.com/bluz71/vim-nightfly-colors) ⭐ 921 | 🐛 0 | 🌐 Lua | 📅 2026-01-18 - ***`[TS][LSP][Lua]`*** A dark midnight colorscheme with Tree-sitter support.
* [fenetikm/falcon](https://github.com/fenetikm/falcon) ⭐ 826 | 🐛 12 | 🌐 Vim Script | 📅 2026-02-17 - ***`[TS][Lua]`*** A colour scheme for terminals, Vim and friends.
* [Mofiqul/dracula.nvim](https://github.com/Mofiqul/dracula.nvim) ⭐ 759 | 🐛 24 | 🌐 Lua | 📅 2025-11-05 - ***`[TS]`*** Dracula colorscheme written in Lua.
* [everviolet/nvim](https://github.com/everviolet/nvim) ⭐ 580 | 🐛 0 | 🌐 Lua | 📅 2026-02-17 - ***`[TS][LSP][L/D][Lua]`*** A comfy colorscheme for cozy morning coding.
* [neanias/everforest-nvim](https://github.com/neanias/everforest-nvim) ⭐ 419 | 🐛 7 | 🌐 Lua | 📅 2025-11-02 - ***`[TS][LSP][L/D][Lua]`*** A Lua port of the Everforest colour scheme.
* [tanvirtin/monokai.nvim](https://github.com/tanvirtin/monokai.nvim) ⭐ 384 | 🐛 14 | 🌐 Lua | 📅 2023-12-02 - ***`[TS][LSP][Lua]`*** Monokai theme written in Lua.
* [nvimdev/zephyr-nvim](https://github.com/nvimdev/zephyr-nvim) ⭐ 376 | 🐛 3 | 🌐 Lua | 📅 2022-12-31 - ***`[TS][Lua]`*** A dark colorscheme with Tree-sitter support.
* [ray-x/aurora](https://github.com/ray-x/aurora) ⭐ 370 | 🐛 2 | 🌐 Lua | 📅 2025-04-09 - ***`[TS][LSP][Lua]`*** A 24-bit dark theme with Tree-sitter and LSP support.
* [ChristianChiarulli/nvcode-color-schemes.vim](https://github.com/ChristianChiarulli/nvcode-color-schemes.vim) ⭐ 306 | 🐛 21 | 🌐 Vim script | 📅 2024-07-08 - ***`[TS]`*** Nvcode, onedark, nord colorschemes with Tree-sitter support.
* [NTBBloodbath/doom-one.nvim](https://github.com/NTBBloodbath/doom-one.nvim) ⭐ 246 | 🐛 10 | 🌐 Lua | 📅 2025-06-28 - ***`[TS][L/D][Lua]`*** Lua port of doom-emacs' doom-one.
* [ray-x/starry.nvim](https://github.com/ray-x/starry.nvim) ⭐ 240 | 🐛 3 | 🌐 Lua | 📅 2025-04-16 - ***`[TS][LSP][L/D][Lua]`*** A collection of modern colorschemes: `material`, `moonlight`, `dracula (blood)`, `monokai`, `mariana`, `emerald`, `earlysummer`, `middlenight_blue`, `darksolar`.
* [rockerBOO/boo-colorscheme-nvim](https://github.com/rockerBOO/boo-colorscheme-nvim) ⭐ 239 | 🐛 3 | 🌐 Lua | 📅 2026-02-10 - ***`[TS][Lua]`*** A colorscheme with handcrafted support for LSP, Tree-sitter.
* [datsfilipe/vesper.nvim](https://github.com/datsfilipe/vesper.nvim) ⭐ 218 | 🐛 0 | 🌐 Lua | 📅 2025-04-21 - ***`[TS][LSP][Lua]`*** It's a port of the popular VS Code theme Vesper, written in Lua.
* [askfiy/visual\_studio\_code](https://github.com/askfiy/visual_studio_code) ⭐ 214 | 🐛 4 | 🌐 Lua | 📅 2024-09-24 - ***`[TS][LSP][L/D][Lua]`***  A theme that highly restores VSCode.
* [Tsuzat/NeoSolarized.nvim](https://github.com/Tsuzat/NeoSolarized.nvim) ⚠️ Archived - ***`[TS][LSP][L/D][Lua]`*** NeoSolarized colorscheme with full transparency.
* [rafamadriz/neon](https://github.com/rafamadriz/neon) ⭐ 205 | 🐛 2 | 🌐 Lua | 📅 2022-11-27 - ***`[TS][LSP][L/D][Lua]`*** Customizable colorscheme with excellent italic and bold support, dark and light variants. Made to work and look good with Tree-sitter.
* [ishan9299/nvim-solarized-lua](https://github.com/ishan9299/nvim-solarized-lua) ⭐ 204 | 🐛 16 | 🌐 Lua | 📅 2024-03-04 - ***`[TS][Lua]`*** Solarized colorscheme written in Lua.
* [ishan9299/modus-theme-vim](https://github.com/ishan9299/modus-theme-vim) ⭐ 177 | 🐛 4 | 🌐 Lua | 📅 2022-10-09 - ***`[TS][L/D][Lua]`*** This is a color scheme developed by Protesilaos Stavrou for emacs.
* [andersevenrud/nordic.nvim](https://github.com/andersevenrud/nordic.nvim) ⭐ 176 | 🐛 4 | 🌐 Lua | 📅 2024-06-16 - ***`[TS][Lua]`*** A nord-esque colorscheme.
* [svrana/neosolarized.nvim](https://github.com/svrana/neosolarized.nvim) ⭐ 166 | 🐛 6 | 🌐 Lua | 📅 2025-06-12 - ***`[TS][LSP][Lua]`*** Dark solarized colorscheme using colorbuddy for easy customization.
* [kdheepak/monochrome.nvim](https://github.com/kdheepak/monochrome.nvim) ⭐ 161 | 🐛 1 | 🌐 Lua | 📅 2021-07-14 - ***`[TS][Lua]`*** A 16-bit monochrome colorscheme that uses [HSLuv](https://www.hsluv.org/) for perceptually distinct gray colors, with support for Tree-sitter and other commonly used plugins.
* [niyabits/calvera-dark.nvim](https://github.com/niyabits/calvera-dark.nvim) ⭐ 160 | 🐛 4 | 🌐 Lua | 📅 2021-12-23 - ***`[TS][Lua]`*** A port of the [VSCode Calvara Dark](https://github.com/saurabhdaware/vscode-calvera-dark) ⭐ 12 | 🐛 1 | 🌐 HTML | 📅 2024-08-17 theme with support for Tree-sitter and many other plugins.
* [serhez/teide.nvim](https://github.com/serhez/teide.nvim) ⭐ 139 | 🐛 1 | 🌐 Lua | 📅 2026-01-12 - ***`[TS][LSP][L/D][Lua]`*** A fork of folke's `tokyonight.nvim` with a different color palette.
* [ofirgall/ofirkai.nvim](https://github.com/ofirgall/ofirkai.nvim) ⭐ 137 | 🐛 14 | 🌐 Lua | 📅 2026-02-14 - ***`[TS][LSP][Lua]`*** Monokai theme that aims to feel like Sublime Text.
* [Th3Whit3Wolf/one-nvim](https://github.com/Th3Whit3Wolf/one-nvim) ⭐ 117 | 🐛 5 | 🌐 Lua | 📅 2021-07-26 - ***`[TS][L/D][Lua]`*** An Atom One inspired dark and light colorscheme.
* [uhs-robert/oasis.nvim](https://github.com/uhs-robert/oasis.nvim) ⭐ 114 | 🐛 3 | 🌐 CSS | 📅 2026-02-05 - ***`[TS][LSP][L/D][Lua]`*** Desert theme from Vim ported to Neovim and made modern with 12 variants, a collection of dark themes for every color of the rainbow.
* [Abstract-IDE/Abstract-cs](https://github.com/Abstract-IDE/Abstract-cs) ⭐ 112 | 🐛 2 | 🌐 Lua | 📅 2025-10-27 - ***`[TS][LSP][Lua]`*** Colorscheme written in Lua, specially made for roshnivim with Tree-sitter support.
* [Th3Whit3Wolf/onebuddy](https://github.com/Th3Whit3Wolf/onebuddy) ⭐ 101 | 🐛 4 | 🌐 Lua | 📅 2021-04-01 - ***`[TS][L/D][Lua]`*** Light and dark atom one theme.
* [sontungexpt/witch](https://github.com/sontungexpt/witch) ⭐ 71 | 🐛 2 | 🌐 Lua | 📅 2025-11-25 - ***`[TS][LSP][L/D][Lua]`*** The primary stinvim distro colorscheme includes the default feature of dimming inactive windows, along with various other customization options for users.
* [datsfilipe/min-theme.nvim](https://github.com/datsfilipe/min-theme.nvim) ⭐ 58 | 🐛 1 | 🌐 Lua | 📅 2024-08-03 - ***`[TS][LSP][Lua]`*** It's a port of Min, a minimal theme for VSCode, written in Lua.
* [Th3Whit3Wolf/space-nvim](https://github.com/Th3Whit3Wolf/space-nvim) ⭐ 49 | 🐛 2 | 🌐 Lua | 📅 2024-05-28 - ***`[TS][L/D][Lua]`*** A spacemacs inspired dark and light colorscheme.
* [bkegley/gloombuddy](https://github.com/bkegley/gloombuddy) ⭐ 48 | 🐛 0 | 🌐 Lua | 📅 2021-04-16 - ***`[TS][Lua]`*** Gloom inspired theme.
* [nxvu699134/vn-night.nvim](https://github.com/nxvu699134/vn-night.nvim) ⭐ 44 | 🐛 0 | 🌐 Lua | 📅 2025-02-17 - ***`[Lua]`*** A dark colorscheme written in Lua.
* [adisen99/codeschool.nvim](https://github.com/adisen99/codeschool.nvim) ⭐ 44 | 🐛 1 | 🌐 Lua | 📅 2026-02-10 - ***`[TS][LSP][Lua]`*** Codeschool colorscheme written in Lua with Tree-sitter and built-in LSP support.
* [wurli/cobalt.nvim](https://github.com/wurli/cobalt.nvim) ⭐ 25 | 🐛 0 | 🌐 Lua | 📅 2025-10-14 - ***`[TS][LSP][Lua]`*** A (mostly) faithful port of the classic blue theme from TextMate.
* [jim-at-jibba/ariake.nvim](https://github.com/jim-at-jibba/ariake.nvim) ⭐ 23 | 🐛 0 | 🌐 Lua | 📅 2025-11-11 - ***`[TS][LSP][Lua]`*** A port of the great Atom theme. Beautiful, dark colour scheme.
* [github-main-user/lytmode.nvim](https://github.com/github-main-user/lytmode.nvim) ⭐ 16 | 🐛 0 | 🌐 Lua | 📅 2025-11-09 - ***`[TS][LSP][Lua]`*** A unique in-between theme inspired by LYT-Mode for Obsidian. Not quite dark, not quite light — just right.
* [kuri-sun/yoda.nvim](https://github.com/kuri-sun/yoda.nvim) ⭐ 13 | 🐛 0 | 🌐 Lua | 📅 2025-12-19 - ***`[TS][LSP][L/D][Lua]`*** Muted green palette for focused, balanced editing.
* [yonatan-perel/lake-dweller.nvim](https://github.com/yonatan-perel/lake-dweller.nvim) ⭐ 11 | 🐛 0 | 🌐 Lua | 📅 2026-02-17 - ***`[TS][LSP][Lua]`*** Dark and opinionated with selective highlighting aiming to be readable at a glance.
* [silentium-theme/silentium.nvim](https://github.com/silentium-theme/silentium.nvim) ⭐ 11 | 🐛 0 | 🌐 Lua | 📅 2026-01-28 - ***`[TS][Luа]`*** Pragmatic and monochrome theme with the goal to increase reading speed and reduce eye strain by highlighting only what is needed.
* [jthvai/lavender.nvim](https://codeberg.org/jthvai/lavender.nvim) - ***`[TS][LSP][Lua]`*** Purple-hued dark mode colorscheme; a complete rewrite of shaunsingh/moonlight.nvim.

<!--lint disable awesome-spell-check-->

* [rose-pine/neovim](https://github.com/rose-pine/neovim) ⭐ 2,942 | 🐛 5 | 🌐 Lua | 📅 2025-12-21 - ***`[TS][LSP][L/D][Lua]`*** All natural pine, faux fur and a bit of soho vibes for the classy minimalist.

<!--lint enable awesome-spell-check-->

* [nvim-mini/mini.nvim#colorschemes](https://github.com/nvim-mini/mini.nvim#plugin-color-schemes) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - ***`[TS][LSP][L/D][Lua]`*** Color schemes included in `mini.nvim`. All of them prioritize high contrast ratio for reading text and computing palettes in perceptually uniform color spaces.
* [catppuccin/nvim](https://github.com/catppuccin/nvim) ⭐ 7,198 | 🐛 14 | 🌐 Lua | 📅 2026-02-17 - ***`[TS][LSP][L/D][Lua]`*** Warm mid-tone dark theme to show off your vibrant self! With support for native LSP, Tree-sitter, and more.
* [rebelot/kanagawa.nvim](https://github.com/rebelot/kanagawa.nvim) ⭐ 5,920 | 🐛 90 | 🌐 Lua | 📅 2025-10-15 - ***`[TS][LSP][L/D][Lua]`*** A dark colorscheme inspired by the colors of the famous painting by Katsushika Hokusai.
* [EdenEast/nightfox.nvim](https://github.com/EdenEast/nightfox.nvim) ⭐ 3,899 | 🐛 36 | 🌐 Lua | 📅 2025-02-09 - ***`[TS][LSP][L/D][Lua]`*** A soft dark, fully customizable colorscheme with support for LSP, Tree-sitter and a variety of plugins.
* [ellisonleao/gruvbox.nvim](https://github.com/ellisonleao/gruvbox.nvim) ⭐ 2,465 | 🐛 27 | 🌐 Lua | 📅 2026-02-15 - ***`[TS][LSP][L/D][Lua]`*** Gruvbox community colorscheme Lua port.
* [scottmckendry/cyberdream.nvim](https://github.com/scottmckendry/cyberdream.nvim) ⭐ 1,261 | 🐛 5 | 🌐 Lua | 📅 2026-01-27 - ***`[TS][L/D][Lua]`*** A high-contrast, futuristic and vibrant coloursheme.
* [zenbones-theme/zenbones.nvim](https://github.com/zenbones-theme/zenbones.nvim) ⭐ 1,063 | 🐛 16 | 🌐 Vim Script | 📅 2026-02-11 - ***`[TS][LSP][L/D][Lua]`*** A collection of Vim/Neovim colorschemes designed to highlight code using contrasts and font variations.
* [olimorris/onedarkpro.nvim](https://github.com/olimorris/onedarkpro.nvim) ⭐ 1,027 | 🐛 0 | 🌐 Lua | 📅 2026-01-15 - ***`[TS][L/D][Lua]`*** Atom's iconic One Dark theme. Cacheable, fully customisable, Tree-sitter and LSP semantic token support. Comes with light and dark variants.
* [embark-theme/vim](https://github.com/embark-theme/vim) ⭐ 717 | 🐛 1 | 🌐 Vim Script | 📅 2025-10-07 - ***`[TS]`*** A deep inky purple theme leveraging bright colors.
* [rmehri01/onenord.nvim](https://github.com/rmehri01/onenord.nvim) ⭐ 623 | 🐛 0 | 🌐 Lua | 📅 2025-12-25 - ***`[TS][LSP][L/D][Lua]`*** A colorscheme that combines the Nord and Atom One Dark color palettes for a more vibrant programming experience.
* [slugbyte/lackluster.nvim](https://github.com/slugbyte/lackluster.nvim) ⭐ 527 | 🐛 0 | 🌐 Lua | 📅 2025-10-06 - ***`[TS][LSP][Lua]`*** A delightful mostly grayscale colorscheme that is soft on the eyes, and supports heaps of plugins.
* [xero/miasma.nvim](https://github.com/xero/miasma.nvim) ⭐ 488 | 🐛 5 | 🌐 Vim Script | 📅 2025-07-12 - ***`[TS][LSP]`*** A dark pastel color scheme inspired by the woods. Built using lush and supports Tree-sitter, diagnostics, CMP, Git-Signs, Telescope, Which-key, Lazy, and more.
* [luisiacc/gruvbox-baby](https://github.com/luisiacc/gruvbox-baby) ⭐ 449 | 🐛 8 | 🌐 Lua | 📅 2024-01-25 - ***`[TS][LSP][Lua]`*** A modern gruvbox theme with full Tree-sitter support.
* [ribru17/bamboo.nvim](https://github.com/ribru17/bamboo.nvim) ⭐ 444 | 🐛 2 | 🌐 Lua | 📅 2025-11-25 - ***`[TS][LSP][Lua]`*** A warm green theme.
* [ramojus/mellifluous.nvim](https://github.com/ramojus/mellifluous.nvim) ⭐ 438 | 🐛 3 | 🌐 Lua | 📅 2026-01-22 - ***`[TS][LSP][L/D][Lua]`*** Pleasant and productive colorscheme.
* [uloco/bluloco.nvim](https://github.com/uloco/bluloco.nvim) ⭐ 421 | 🐛 10 | 🌐 Lua | 📅 2026-02-12 - ***`[TS][LSP][L/D][Lua]`*** A fancy and sophisticated colorscheme for night and day coding. Supports LSP, Tree-sitter and all the plugins you love.
* [miikanissi/modus-themes.nvim](https://github.com/miikanissi/modus-themes.nvim) ⭐ 404 | 🐛 5 | 🌐 Lua | 📅 2025-10-05 - ***`[TS][LSP][L/D][Lua]`*** Accessible theme, conforming with the highest standard for color contrast (WCAG AAA).
* [mellow-theme/mellow.nvim](https://github.com/mellow-theme/mellow.nvim) ⭐ 403 | 🐛 1 | 🌐 Lua | 📅 2025-09-02 - ***`[TS][LSP][Lua]`*** A soothing dark color scheme with Tree-sitter support.
* [thesimonho/kanagawa-paper.nvim](https://github.com/thesimonho/kanagawa-paper.nvim) ⭐ 357 | 🐛 2 | 🌐 Lua | 📅 2026-01-28 - ***`[TS][LSP][L/D][Lua]`*** Remixed light and dark Kanagawa colourschemes with muted colors.
* [oxfist/night-owl.nvim](https://github.com/oxfist/night-owl.nvim) ⭐ 336 | 🐛 5 | 🌐 Lua | 📅 2024-09-12 - ***`[TS][LSP][Lua]`*** A [Night Owl colorscheme port from VSCode](https://github.com/sdras/night-owl-vscode-theme) ⭐ 2,934 | 🐛 47 | 📅 2024-12-31 with support for Tree-sitter and semantic tokens.
* [FrenzyExists/aquarium-vim](https://github.com/FrenzyExists/aquarium-vim) ⭐ 313 | 🐛 6 | 🌐 Vim Script | 📅 2024-11-27 - ***`[TS][L/D]`*** A dark, yet vibrant colorscheme.
* [Everblush/nvim](https://github.com/Everblush/nvim) ⭐ 298 | 🐛 4 | 🌐 Lua | 📅 2025-05-18 - ***`[TS][LSP][Lua]`*** A dark, vibrant and beautiful colorscheme written in Lua.
* [maxmx03/fluoromachine.nvim](https://github.com/maxmx03/fluoromachine.nvim) ⭐ 298 | 🐛 1 | 🌐 Lua | 📅 2025-10-21 - ***`[TS][LSP][Lua]`*** Synthwave x Fluoromachine port.
* [gbprod/nord.nvim](https://github.com/gbprod/nord.nvim) ⭐ 290 | 🐛 7 | 🌐 Lua | 📅 2025-10-15 - ***`[TS][LSP][Lua]`*** An arctic, north-bluish clean and elegant theme, based on Nord Palette.
* [Mofiqul/adwaita.nvim](https://github.com/Mofiqul/adwaita.nvim) ⭐ 282 | 🐛 13 | 🌐 Lua | 📅 2026-01-07 - ***`[TS][LSP][L/D][Lua]`*** Colorscheme based on GNOME Adwaita syntax with support for popular plugins.
* [0xstepit/flow.nvim](https://github.com/0xstepit/flow.nvim) ⭐ 280 | 🐛 4 | 🌐 Lua | 📅 2026-02-17 - ***`[TS][L/D][Lua]`*** Carefully designed colors to help focusing during coding plus fluorescent details. Support many plugins and tools.
* [zootedb0t/citruszest.nvim](https://github.com/zootedb0t/citruszest.nvim) ⭐ 247 | 🐛 2 | 🌐 Lua | 📅 2025-06-16 - ***`[TS][LSP][Lua]`*** A colorscheme that features a combination of bright and juicy colors reminiscent of various citrus fruits, with LSP and Tree-sitter support.
* [dasupradyumna/midnight.nvim](https://github.com/dasupradyumna/midnight.nvim) ⭐ 230 | 🐛 2 | 🌐 Lua | 📅 2024-11-01 - ***`[TS][LSP][Lua]`*** A modern black theme with comfortable color contrast for a pleasant visual experience, with LSP and Tree-sitter support.
* [diegoulloao/neofusion.nvim](https://github.com/diegoulloao/neofusion.nvim) ⭐ 227 | 🐛 0 | 🌐 Lua | 📅 2025-03-17 - ***`[TS][LSP][Lua]`*** A theme compatible with Tree-sitter inspired by `gruvbox.nvim`.
* [rockyzhang24/arctic.nvim](https://github.com/rockyzhang24/arctic.nvim) ⭐ 214 | 🐛 2 | 🌐 Lua | 📅 2024-12-18 - ***`[TS][LSP][Lua]`*** A colorscheme ported from VSCode Dark+ theme with the strict and precise color picking for both the editor and UI.
* [cpea2506/one\_monokai.nvim](https://github.com/cpea2506/one_monokai.nvim) ⭐ 188 | 🐛 1 | 🌐 Lua | 📅 2025-09-10 - ***`[TS][LSP][Lua]`*** One Monokai theme written in Lua.
* [polirritmico/monokai-nightasty.nvim](https://github.com/polirritmico/monokai-nightasty.nvim) ⭐ 163 | 🐛 0 | 🌐 Lua | 📅 2025-12-14 - ***`[TS][LSP][L/D][Lua]`*** A dark/light theme based on the Monokai color palette written in Lua, support for LSP, Tree-sitter and lots of plugins.
* [Verf/deepwhite.nvim](https://github.com/Verf/deepwhite.nvim) ⭐ 157 | 🐛 0 | 🌐 Lua | 📅 2026-02-11 - ***`[TS][LSP][Lua]`*** A light colorscheme inspired by [flatwhite-syntax](https://github.com/biletskyy/flatwhite-syntax) ⭐ 187 | 🐛 15 | 🌐 CSS | 📅 2020-04-27 and [elegant-emacs](https://github.com/rougier/elegant-emacs) ⭐ 1,427 | 🐛 9 | 🌐 Emacs Lisp | 📅 2021-11-22.
* [HoNamDuong/hybrid.nvim](https://github.com/HoNamDuong/hybrid.nvim) ⭐ 148 | 🐛 0 | 🌐 Lua | 📅 2026-02-12 - ***`[TS][LSP][Lua]`*** A dark theme written in Lua.
* [nyngwang/nvimgelion](https://github.com/nyngwang/nvimgelion) ⭐ 132 | 🐛 4 | 🌐 Vim Script | 📅 2024-03-07 - ***`[TS]`*** Neon Genesis Evangelion but for Vimmers.
* [metalelf0/jellybeans-nvim](https://github.com/metalelf0/jellybeans-nvim) ⭐ 125 | 🐛 2 | 🌐 Lua | 📅 2025-01-15 - ***`[TS][Lua]`*** A port of jellybeans colorscheme.
* [lalitmee/cobalt2.nvim](https://github.com/lalitmee/cobalt2.nvim) ⭐ 112 | 🐛 0 | 🌐 Lua | 📅 2025-10-30 - ***`[Lua]`*** A port of cobalt2 colorscheme using colorbuddy.
* [phha/zenburn.nvim](https://github.com/phha/zenburn.nvim) ⭐ 110 | 🐛 4 | 🌐 Lua | 📅 2024-07-02 - ***`[TS][Lua]`*** A low-contrast dark colorscheme with support for various plugins.
* [killitar/obscure.nvim](https://github.com/killitar/obscure.nvim) ⭐ 80 | 🐛 4 | 🌐 Lua | 📅 2026-01-27 - ***`[TS][LSP][Lua]`*** A pastel dark colorscheme inspired by the palette Mellow. Support Tree-sitter, LSP *(including semantic tokens)* and lots of plugins.
* [lewpoly/sherbet.nvim](https://github.com/lewpoly/sherbet.nvim) ⭐ 71 | 🐛 0 | 🌐 Lua | 📅 2022-12-17 - ***`[TS][Lua]`*** A soothing colorscheme with support for popular plugins and Tree-sitter.
* [ptdewey/darkearth-nvim](https://github.com/ptdewey/darkearth-nvim) ⭐ 71 | 🐛 0 | 🌐 Fennel | 📅 2026-02-15 - ***`[TS][LSP][Fnl]`*** A dark and earthy colorscheme supporting Tree-sitter and LSP.
* [cryptomilk/nightcity.nvim](https://github.com/cryptomilk/nightcity.nvim) ⭐ 70 | 🐛 0 | 🌐 Lua | 📅 2025-08-11 - ***`[TS][LSP][Lua]`*** A dark colorscheme inspired by Inkpot, Jellybeans, Gruvbox and Tokyonight with LSP support.
* [ldelossa/vimdark](https://github.com/ldelossa/vimdark) ⭐ 69 | 🐛 0 | 🌐 Vim script | 📅 2022-03-20 - ***`[TS][L/D]`*** A minimal Vim theme for night time. Loosely based on vim-monotonic and chrome's dark reader extension. A light theme is included as well for the day time.
* [jpwol/thorn.nvim](https://github.com/jpwol/thorn.nvim) ⭐ 68 | 🐛 0 | 🌐 Lua | 📅 2026-01-30 - ***`[TS][LSP][L/D][Lua]`*** A rich green theme with dark and light options. Supports LSP, transparency, many plugins, and more.
* [2nthony/vitesse.nvim](https://github.com/2nthony/vitesse.nvim) ⭐ 64 | 🐛 1 | 🌐 Lua | 📅 2024-08-17 - ***`[TS][LSP][Lua]`*** Vitesse theme Lua port.
* [samharju/synthweave.nvim](https://github.com/samharju/synthweave.nvim) ⭐ 62 | 🐛 1 | 🌐 Lua | 📅 2025-09-25 - ***`[TS][LSP][Lua]`*** Synthwave '84 colorscheme port.
* [neko-night/nvim](https://github.com/neko-night/nvim) ⭐ 61 | 🐛 0 | 🌐 Lua | 📅 2025-01-25 - ***`[TS][LSP][L/D][Lua]`*** A buffet of colorschemes for every taste and mood.
* [adisen99/apprentice.nvim](https://github.com/adisen99/apprentice.nvim) ⭐ 47 | 🐛 1 | 🌐 Lua | 📅 2026-02-06 - ***`[TS][L/D][Lua]`*** Colorscheme written in Lua based on the [Apprentice](https://github.com/romainl/Apprentice) ⭐ 917 | 🐛 1 | 🌐 Vim Script | 📅 2025-07-14 color palette with Tree-sitter and built-in LSP support.
* [samharju/serene.nvim](https://github.com/samharju/serene.nvim) ⭐ 46 | 🐛 0 | 🌐 Lua | 📅 2024-08-08 - ***`[TS][Lua]`*** A soothing and dark Tree-sitter/LSP-supported theme for relaxing your eyes after using more vibrant colorschemes.
* [uncleTen276/dark\_flat.nvim](https://github.com/uncleTen276/dark_flat.nvim) ⭐ 43 | 🐛 3 | 🌐 Lua | 📅 2024-06-19 - ***`[TS][LSP][Lua]`*** A colorscheme written in Lua ported from Dark Flat iTerm2 theme, with LSP and Tree-sitter support.
* [calind/selenized.nvim](https://github.com/calind/selenized.nvim) ⭐ 28 | 🐛 3 | 🌐 Lua | 📅 2025-08-06 - ***`[TS][LSP][L/D][Lua]`*** Lua port of [selenized](https://github.com/jan-warchol/selenized) ⭐ 888 | 🐛 57 | 🌐 Emacs Lisp | 📅 2025-09-28 with support for Tree-sitter, `nvim-cmp`, GitSigns, and more.
* [titanzero/zephyrium](https://github.com/titanzero/zephyrium) ⭐ 26 | 🐛 0 | 🌐 Lua | 📅 2022-02-20 - ***`[TS][Lua]`*** A zephyr-esque theme, written in Lua, with Tree-sitter support.
* [alexmozaidze/palenight.nvim](https://github.com/alexmozaidze/palenight.nvim) ⭐ 25 | 🐛 0 | 🌐 Fennel | 📅 2026-01-26 - ***`[TS][LSP][Fnl]`*** Palenight colorscheme supporting Tree-sitter, LSP *(including semantic tokens)* and lots of plugins.
* [loganswartz/sunburn.nvim](https://github.com/loganswartz/sunburn.nvim) ⭐ 21 | 🐛 0 | 🌐 Lua | 📅 2025-03-26 - ***`[TS][Lua]`*** A colorscheme sitting somewhere between pastels and solarized, emphasizing readability and hue uniformity above all else.
* [chrsm/paramount-ng.nvim](https://github.com/chrsm/paramount-ng.nvim) ⭐ 20 | 🐛 0 | 🌐 Lua | 📅 2022-06-18 - ***`[TS][Lua]`*** A dark color scheme written using Lush. Tree-sitter supported.
* [qaptoR-nvim/chocolatier.nvim](https://github.com/qaptoR-nvim/chocolatier.nvim) ⭐ 20 | 🐛 0 | 🌐 Lua | 📅 2025-08-02 - ***`[TS][LSP][Lua]`*** An espresso/kimbie inspired chocolatey theme adapted from ellisonleao/gruvbox.nvim theme as a code template.
* [bakageddy/alduin.nvim](https://github.com/bakageddy/alduin.nvim) ⭐ 17 | 🐛 0 | 🌐 Lua | 📅 2024-01-27 - ***`[TS][LSP][Lua]`*** A port of [alduin](https://github.com/AlessandroYorba/alduin) ⭐ 478 | 🐛 9 | 🌐 Vim script | 📅 2022-08-31 theme to Lua with Tree-sitter and semantic highlights support.
* [judaew/ronny.nvim](https://github.com/judaew/ronny.nvim) ⭐ 16 | 🐛 0 | 🌐 Lua | 📅 2025-11-02 - ***`[TS][LSP][Lua]`*** A dark colorscheme, which mostly was inspired by the Monokai originally created by Wimem Hazenberg.
* [sonjiku/yawnc.nvim](https://github.com/sonjiku/yawnc.nvim) ⭐ 15 | 🐛 1 | 🌐 Lua | 📅 2023-06-25 - ***`[TS][LSP][Lua]`*** Theming using pywal, with a Base16 twist.
* [dybdeskarphet/gruvbox-minimal.nvim](https://github.com/dybdeskarphet/gruvbox-minimal.nvim) ⭐ 14 | 🐛 0 | 🌐 Lua | 📅 2026-01-18 - ***`[TS][L/D][Lua]`*** A Gruvbox Material theme conceptually inspired by Alabaster.
* [pmouraguedes/neodarcula.nvim](https://github.com/pmouraguedes/neodarcula.nvim) ⭐ 11 | 🐛 0 | 🌐 Lua | 📅 2026-02-01 - ***`[TS][LSP][Lua]`*** A dark theme with support for transparency, dimming, LSP semantic tokens and more.
* [pebeto/dookie.nvim](https://github.com/pebeto/dookie.nvim) ⭐ 11 | 🐛 0 | 🌐 Lua | 📅 2025-12-25 - ***`[TS][Lua]`*** A color scheme inspired by Plan9's acme editor.
* [samesense/savitsky.nvim](https://github.com/samesense/savitsky.nvim) ⭐ 9 | 🐛 0 | 🌐 Lua | 📅 2026-01-18 - ***`[TS][LSP][L/D][Lua]`*** Curated color palettes inspired by paintings from the Savitsky Museum, built on top of `catppuccin`.
* [ptdewey/monalisa-nvim](https://github.com/ptdewey/monalisa-nvim) ⭐ 9 | 🐛 0 | 🌐 Fennel | 📅 2025-08-20 - ***`[TS][LSP][Lua]`*** A dark and colorful Mona Lisa inspired colorscheme.
* [kevinm6/kurayami.nvim](https://github.com/kevinm6/kurayami.nvim) ⭐ 8 | 🐛 0 | 🌐 Lua | 📅 2025-11-01 - ***`[TS][LSP][Lua]`*** Dark only theme with Tree-sitter support.
* [y3owk1n/base16-pro-max.nvim](https://github.com/y3owk1n/base16-pro-max.nvim) ⭐ 8 | 🐛 0 | 🌐 Lua | 📅 2025-12-14 - ***`[TS][LSP][Lua]`*** Base16 for modern Neovim — not just colors.
* [ntk148v/slack.nvim](https://github.com/ntk148v/slack.nvim) ⭐ 6 | 🐛 1 | 🌐 Lua | 📅 2025-06-12 - ***`[TS][L/D][Lua]`*** A ported Slack colorscheme.
* [sxwpb/halfspace.nvim](https://gitlab.com/sxwpb/halfspace.nvim) - ***`[TS][LSP][Lua]`*** A semi-light colorscheme for minimal eye melting.
* [bartekjaszczak/distinct-nvim](https://gitlab.com/bartekjaszczak/distinct-nvim) - ***`[TS][LSP][L/D][Lua]`*** Theme with distinct syntax colours. Supports Tree-sitter and semantic highlighting. For people who love multi-colour syntax highlighting.
* [bartekjaszczak/luma-nvim](https://gitlab.com/bartekjaszczak/luma-nvim) - ***`[TS][LSP][L/D][Lua]`*** A colorful theme with dark/light modes and adjustable contrast. Supports Tree-sitter and semantic highlighting.
* [bartekjaszczak/finale-nvim](https://gitlab.com/bartekjaszczak/finale-nvim) - ***`[TS][LSP][Lua]`*** A balanced dark theme, blending vivid and pastel colors for a comfortable, high-contrast experience. Supports Tree-sitter and semantic highlighting.
* [m15a/nvim-srcerite](https://codeberg.org/m15a/nvim-srcerite) - ***`[TS][Lua]`*** A colorscheme inspired by [Srcery](https://srcery.sh/), based on `nvim-highlite`.
* [motaz-shokry/gruvbox.nvim](https://gitlab.com/motaz-shokry/gruvbox.nvim) - ***`[TS][L/D][Lua]`*** A new gruvbox theme with a different background color for the hard variant, and comes with 4 variants.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

### Colorscheme Creation

* [nvim-mini/mini.nvim#mini.base16](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-base16.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` with fast implementation of base16 theme for manually supplied palette.
* [nvim-mini/mini.nvim#mini.colors](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-colors.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` to tweak and save any color scheme. Also can animate transition and convert between some color spaces.
* [nvim-mini/mini.nvim#mini.hues](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-hues.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` to generate configurable color scheme. Takes only background and foreground colors as required arguments. Can adjust number of hues for non-base colors, saturation, accent color, plugin integration.
* [rktjmp/lush.nvim](https://github.com/rktjmp/lush.nvim) ⭐ 1,746 | 🐛 13 | 🌐 Lua | 📅 2025-09-01 - Define Neovim themes as a DSL in Lua, with real-time feedback.
* [tjdevries/colorbuddy.nvim](https://github.com/tjdevries/colorbuddy.nvim) ⭐ 756 | 🐛 4 | 🌐 Lua | 📅 2024-05-08 - A colorscheme helper. Written in Lua! Quick and Easy Color Schemes.
* [RRethy/base16-nvim](https://github.com/RRethy/base16-nvim) ⭐ 614 | 🐛 3 | 🌐 Lua | 📅 2026-02-18 - A base16 colorscheme builder. Includes support for Tree-sitter and LSP highlight groups.
* [svermeulen/text-to-colorscheme](https://github.com/svermeulen/text-to-colorscheme) ⭐ 314 | 🐛 6 | 🌐 Lua | 📅 2024-08-14 - Allows the user to generate colorschemes with a text prompt using OpenAI's GPT API.
* [ThemerCorp/themer.lua](https://github.com/ThemerCorp/themer.lua) ⭐ 257 | 🐛 7 | 🌐 Lua | 📅 2023-10-17 - A simple highlighter with a huge collection of colorschemes. It also has ability to create colorschemes for Vim/Neovim and other supported apps (such as `kitty` and `alacritty`).
* [Iron-E/nvim-highlite](https://github.com/Iron-E/nvim-highlite) ⭐ 246 | 🐛 1 | 🌐 Lua | 📅 2026-02-17 - A colorscheme generator that is "lite" on logic for the developer.
* [norcalli/nvim-base16.lua](https://github.com/norcalli/nvim-base16.lua) ⭐ 79 | 🐛 2 | 🌐 Lua | 📅 2023-04-11 - Programmatic Lua library for setting base16 themes.
* [loganswartz/polychrome.nvim](https://github.com/loganswartz/polychrome.nvim) ⭐ 26 | 🐛 0 | 🌐 Lua | 📅 2025-01-26 - A colorscheme micro-framework, with support for specifying colors directly in many different formats (sRGB, HSL, Oklab, XYZ and more, with intelligent chroma clipping), live editing preview, and a simple DSL.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

### Colorscheme Switchers

* [f-person/auto-dark-mode.nvim](https://github.com/f-person/auto-dark-mode.nvim) ⭐ 474 | 🐛 12 | 🌐 Lua | 📅 2025-08-03 - Follow the system appearance on macOS.
* [zaldih/themery.nvim](https://github.com/zaldih/themery.nvim) ⭐ 356 | 🐛 18 | 🌐 Lua | 📅 2025-01-01 - A new way to change the colorscheme on the fly like in VSCode.
* [LmanTW/themify.nvim](https://github.com/LmanTW/themify.nvim/tree/main) ⭐ 59 | 🐛 1 | 🌐 Lua | 📅 2025-05-13 - A lightweight colorscheme manager and switcher inspired by Themery.nvim and Lazy.nvim.
* [CWood-sdf/pineapple](https://github.com/CWood-sdf/pineapple) ⭐ 57 | 🐛 0 | 🌐 Lua | 📅 2026-02-08 - Install any colorscheme in your config without leaving your terminal. Collects every colorscheme on the internet and allows you to preview them all before installing.
* [linrongbin16/colorbox.nvim](https://github.com/linrongbin16/colorbox.nvim) ⭐ 46 | 🐛 0 | 🌐 Lua | 📅 2026-02-04 - Load all the ultra colorschemes into your Neovim player.
* [4e554c4c/darkman.nvim](https://github.com/4e554c4c/darkman.nvim) ⭐ 40 | 🐛 3 | 🌐 Go | 📅 2025-04-06 - Follow the system dark-mode setting on Linux.
* [Erl-koenig/theme-hub.nvim](https://github.com/Erl-koenig/theme-hub.nvim) ⭐ 23 | 🐛 0 | 🌐 Lua | 📅 2025-10-19 - Manage and install colorschemes via telescope-pickers.
* [itsfernn/auto-gnome-theme.nvim](https://github.com/itsfernn/auto-gnome-theme.nvim) ⭐ 13 | 🐛 0 | 🌐 Lua | 📅 2025-12-02 - Fast colorscheme switcher following GNOME system's light/dark mode (based on `gsetting monitor`).
* [flashcodes-themayankjha/fkthemes.nvim](https://github.com/flashcodes-themayankjha/fkthemes.nvim) ⭐ 10 | 🐛 1 | 🌐 Lua | 📅 2025-11-14 - A fast, lightweight and powerful theme switcher written in Lua.
* [DrKJeff16/which-colorscheme.nvim](https://github.com/DrKJeff16/which-colorscheme.nvim) ⭐ 7 | 🐛 0 | 🌐 Lua | 📅 2026-02-16 - Cycle between colorschemes using either custom or autogenerated `which-key.nvim` bindings.
* [BrunoCiccarino/gardenal](https://github.com/BrunoCiccarino/gardenal) ⭐ 5 | 🐛 0 | 🌐 Vim Script | 📅 2024-10-31 - Gardenal is a theme switcher, which allows the user to create keyboard shortcuts to switch between themes with one click.
* [nishu-murmu/ThemeSwitch.nvim](https://github.com/nishu-murmu/ThemeSwitch.nvim) ⭐ 4 | 🐛 0 | 🌐 Lua | 📅 2025-06-26 - Light weight color scheme switcher.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Bars and Lines

* [SmiteshP/nvim-navic](https://github.com/SmiteshP/nvim-navic) ⭐ 1,635 | 🐛 28 | 🌐 Lua | 📅 2025-12-29 - A simple statusline/winbar component that uses LSP to show your current code context.
* [Bekaboo/dropbar.nvim](https://github.com/Bekaboo/dropbar.nvim) ⭐ 1,499 | 🐛 9 | 🌐 Lua | 📅 2025-10-05 - IDE-like breadcrumbs, out of the box.
* [utilyre/barbecue.nvim](https://github.com/utilyre/barbecue.nvim) ⚠️ Archived - A VSCode like winbar.
* [luukvbaal/statuscol.nvim](https://github.com/luukvbaal/statuscol.nvim) ⭐ 599 | 🐛 9 | 🌐 Lua | 📅 2025-06-02 - Configurable 'statuscolumn' with built-in segments and click handlers.
* [m4xshen/smartcolumn.nvim](https://github.com/m4xshen/smartcolumn.nvim) ⭐ 358 | 🐛 2 | 🌐 Lua | 📅 2025-07-21 - Hide your colorcolumn when unneeded.
* [Bekaboo/deadcolumn.nvim](https://github.com/Bekaboo/deadcolumn.nvim) ⭐ 342 | 🐛 2 | 🌐 Lua | 📅 2025-09-04 - Shows your colorcolumn dynamically.
* [ecthelionvi/NeoColumn.nvim](https://github.com/ecthelionvi/NeoColumn.nvim) ⚠️ Archived - Toggleable colorcolumn highlighting specific characters.
* [OXY2DEV/bars.nvim](https://github.com/OXY2DEV/bars.nvim) ⭐ 91 | 🐛 1 | 🌐 Lua | 📅 2026-02-17 - A starting point/guide for creating custom statusline, statuscolumn, tabline and winbar.
* [mawkler/hml.nvim](https://github.com/mawkler/hml.nvim) ⭐ 32 | 🐛 0 | 🌐 Lua | 📅 2024-11-21 - Adds `H`/`M`/`L` indicators to your line numbers.
* [neur1n/noline.nvim](https://github.com/neur1n/noline.nvim) ⭐ 1 | 🐛 0 | 🌐 Lua | 📅 2025-07-11 - Fully customizable bars and lines components with no presets nor constraints.

### Statusline

* [nvim-mini/mini.nvim#mini.statusline](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-statusline.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` for minimal and fast statusline. Supports content change depending on window width.
* [nvim-lualine/lualine.nvim](https://github.com/nvim-lualine/lualine.nvim) ⭐ 7,740 | 🐛 267 | 🌐 Lua | 📅 2025-11-23 - Easily configurable, blazingly fast statusline.
* [rebelot/heirline.nvim](https://github.com/rebelot/heirline.nvim) ⭐ 1,240 | 🐛 28 | 🌐 Lua | 📅 2025-05-23 - A no-nonsense statusline designed around recursive inheritance to be exceptionally fast and versatile.
* [b0o/incline.nvim](https://github.com/b0o/incline.nvim) ⭐ 1,011 | 🐛 9 | 🌐 Lua | 📅 2025-12-18 - Lightweight floating statuslines, intended for use with Neovim's new global statusline.
* [windwp/windline.nvim](https://github.com/windwp/windline.nvim) ⭐ 516 | 🐛 0 | 🌐 Lua | 📅 2025-10-22 - The next generation statusline. Animation statusline.
* [tamton-aquib/staline.nvim](https://github.com/tamton-aquib/staline.nvim) ⭐ 394 | 🐛 7 | 🌐 Lua | 📅 2024-06-02 - A modern lightweight statusline in Lua. Mainly uses unicode symbols for showing info.
* [tjdevries/express\_line.nvim](https://github.com/tjdevries/express_line.nvim) ⭐ 315 | 🐛 18 | 🌐 Lua | 📅 2024-05-17 - Supports co-routines, functions and jobs.
* [adelarsq/neoline.vim](https://github.com/adelarsq/neoline.vim) ⭐ 258 | 🐛 13 | 🌐 Lua | 📅 2024-04-25 - A light statusline/tabline plugin using Lua.
* [beauwilliams/statusline.lua](https://github.com/beauwilliams/statusline.lua) ⭐ 256 | 🐛 5 | 🌐 Lua | 📅 2025-04-30 - A zero-config minimal statusline written in Lua featuring awesome integrations and blazing speed!
* [MunifTanjim/nougat.nvim](https://github.com/MunifTanjim/nougat.nvim) ⭐ 202 | 🐛 3 | 🌐 Lua | 📅 2024-01-07 - Hyperextensible statusline/tabline/winbar.
* [ojroques/nvim-hardline](https://github.com/ojroques/nvim-hardline) ⭐ 200 | 🐛 2 | 🌐 Lua | 📅 2023-12-27 - A statusline / bufferline inspired by [vim-airline](https://github.com/vim-airline/vim-airline) ⭐ 17,943 | 🐛 50 | 🌐 Vim Script | 📅 2025-12-23 that aims to be as light and simple as possible.
* [NTBBloodbath/galaxyline.nvim](https://github.com/NTBBloodbath/galaxyline.nvim) ⭐ 167 | 🐛 13 | 🌐 Lua | 📅 2022-05-16 - A light-weight and super fast statusline plugin written in Lua.
* [Zeioth/heirline-components.nvim](https://github.com/Zeioth/heirline-components.nvim) ⭐ 150 | 🐛 3 | 🌐 Lua | 📅 2025-11-17 - 30+ `heirline.nvim` components to be used out of the box to create the perfect user interface.
* [sschleemilch/slimline.nvim](https://github.com/sschleemilch/slimline.nvim) ⭐ 121 | 🐛 3 | 🌐 Lua | 📅 2026-02-16 - A slim, minimal and opinionated Lua statusline.
* [sontungexpt/witch-line](https://github.com/sontungexpt/witch-line) ⭐ 58 | 🐛 1 | 🌐 Lua | 📅 2026-01-22 - A blazing fast statusline based on reference concept.
* [yaocccc/nvim-lines.lua](https://github.com/yaocccc/nvim-lines.lua) ⭐ 39 | 🐛 0 | 🌐 Lua | 📅 2023-04-06 - A fast, light, customizable statusline and tabline (buffers).
* [konapun/vacuumline.nvim](https://github.com/konapun/vacuumline.nvim) ⭐ 30 | 🐛 1 | 🌐 Lua | 📅 2023-02-18 - A galaxyline configuration inspired by airline.
* [mikesmithgh/git-prompt-string-lualine.nvim](https://github.com/mikesmithgh/git-prompt-string-lualine.nvim) ⭐ 26 | 🐛 1 | 🌐 Lua | 📅 2024-04-22 - Add git-prompt-string to your statusline.
* [Mr-LLLLL/lualine-ext.nvim](https://github.com/Mr-LLLLL/lualine-ext.nvim) ⭐ 20 | 🐛 0 | 🌐 Lua | 📅 2025-10-21 - Show more information on lualine.

### Tabline

* [nvim-mini/mini.nvim#mini.tabline](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-tabline.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` for minimal tabline showing listed buffers in case of one tab and falling back to default otherwise.
* [akinsho/bufferline.nvim](https://github.com/akinsho/bufferline.nvim) ⭐ 4,235 | 🐛 99 | 🌐 Lua | 📅 2025-01-14 - A snazzy bufferline built using Lua.
* [romgrk/barbar.nvim](https://github.com/romgrk/barbar.nvim) ⭐ 2,645 | 🐛 32 | 🌐 Lua | 📅 2025-12-02 - A tabline with re-orderable, auto-sizing, clickable tabs, icons, nice highlighting, sort-by commands and a magic jump-to-buffer mode.
* [nanozuki/tabby.nvim](https://github.com/nanozuki/tabby.nvim) ⭐ 730 | 🐛 6 | 🌐 Lua | 📅 2026-01-07 - A minimal, configurable tabline that allows using tabs as workspace multiplexers.
* [willothy/nvim-cokeline](https://github.com/willothy/nvim-cokeline) ⭐ 617 | 🐛 13 | 🌐 Lua | 📅 2025-01-24 - A bufferline for people with addictive personalities.
* [alvarosevilla95/luatab.nvim](https://github.com/alvarosevilla95/luatab.nvim) ⭐ 206 | 🐛 8 | 🌐 Lua | 📅 2025-03-21 - A simple tabline written in Lua.
* [rafcamlet/tabline-framework.nvim](https://github.com/rafcamlet/tabline-framework.nvim) ⭐ 101 | 🐛 4 | 🌐 Lua | 📅 2023-03-10 - User-friendly framework for building your dream tabline in a few lines of code.
* [crispgm/nvim-tabline](https://github.com/crispgm/nvim-tabline) ⭐ 92 | 🐛 2 | 🌐 Lua | 📅 2024-06-03 - A port of `tabline.vim` written in Lua.
* [tomiis4/BufferTabs.nvim](https://github.com/tomiis4/BufferTabs.nvim) ⭐ 91 | 🐛 0 | 🌐 Lua | 📅 2024-08-11 - Simple and Fancy tabline.
* [johann2357/nvim-smartbufs](https://github.com/johann2357/nvim-smartbufs) ⭐ 53 | 🐛 0 | 🌐 Lua | 📅 2023-01-17 - Smart buffer management.

### Cursorline

* [nvim-mini/mini.nvim#mini.cursorword](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-cursorword.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` for automatic highlighting of word under cursor (displayed after customizable delay).
* [RRethy/vim-illuminate](https://github.com/RRethy/vim-illuminate) ⭐ 2,434 | 🐛 11 | 🌐 Lua | 📅 2025-05-24 - Highlight the word under the cursor with built-in LSP support.
* [ya2s/nvim-cursorline](https://github.com/ya2s/nvim-cursorline) ⭐ 456 | 🐛 7 | 🌐 Lua | 📅 2026-02-14 - Highlights cursor words and lines.
* [mawkler/modicator.nvim](https://github.com/mawkler/modicator.nvim) ⭐ 366 | 🐛 3 | 🌐 Lua | 📅 2025-10-24 - Cursor line number mode indicator. Changes the `CursorLineNr` highlight based on Vim mode.
* [sontungexpt/stcursorword](https://github.com/sontungexpt/stcursorword) ⭐ 81 | 🐛 0 | 🌐 Lua | 📅 2025-11-30 - Highlight the word under the cursor (improved and compact version of `nvim-cursorline`).

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Startup

* [nvim-mini/mini.nvim#mini.starter](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-starter.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` for start screen. Displayed items are fully customizable, item selection can be done using prefix query with instant visual feedback.
* [nvimdev/dashboard-nvim](https://github.com/nvimdev/dashboard-nvim) ⭐ 2,779 | 🐛 73 | 🌐 Lua | 📅 2025-08-31 - A minimalist dashboard, inspired by doom-emacs.
* [goolord/alpha-nvim](https://github.com/goolord/alpha-nvim) ⭐ 2,325 | 🐛 40 | 🌐 Lua | 📅 2026-02-10 - A fast and highly customizable greeter like [vim-startify](https://github.com/mhinz/vim-startify) ⭐ 5,388 | 🐛 80 | 🌐 Vim Script | 📅 2024-01-05/dashboard-nvim.
* [max397574/startup.nvim](https://github.com/max397574/startup.nvim) ⭐ 499 | 🐛 9 | 🌐 Lua | 📅 2024-10-30 - The fully customizable greeter.
* [CWood-sdf/spaceport.nvim](https://github.com/CWood-sdf/spaceport.nvim) ⭐ 144 | 🐛 0 | 🌐 Lua | 📅 2026-01-02 - The start screen that gets you to your projects blazingly fast.
* [TobinPalmer/Tip.nvim](https://github.com/TobinPalmer/Tip.nvim) ⭐ 81 | 🐛 1 | 🌐 Lua | 📅 2024-02-04 - Get a simple tip on startup.
* [mong8se/actually.nvim](https://github.com/mong8se/actually.nvim) ⭐ 63 | 🐛 2 | 🌐 Lua | 📅 2025-10-13 - Load the file you actually meant to load.
* [henriquehbr/nvim-startup.lua](https://sr.ht/~henriquehbr/nvim-startup.lua) - Displays the startup time.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Icon

* [nvim-mini/mini.nvim#mini.icons](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-icons.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` meant as a general icon provider. Uses fixed set of highlight groups. Supports various categories, icon and style customizations, caching for performance. Integrates with built-in filetype matching.
* [nvim-tree/nvim-web-devicons](https://github.com/nvim-tree/nvim-web-devicons) ⭐ 2,610 | 🐛 18 | 🌐 Lua | 📅 2026-02-05 - A Lua fork of [vim-devicons](https://github.com/ryanoasis/vim-devicons) ⭐ 5,791 | 🐛 70 | 🌐 Vim Script | 📅 2024-05-09.
* [2KAbhishek/nerdy.nvim](https://github.com/2KAbhishek/nerdy.nvim/) ⭐ 376 | 🐛 0 | 🌐 Lua | 📅 2026-01-20 - Find and insert the latest nerd font glyphs.
* [stephansama/fzf-nerdfont.nvim](https://github.com/stephansama/fzf-nerdfont.nvim) ⭐ 9 | 🐛 3 | 🌐 Lua | 📅 2026-01-14 - A picker for selecting Nerd Font icons using `fzf-lua`.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Media

* [3rd/image.nvim](https://github.com/3rd/image.nvim) ⭐ 1,877 | 🐛 47 | 🌐 Lua | 📅 2026-02-15 - Add image support through Kitty's graphics protocol or ueberzugpp.
* [edluffy/hologram.nvim](https://github.com/edluffy/hologram.nvim) ⭐ 1,425 | 🐛 29 | 🌐 Lua | 📅 2023-11-15 - A cross platform terminal image viewer. Works on macOS and Linux.
* [HakonHarnes/img-clip.nvim](https://github.com/HakonHarnes/img-clip.nvim) ⭐ 869 | 🐛 10 | 🌐 Lua | 📅 2025-12-19 - Effortlessly embed images into any markup language, like LaTeX, Markdown or Typst.
* [vyfor/cord.nvim](https://github.com/vyfor/cord.nvim) ⭐ 556 | 🐛 0 | 🌐 Lua | 📅 2026-02-17 - Highly extensible Rich Presence for Discord.
* [ekickx/clipboard-image.nvim](https://github.com/ekickx/clipboard-image.nvim) ⭐ 335 | 🐛 10 | 🌐 Lua | 📅 2024-03-19 - Allows pasting images from clipboard.
* [davidgranstrom/scnvim](https://github.com/davidgranstrom/scnvim) ⭐ 256 | 🐛 22 | 🌐 Lua | 📅 2025-10-02 - A frontend for SuperCollider.
* [neo451/feed.nvim](https://github.com/neo451/feed.nvim) ⭐ 197 | 🐛 9 | 🌐 Lua | 📅 2025-12-15 - Web feed reader written in Lua (RSS, Atom, JSON feed).
* [adelarsq/image\_preview.nvim](https://github.com/adelarsq/image_preview.nvim) ⭐ 190 | 🐛 11 | 🌐 Lua | 📅 2024-10-22 - Image preview based on terminal's Image Protocol support.
* [Chaitanyabsrip/present.nvim](https://github.com/Chaitanyabsprip/present.nvim) ⭐ 157 | 🐛 0 | 🌐 Lua | 📅 2025-03-03 - A Presentation plugin written in Lua.
* [askfiy/nvim-picgo](https://github.com/askfiy/nvim-picgo) ⭐ 67 | 🐛 3 | 🌐 Lua | 📅 2025-05-01 - Allows you to upload images to the image bed, allowing viewing images from anywhere on the internet.
* [niuiic/code-shot.nvim](https://github.com/niuiic/code-shot.nvim) ⭐ 65 | 🐛 0 | 🌐 Lua | 📅 2025-01-04 - Take a picture of the code.
* [AntonVanAssche/music-controls.nvim](https://github.com/AntonVanAssche/music-controls.nvim) ⭐ 36 | 🐛 0 | 🌐 Lua | 📅 2025-09-29 - Quickly control your favorite music player (Spotify, VLC, and more).
* [iamt4nk/smm.nvim](https://github.com/iamt4nk/smm.nvim) ⭐ 30 | 🐛 0 | 🌐 Lua | 📅 2025-10-22 - Small TUI that allows for controlling Spotify playback.
* [melMass/echo.nvim](https://github.com/melMass/echo.nvim) ⭐ 14 | 🐛 1 | 🌐 Rust | 📅 2025-11-26 - Seamless sound integration for your editing workflow.
* [niuiic/cp-image.nvim](https://github.com/niuiic/cp-image.nvim) ⭐ 10 | 🐛 0 | 🌐 Lua | 📅 2024-05-11 - Paste image from clipboard and insert the reference code.
* [ricmonmol/nvim-music-player](https://github.com/ricmonmol/nvim-music-player) ⭐ 4 | 🐛 2 | 🌐 Python | 📅 2026-01-20 - A simple music player powered by `mpv`, written in Python, including a Telescope browser.
* [\~elisoli/nekovim](https://git.sr.ht/~elisoli/nekovim) - Flexible Discord rich presence.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Note Taking

* [nvim-neorg/neorg](https://github.com/nvim-neorg/neorg) ⭐ 7,218 | 🐛 219 | 🌐 Lua | 📅 2026-02-01 - Modernity meets insane extensibility. The future of organizing your life.
* [nvim-orgmode/orgmode](https://github.com/nvim-orgmode/orgmode) ⭐ 3,675 | 🐛 135 | 🌐 Lua | 📅 2026-02-11 - Org-mode clone written in Lua.
* [nvim-telekasten/telekasten.nvim](https://github.com/nvim-telekasten/telekasten.nvim) ⭐ 1,634 | 🐛 66 | 🌐 Lua | 📅 2026-02-03 - Work with a text-based, Markdown zettelkasten / wiki and mix it with a journal, based on telescope.nvim.
* [obsidian-nvim/obsidian.nvim](https://github.com/obsidian-nvim/obsidian.nvim) ⭐ 1,550 | 🐛 67 | 🌐 Lua | 📅 2026-02-16 - Plugin for Obsidian, written in Lua.
* [jbyuki/venn.nvim](https://github.com/jbyuki/venn.nvim) ⭐ 1,150 | 🐛 4 | 🌐 Lua | 📅 2024-08-16 - Draw ASCII diagrams.
* [zk-org/zk-nvim](https://github.com/zk-org/zk-nvim) ⭐ 793 | 🐛 4 | 🌐 Lua | 📅 2026-01-24 -  Provides integration with `zk`, a plain text note-taking assistant.
* [jakewvincent/mkdnflow.nvim](https://github.com/jakewvincent/mkdnflow.nvim) ⭐ 776 | 🐛 12 | 🌐 Lua | 📅 2026-02-18 - Fluent Markdown notebook navigation and management (create links, follow links, create and manage to-do lists, reference bib files, and more).
* [jbyuki/nabla.nvim](https://github.com/jbyuki/nabla.nvim) ⭐ 730 | 🐛 24 | 🌐 Lua | 📅 2025-04-21 - Take your scientific notes.
* [bngarren/checkmate.nvim](https://github.com/bngarren/checkmate.nvim) ⭐ 351 | 🐛 7 | 🌐 Lua | 📅 2025-11-15 - A full-featured Markdown-based TODO plugin.
* [serenevoid/kiwi.nvim](https://github.com/serenevoid/kiwi.nvim) ⭐ 245 | 🐛 10 | 🌐 Lua | 📅 2025-07-07 - A stripped down VimWiki with necessary features.
* [jghauser/papis.nvim](https://github.com/jghauser/papis.nvim) ⭐ 175 | 🐛 10 | 🌐 Lua | 📅 2025-11-19 - Manage your bibliography from within your favourite editor.
* [backdround/global-note.nvim](https://github.com/backdround/global-note.nvim) ⭐ 143 | 🐛 4 | 🌐 Lua | 📅 2024-02-14 - One global note in a floating window.
* [echaya/neowiki.nvim](https://github.com/echaya/neowiki.nvim) ⭐ 125 | 🐛 1 | 🌐 Lua | 📅 2026-01-30 - The modern vimwiki successor offering a minimal, intuitive workflow out of the box for note-taking and Getting Things Done (GTD).
* [nfrid/due.nvim](https://github.com/nfrid/due.nvim) ⭐ 118 | 🐛 0 | 🌐 Lua | 📅 2023-09-04 - Displays due for a date string as a virtual text.
* [chrsm/impulse.nvim](https://github.com/chrsm/impulse.nvim) ⭐ 100 | 🐛 3 | 🌐 MoonScript | 📅 2022-06-26 - Read Notion.so notes.
* [2KAbhishek/tdo.nvim](https://github.com/2KAbhishek/tdo.nvim) ⭐ 97 | 🐛 0 | 🌐 Lua | 📅 2025-11-20 - Fast and simple note taking.
* [0styx0/abbreinder.nvim](https://github.com/0styx0/abbreinder.nvim) ⭐ 91 | 🐛 0 | 🌐 Lua | 📅 2022-06-30 - Abbreviation reminders.
* [apdot/doodle](https://github.com/apdot/doodle) ⭐ 86 | 🐛 0 | 🌐 Lua | 📅 2025-10-26 - A developer-centric knowledge base with project/branch scoped notes, bi-directional linking, note-tagging, graph-view, telescope integration, and Git synchronization.
* [IlyasYOY/obs.nvim](https://github.com/IlyasYOY/obs.nvim) ⭐ 84 | 🐛 6 | 🌐 Lua | 📅 2026-02-01 - Your Obsidian notes at the speed of thought.
* [jameswolensky/marker-groups.nvim](https://github.com/jameswolensky/marker-groups.nvim) ⭐ 56 | 🐛 3 | 🌐 Lua | 📅 2025-09-04 - Take persistent code notes without modifying code.
* [iwe-org/iwe.nvim](https://github.com/iwe-org/iwe.nvim) ⭐ 40 | 🐛 0 | 🌐 Lua | 📅 2026-01-25 - Integration with `IWE`, an LSP designed for Markdown-based knowledge management and note-taking workflows.
* [lfilho/note2cal.nvim](https://github.com/lfilho/note2cal.nvim) ⭐ 26 | 🐛 1 | 🌐 Lua | 📅 2025-10-27 - Create calendar events from Markdown notes (macOS only).
* [Ostralyan/scribe.nvim](https://github.com/Ostralyan/scribe.nvim) ⭐ 25 | 🐛 0 | 🌐 Lua | 📅 2023-02-02 - Take notes, easily.
* [y3owk1n/dotmd.nvim](https://github.com/y3owk1n/dotmd.nvim) ⭐ 23 | 🐛 0 | 🌐 Lua | 📅 2025-12-14 - Managing notes, TODO's, journal entries, and your inbox, all with Markdown.
* [niuiic/todo.nvim](https://github.com/niuiic/todo.nvim) ⭐ 18 | 🐛 0 | 🌐 Lua | 📅 2024-11-05 - Simple but powerful TODO manager based on text.
* [athar-qadri/scratchpad.nvim](https://github.com/athar-qadri/scratchpad.nvim) ⭐ 13 | 🐛 0 | 🌐 Lua | 📅 2025-03-09 - Effortlessly manage scratchpads within your favorite editor.
* [flashcodes-themayankjha/Fknotes.nvim](https://github.com/flashcodes-themayankjha/Fknotes.nvim) ⭐ 12 | 🐛 0 | 🌐 Lua | 📅 2025-10-16 - Take notes, TODOs from anywhere inside your project, search all TODOs, get reminders and more.
* [slugbyte/whip.nvim](http://github.com/slugbyte/whip.nvim) ⭐ 12 | 🐛 0 | 🌐 Lua | 📅 2025-04-03 - A super fast minimal scratchpad management plugin, biew biew biew.
* [happyeric77/joplin.nvim](https://github.com/happyeric77/joplin.nvim) ⭐ 8 | 🐛 0 | 🌐 Lua | 📅 2025-09-07 - Joplin notes utilities: tree browser, search, open, and Telescope integration.
* [ymich9963/mdnotes.nvim](https://github.com/ymich9963/mdnotes.nvim) ⭐ 6 | 🐛 2 | 🌐 Lua | 📅 2026-02-17 - Simple and improved Markdown note taking.
* [nbeversl/urtext\_neovim](https://github.com/nbeversl/urtext_neovim) ⭐ 4 | 🐛 0 | 🌐 Python | 📅 2025-12-23 - An implementation of Urtext.
* [stikypiston/studytools.nvim](https://github.com/stikypiston/studytools.nvim) ⭐ 4 | 🐛 0 | 🌐 Lua | 📅 2026-02-17 - Various utilities to enhance the studying and note-taking experience.
* [carloscalla/notepad.nvim](https://github.com/carloscalla/notepad.nvim) ⭐ 2 | 🐛 0 | 🌐 Lua | 📅 2026-01-27 - Quick note-taking in Markdown with both repo-specific and global notepad support.
* [losch/ztl](https://codeberg.org/losch/ztl) - A fast static note generator in a single binary with everything built-in.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Utility

* [jbyuki/instant.nvim](https://github.com/jbyuki/instant.nvim) ⭐ 1,410 | 🐛 9 | 🌐 Lua | 📅 2022-12-31 - A collaborative editing plugin written in Lua with no dependencies.
* [mistricky/codesnap.nvim](https://github.com/mistricky/codesnap.nvim) ⭐ 918 | 🐛 29 | 🌐 Lua | 📅 2026-01-31 - Snapshot plugin with rich features that can make pretty code snapshots.
* [code-biscuits/nvim-biscuits](https://github.com/code-biscuits/nvim-biscuits) ⭐ 324 | 🐛 8 | 🌐 Lua | 📅 2025-10-08 - A port of Assorted Biscuits. Ends up with more supported languages too.
* [axieax/urlview.nvim](https://github.com/axieax/urlview.nvim) ⭐ 271 | 🐛 7 | 🌐 Lua | 📅 2025-11-30 - Browse all URLs in the current buffer.
* [LintaoAmons/scratch.nvim](https://github.com/LintaoAmons/scratch.nvim) ⭐ 271 | 🐛 12 | 🌐 Lua | 📅 2025-09-08 - Create and manage scratch files.
* [crusj/bookmarks.nvim](https://github.com/crusj/bookmarks.nvim) ⭐ 245 | 🐛 10 | 🌐 Lua | 📅 2024-07-12 - Remember file locations and sort by time and frequency.
* [chrisgrieser/nvim-genghis](https://github.com/chrisgrieser/nvim-genghis) ⭐ 217 | 🐛 1 | 🌐 Lua | 📅 2026-02-06 - Convenience file operations, written in Lua.
* [subnut/nvim-ghost.nvim](https://github.com/subnut/nvim-ghost.nvim) ⭐ 194 | 🐛 12 | 🌐 Python | 📅 2025-09-08 - GhostText support with zero dependencies.
* [philosofonusus/ecolog.nvim](https://github.com/philosofonusus/ecolog.nvim) ⭐ 171 | 🐛 3 | 🌐 Lua | 📅 2026-02-02 - Sophisticated all-in-one toolkit to work with `.env` files and environment variables.
* [Owen-Dechow/videre.nvim](https://github.com/Owen-Dechow/videre.nvim) ⭐ 136 | 🐛 1 | 🌐 Lua | 📅 2026-01-31 - Explore JSON, YAML, and TOML files as nested unit/node-based graphical representations.
* [mluders/comfy-line-numbers.nvim](https://github.com/mluders/comfy-line-numbers.nvim) ⭐ 113 | 🐛 7 | 🌐 Lua | 📅 2026-01-26 - Limits relative numbers to only show left-hand digits on the keyboard.
* [sontungexpt/url-open](https://github.com/sontungexpt/url-open) ⭐ 106 | 🐛 9 | 🌐 Lua | 📅 2025-10-29 - Open URLs under the cursor and create highlight effects for them.
* [rktjmp/paperplanes.nvim](https://github.com/rktjmp/paperplanes.nvim) ⭐ 99 | 🐛 0 | 🌐 Fennel | 📅 2025-07-14 - Post selections or buffers to online paste bins.
* [ysmb-wtsg/in-and-out.nvim](https://github.com/ysmb-wtsg/in-and-out.nvim) ⭐ 83 | 🐛 0 | 🌐 Lua | 📅 2025-08-16 - Quick navigation in and out of surrounding characters.
* [gpanders/nvim-moonwalk](https://github.com/gpanders/nvim-moonwalk) ⭐ 78 | 🐛 0 | 🌐 Lua | 📅 2022-04-12 - Use any language that compiles to Lua anywhere in your Neovim configuration.
* [y3owk1n/time-machine.nvim](https://github.com/y3owk1n/time-machine.nvim) ⭐ 70 | 🐛 0 | 🌐 Lua | 📅 2025-12-14 - Take control of your edit history with an interactive timeline, diff previews, taggings, live reloading trees and cleanup functions.
* [doctorfree/cheatsheet.nvim](https://github.com/doctorfree/cheatsheet.nvim) ⭐ 67 | 🐛 6 | 🌐 Lua | 📅 2025-10-31 - Searchable cheatsheet.
* [figsoda/nix-develop.nvim](https://github.com/figsoda/nix-develop.nvim) ⭐ 64 | 🐛 0 | 🌐 Lua | 📅 2026-01-29 - Run `nix develop` without restarting Neovim.
* [josephburgess/nvumi](https://github.com/josephburgess/nvumi) ⭐ 57 | 🐛 0 | 🌐 Lua | 📅 2025-10-31 - Natural language calculator in a scratch buffer.
* [ellisonleao/dotenv.nvim](https://github.com/ellisonleao/dotenv.nvim) ⭐ 55 | 🐛 3 | 🌐 Lua | 📅 2025-03-27 - Minimalist `.env` support.
* [redoxahmii/json-to-types.nvim](https://github.com/redoxahmii/json-to-types.nvim) ⭐ 54 | 🐛 2 | 🌐 Lua | 📅 2025-03-06 - Convert JSON objects to type definitions for multiple languages.
* [MisanthropicBit/decipher.nvim](https://github.com/MisanthropicBit/decipher.nvim) ⭐ 43 | 🐛 5 | 🌐 Lua | 📅 2026-02-01 - Encode and decode text using various codecs such as base64.
* [necrom4/calcium.nvim](https://github.com/necrom4/calcium.nvim) ⭐ 42 | 🐛 0 | 🌐 Lua | 📅 2025-12-27 - A powerful [`lua-lib-math`](https://www.lua.org/pil/18.html) in-buffer calculator with visual mode, functions and variable support.
* [terje/simctl.nvim](https://github.com/terje/simctl.nvim) ⭐ 40 | 🐛 0 | 🌐 Lua | 📅 2024-12-15 - Interact with iOS Simulators.
* [zeybek/camouflage.nvim](https://github.com/zeybek/camouflage.nvim) ⭐ 36 | 🐛 1 | 🌐 Lua | 📅 2026-02-14 - Hide sensitive values in configuration files during screen sharing by visually masking secrets in `.env`, `.json`, `.yaml`, `.toml`, and `.properties` files.
* [0xJohnnyboy/scretch.nvim](https://github.com/0xJohnnyboy/scretch.nvim) ⭐ 34 | 🐛 0 | 🌐 Lua | 📅 2025-09-11 - Create and manage scratch files, scratch templates, with picker integrations.
* [yutkat/confirm-quit.nvim](https://github.com/yutkat/confirm-quit.nvim) ⭐ 34 | 🐛 0 | 🌐 Lua | 📅 2025-04-25 - Confirm before quitting.
* [tenxsoydev/nx.nvim](https://github.com/tenxsoydev/nx.nvim) ⭐ 33 | 🐛 5 | 🌐 Lua | 📅 2024-10-17 - Neovim API utility wrapper for more convenience with Lua keymaps, highlights, autocommands and options.
* [ovk/endec.nvim](https://github.com/ovk/endec.nvim) ⭐ 32 | 🐛 1 | 🌐 Lua | 📅 2025-04-07 - Encode, decode and re-encode text using Base64, Base64URL and URL (percent) encodings.
* [AlejandroSuero/freeze-code.nvim](https://github.com/AlejandroSuero/freeze-code.nvim) ⭐ 31 | 🐛 2 | 🌐 Lua | 📅 2025-03-15 - Code screenshot plugin that makes use of [freeze](https://github.com/charmbracelet/freeze) ⭐ 4,348 | 🐛 67 | 🌐 Go | 📅 2026-02-09 inside the editor.
* [aPeoplesCalendar/apc.nvim](https://github.com/aPeoplesCalendar/apc.nvim) ⭐ 23 | 🐛 2 | 🌐 Lua | 📅 2024-06-18 - "On this day" style calendar, which provides information about worldwide history of working class movements and liberation struggles.
* [linrongbin16/gentags.nvim](https://github.com/linrongbin16/gentags.nvim) ⭐ 23 | 🐛 1 | 🌐 Lua | 📅 2025-08-20 - The tags generator/management for old school vimers.
* [bgaillard/readonly.nvim](https://github.com/bgaillard/readonly.nvim) ⭐ 22 | 🐛 0 | 🌐 Lua | 📅 2025-07-11 - Secure edition of files containing sensible / secret information, passwords, API keys, SSH keys, etc.
* [gaborvecsei/cryptoprice.nvim](https://github.com/gaborvecsei/cryptoprice.nvim) ⭐ 22 | 🐛 0 | 🌐 Lua | 📅 2025-11-03 - Check the price of the defined cryptocurrencies.
* [piersolenski/brewfile.nvim](https://github.com/piersolenski/brewfile.nvim) ⭐ 18 | 🐛 0 | 🌐 Lua | 📅 2025-11-03 - Manage your [Homebrew](https://brew.sh/) [Brewfile](https://docs.brew.sh/Brew-Bundle-and-Brewfile).
* [johannww/tts.nvim](https://github.com/johannww/tts.nvim) ⭐ 18 | 🐛 0 | 🌐 Lua | 📅 2025-11-26 - Text to speech tool based on the Microsoft Edge online services.
* [ragnarok22/whereami.nvim](https://github.com/ragnarok22/whereami.nvim) ⭐ 17 | 🐛 0 | 🌐 Lua | 📅 2025-08-21 - Test your VPN by getting you current location.
* [athar-qadri/weather.nvim](https://github.com/athar-qadri/weather.nvim) ⭐ 13 | 🐛 0 | 🌐 Lua | 📅 2025-07-27 - Realtime weather and earthquake alerts with support for lualine integration (no API key required).
* [theKnightsOfRohan/hexer.nvim](https://github.com/theKnightsOfRohan/hexer.nvim) ⭐ 11 | 🐛 0 | 🌐 Lua | 📅 2025-11-06 - Easily convert between binary representations without a conversion table.
* [Zeioth/distroupdate.nvim](https://github.com/Zeioth/distroupdate.nvim) ⭐ 10 | 🐛 0 | 🌐 Lua | 📅 2025-08-11 - Distro agnostic updater to get the latest changes from the Git repository of your config.
* [glyccogen/imprint.nvim](https://github.com/glyccogen/imprint.nvim) ⭐ 10 | 🐛 0 | 🌐 Lua | 📅 2026-02-15 - Take WYSIWYG screenshots of your code via Playwright and headless Chromium, preserving your colorscheme and highlights.
* [wsdjeg/mru.nvim](https://github.com/wsdjeg/mru.nvim) ⭐ 9 | 🐛 1 | 🌐 Lua | 📅 2026-01-25 - Manage and display your Most Recently Used (MRU) files.
* [wsdjeg/ctags.nvim](https://github.com/wsdjeg/ctags.nvim) ⭐ 8 | 🐛 1 | 🌐 Lua | 📅 2025-12-03 - Generate tags files and update tags option automatically.
* [leo-alvarenga/quoth.nvim](https://github.com/leo-alvarenga/quoth.nvim) ⭐ 5 | 🐛 0 | 🌐 Lua | 📅 2025-12-17 - A lightweight, configurable random quote provider with lazy loading, custom tables, and filters.
* [stikypiston/cheaty.nvim](https://github.com/stikypiston/cheaty.nvim) ⭐ 5 | 🐛 1 | 🌐 Lua | 📅 2026-02-17 - A simple, configurable cheatsheet.
* [StefanBartl/color\_my\_ascii.nvim](https://github.com/StefanBartl/color_my_ascii.nvim) ⭐ 4 | 🐛 0 | 🌐 Lua | 📅 2026-01-12 - Colorful highlighting of ASCII art in Markdown code blocks.
* [iquzart/toggleword.nvim](https://github.com/iquzart/toggleword.nvim) ⭐ 4 | 🐛 0 | 🌐 Lua | 📅 2025-07-25 - Toggle between common code keywords under the cursor such as true ⇄ false, on ⇄ off, enabled ⇄ disabled, and dev ⇄ prod.
* [cxwx/lazyUrlUpdate.nvim](https://github.com/cxwx/lazyUrlUpdate.nvim) ⭐ 3 | 🐛 0 | 🌐 Lua | 📅 2026-01-03 - Update plugin under cursor by `lazy.nvim`.
* [penaz91/MiniDYM](https://github.com/Penaz91/MiniDYM) ⭐ 3 | 🐛 0 | 🌐 Lua | 📅 2026-01-17 - A very small "Did you mean" plugin, suggesting files the user might have wanted to open instead of creating a new one.
* [mahyarmirrashed/famous-quotes.nvim](https://github.com/mahyarmirrashed/famous-quotes.nvim) ⭐ 3 | 🐛 0 | 🌐 Lua | 📅 2025-07-01 - Get famous quotes from history to display on startup.
* [stikypiston/unobtrusive-relnums.nvim](https://github.com/stikypiston/unobtrusive-relnums) - Unobtrusive relative line numbers in the sign column.

### CSV Files

* [hat0uma/csvview.nvim](https://github.com/hat0uma/csvview.nvim) ⭐ 545 | 🐛 14 | 🌐 Lua | 📅 2026-02-14 - An asynchronous CSV/TSV table viewer with real-time updates, configurable comments and delimiters, and multiple display modes.
* [emmanueltouzery/decisive.nvim](https://github.com/emmanueltouzery/decisive.nvim) ⭐ 124 | 🐛 2 | 🌐 Lua | 📅 2025-06-05 - View and edit CSV files with ease and speed.
* [VidocqH/data-viewer.nvim](https://github.com/VidocqH/data-viewer.nvim) ⭐ 122 | 🐛 9 | 🌐 Lua | 📅 2024-07-29 - Provide a simple table view to inspect data files such as `csv`, `tsv`.
* [theKnightsOfRohan/csvlens.nvim](https://github.com/theKnightsOfRohan/csvlens.nvim) ⭐ 39 | 🐛 1 | 🌐 Lua | 📅 2024-04-28 - A port of [YS-L/csvlens](https://github.com/YS-L/csvlens) ⭐ 3,459 | 🐛 53 | 🌐 Rust | 📅 2026-02-02, for easy previewing of tabular data.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Animation

* [nvim-mini/mini.nvim#mini.animate](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-animate.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` to add out of the box animations for common built-in actions (cursor movement, scroll, resize, window open/close).
* [sphamba/smear-cursor.nvim](https://github.com/sphamba/smear-cursor.nvim) ⭐ 1,667 | 🐛 6 | 🌐 Lua | 📅 2025-12-01 - Animate the cursor with a smear effect in all terminals. Inspired by Neovide's animated cursor.
* [rachartier/tiny-glimmer.nvim](https://github.com/rachartier/tiny-glimmer.nvim/) ⭐ 395 | 🐛 1 | 🌐 Lua | 📅 2026-01-19 - Adds subtle animations to various operations.
* [gen740/SmoothCursor.nvim](https://github.com/gen740/SmoothCursor.nvim) ⭐ 392 | 🐛 3 | 🌐 Lua | 📅 2024-09-18 - Add fancy sub-cursor to signcolumn to show your scroll or jump direction.
* [y3owk1n/undo-glow.nvim](https://github.com/y3owk1n/undo-glow.nvim/) ⭐ 86 | 🐛 0 | 🌐 Lua | 📅 2025-12-14 - Animated glow/highlight effects for editing operations (undo, redo, yank, paste, etc.) with fully customizable animations and appearance.
* [LuxVim/nvim-luxmotion](https://github.com/LuxVim/nvim-luxmotion) ⭐ 44 | 🐛 2 | 🌐 Lua | 📅 2026-02-08 - Smooth, high‑performance motion and scrolling animations — 60fps fluid cursor moves, word jumps, and viewport scrolling, all in one.
* [stikypiston/smudge.nvim](https://github.com/stikypiston/smudge.nvim) ⭐ 8 | 🐛 0 | 🌐 Lua | 📅 2026-02-09 - Performant cursor animations.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Terminal Integration

* [akinsho/toggleterm.nvim](https://github.com/akinsho/toggleterm.nvim) ⭐ 5,372 | 🐛 85 | 🌐 Lua | 📅 2025-03-09 - Easily manage multiple terminal windows.
* [kassio/neoterm](https://github.com/kassio/neoterm) ⭐ 1,337 | 🐛 31 | 🌐 Vim Script | 📅 2023-03-09 - Wrapper of some `:terminal` functions.
* [mikesmithgh/kitty-scrollback.nvim](https://github.com/mikesmithgh/kitty-scrollback.nvim) ⭐ 819 | 🐛 29 | 🌐 Lua | 📅 2026-01-21 - Open your Kitty scrollback buffer. Ameowzing.
* [numToStr/FTerm.nvim](https://github.com/numToStr/FTerm.nvim) ⭐ 803 | 🐛 25 | 🌐 Lua | 📅 2023-10-19 - No nonsense floating terminal written in Lua.
* [willothy/flatten.nvim](https://github.com/willothy/flatten.nvim) ⭐ 687 | 🐛 14 | 🌐 Lua | 📅 2025-05-27 - Open files from terminal buffers in your current Neovim instance instead of launching a nested instance.
* [nikvdp/neomux](https://github.com/nikvdp/neomux) ⭐ 376 | 🐛 0 | 🌐 Vim Script | 📅 2025-12-14 - Control Neovim from shells ran through the `:term` command.
* [norcalli/nvim-terminal.lua](https://github.com/norcalli/nvim-terminal.lua) ⭐ 277 | 🐛 8 | 🌐 Lua | 📅 2022-11-21 - A high performance filetype mode which leverages conceal and highlights your buffer with the correct color codes.
* [samjwill/nvim-unception](https://github.com/samjwill/nvim-unception) ⭐ 236 | 🐛 9 | 🌐 Lua | 📅 2025-08-15 - Automatic unnesting of Neovim sessions started from terminal buffers.
* [chomosuke/term-edit.nvim](https://github.com/chomosuke/term-edit.nvim) ⭐ 207 | 🐛 7 | 🌐 Lua | 📅 2024-10-17 - Allowing you to edit your command in the terminal just like any other buffer.
* [laktak/tome](https://github.com/laktak/tome) ⭐ 155 | 🐛 1 | 🌐 Vim Script | 📅 2025-10-08 - Interactive Script playbooks for your terminal (optionally with Tmux).
* [s1n7ax/nvim-terminal](https://github.com/s1n7ax/nvim-terminal) ⭐ 120 | 🐛 2 | 🌐 Lua | 📅 2026-02-10 - A simple and easy to use multi-terminal plugin.
* [samharju/yeet.nvim](https://github.com/samharju/yeet.nvim) ⭐ 118 | 🐛 1 | 🌐 Lua | 📅 2025-10-22 - Run shell commands in terminal buffers or tmux panes.
* [jghauser/kitty-runner.nvim](https://github.com/jghauser/kitty-runner.nvim) ⭐ 106 | 🐛 7 | 🌐 Lua | 📅 2025-08-31 - Poor man's REPL. Easily send buffer lines and commands to a kitty terminal.
* [waiting-for-dev/ergoterm.nvim](https://github.com/waiting-for-dev/ergoterm.nvim) ⭐ 95 | 🐛 0 | 🌐 Lua | 📅 2026-02-05 - Seamless terminal workflow integration with smart picker-based terminal selection, flexible text sending and persistent configuration.
* [2KAbhishek/termim.nvim](https://github.com/2KAbhishek/termim.nvim/) ⭐ 79 | 🐛 0 | 🌐 Lua | 📅 2025-12-01 - Neovim Terminal, Improved.
* [nyngwang/NeoTerm.lua](https://github.com/nyngwang/NeoTerm.lua) ⭐ 68 | 🐛 7 | 🌐 Lua | 📅 2024-01-27 - Attach a terminal for each **buffer**, now with stable toggle and astonishing cursor restoring.
* [jlesquembre/nterm.nvim](https://github.com/jlesquembre/nterm.nvim) ⭐ 58 | 🐛 1 | 🌐 Lua | 📅 2026-02-17 - Interact with the terminal, with notifications.
* [Dan7h3x/neaterm.nvim](https://github.com/Dan7h3x/neaterm.nvim) ⭐ 57 | 🐛 1 | 🌐 Lua | 📅 2025-07-25 - A little smart terminal/REPL manager with awesome features.
* [isak102/ghostty.nvim](https://github.com/isak102/ghostty.nvim) ⭐ 46 | 🐛 1 | 🌐 Lua | 📅 2025-01-04 - Automatically validate your Ghostty configuration on save.
* [da-moon/telescope-toggleterm.nvim](https://github.com/da-moon/telescope-toggleterm.nvim) ⭐ 40 | 🐛 0 | 🌐 Dockerfile | 📅 2022-02-09 - Telescope picker for terminal buffers.
* [logicmagix/tide42](https://github.com/logicmagix/tide42) ⭐ 23 | 🐛 0 | 🌐 Shell | 📅 2025-09-29 - A fully integrated terminal IDE built on Neovim, tmux, and scriptable workflows.
* [ingur/floatty.nvim](https://github.com/ingur/floatty.nvim) ⭐ 22 | 🐛 0 | 🌐 Lua | 📅 2025-09-12 - A tiny (<200 LOC) but highly customizable floating terminal manager.
* [niuiic/terminal.nvim](https://github.com/niuiic/terminal.nvim) ⭐ 20 | 🐛 0 | 🌐 Lua | 📅 2024-11-13 - Manage terminal as buffer, multiple terminals support.
* [benoror/gpg.nvim](https://github.com/benoror/gpg.nvim) ⭐ 20 | 🐛 1 | 🌐 Lua | 📅 2026-02-08 - Edit GPG encrypted files symmetrically.
* [NeViRAIDE/nekifoch.nvim](https://github.com/NeViRAIDE/nekifoch.nvim) ⚠️ Archived - Managing Kitty terminal font settings.
* [LuxVim/nvim-luxterm](https://github.com/LuxVim/nvim-luxterm) ⭐ 12 | 🐛 0 | 🌐 Lua | 📅 2026-02-11 - A floating-window terminal session manager, offering elegant multi-terminal organization, live previews, and intuitive navigation with modern UI design. Manage, switch, and customize multiple terminals effortlessly.
* [imranzero/multiterm.nvim](https://github.com/imranZERO/multiterm.nvim) ⭐ 12 | 🐛 0 | 🌐 Lua | 📅 2026-01-24 - Effortlessly manage multiple floating terminal windows.
* [idanarye/nvim-channelot](https://github.com/idanarye/nvim-channelot) ⭐ 7 | 🐛 2 | 🌐 Lua | 📅 2025-10-26 - Operate Neovim jobs from Lua coroutines.
* [Axot017/multiterm.nvim](https://github.com/Axot017/multiterm.nvim) ⭐ 5 | 🐛 0 | 🌐 Lua | 📅 2025-04-29 - A lightweight manager of multiple terminal instances with key bindings.
* [gh-liu/nvim-winterm](https://github.com/gh-liu/nvim-winterm) ⭐ 5 | 🐛 0 | 🌐 Lua | 📅 2026-01-29 - Multi-terminal window manager.
* [TheLazyCat00/runner-nvim](https://github.com/TheLazyCat00/runner-nvim) ⭐ 4 | 🐛 0 | 🌐 Lua | 📅 2026-02-11 - Run commands in a floating terminal and keep track of the last command executed per CWD, making it easy to repeat build or test commands.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Debugging

* [mfussenegger/nvim-dap](https://github.com/mfussenegger/nvim-dap) ⭐ 6,952 | 🐛 30 | 🌐 Lua | 📅 2026-02-11 - Debug Adapter Protocol client implementation.
* [rcarriga/nvim-dap-ui](https://github.com/rcarriga/nvim-dap-ui) ⭐ 3,280 | 🐛 107 | 🌐 Lua | 📅 2025-07-09 - A UI for nvim-dap.
* [theHamsta/nvim-dap-virtual-text](https://github.com/theHamsta/nvim-dap-virtual-text) ⭐ 1,053 | 🐛 10 | 🌐 Lua | 📅 2025-05-25 - Virtual text support for nvim-dap.
* [sakhnik/nvim-gdb](https://github.com/sakhnik/nvim-gdb) ⭐ 771 | 🐛 4 | 🌐 Lua | 📅 2025-12-31 - Thin wrapper for GDB, LLDB, PDB/PDB++ and BashDB.
* [igorlfs/nvim-dap-view](https://github.com/igorlfs/nvim-dap-view) ⭐ 629 | 🐛 7 | 🌐 Lua | 📅 2026-02-11 - A modern, minimalistic UI for nvim-dap.
* [andrewferrier/debugprint.nvim](https://github.com/andrewferrier/debugprint.nvim) ⭐ 509 | 🐛 10 | 🌐 Lua | 📅 2026-02-12 - Debugging the print() way.
* [pocco81/dap-buddy.nvim](https://github.com/pocco81/dap-buddy.nvim) ⭐ 398 | 🐛 25 | 🌐 Lua | 📅 2022-09-26 - Manage several debuggers for nvim-dap.
* [t-troebst/perfanno.nvim](https://github.com/t-troebst/perfanno.nvim) ⭐ 359 | 🐛 1 | 🌐 Lua | 📅 2026-01-20 - Annotate your code with callgraph profiling data. Native support for perf, flamegraph and the LuaJit profiler.
* [Weissle/persistent-breakpoints.nvim](https://github.com/Weissle/persistent-breakpoints.nvim) ⭐ 250 | 🐛 2 | 🌐 Lua | 📅 2025-03-22 - Persistent breakpoints for nvim-dap.
* [chrisgrieser/nvim-chainsaw](https://github.com/chrisgrieser/nvim-chainsaw) ⭐ 136 | 🐛 0 | 🌐 Lua | 📅 2026-02-06 - Speed up log creation. Creates various kinds of language-specific log statements, like logs of variables, assertions, or time-measuring.
* [niuiic/dap-utils](https://github.com/niuiic/dap-utils.nvim) ⭐ 40 | 🐛 0 | 🌐 Lua | 📅 2024-05-11 - Utilities to provide a better experience for using nvim-dap.
* [Willem-J-an/visidata.nvim](https://github.com/Willem-J-an/visidata.nvim) ⭐ 34 | 🐛 0 | 🌐 Lua | 📅 2024-03-19 - Render Pandas dataframes in `nvim-dap` using the power of visidata.
* [ofirgall/goto-breakpoints.nvim](https://github.com/ofirgall/goto-breakpoints.nvim) ⭐ 33 | 🐛 0 | 🌐 Lua | 📅 2023-11-02 - Cycle between breakpoints for nvim-dap.
* [Carcuis/dap-breakpoints.nvim](https://github.com/Carcuis/dap-breakpoints.nvim) ⭐ 17 | 🐛 0 | 🌐 Lua | 📅 2026-01-09 - Manage and create advanced breakpoints with virtual text and popup reveal for nvim-dap.
* [ravsii/nvim-dap-envfile](https://github.com/ravsii/nvim-dap-envfile) ⭐ 14 | 🐛 0 | 🌐 Lua | 📅 2026-01-10 - Automatic `envFile` support for nvim-dap.
* [fschaal/azfunc.nvim](https://github.com/fschaal/azfunc.nvim) ⭐ 3 | 🐛 0 | 🌐 Lua | 📅 2025-11-09 - Seamlessly debug Azure Functions with automatic DAP integration.

### Quickfix

* [kevinhwang91/nvim-bqf](https://github.com/kevinhwang91/nvim-bqf) ⭐ 1,986 | 🐛 17 | 🌐 Lua | 📅 2026-02-02 - Makes the quickfix window better.
* [stevearc/quicker.nvim](https://github.com/stevearc/quicker.nvim) ⭐ 912 | 🐛 16 | 🌐 Lua | 📅 2026-01-12 - Improved quickfix UI and editable quickfix buffer.
* [yorickpeterse/nvim-pqf](https://github.com/yorickpeterse/nvim-pqf) ⭐ 177 | 🐛 1 | 🌐 Lua | 📅 2024-08-12 - Prettier quickfix/location list windows.
* [ashfinal/qfview.nvim](https://github.com/ashfinal/qfview.nvim) ⭐ 54 | 🐛 0 | 🌐 Lua | 📅 2023-09-09 - Pretty quickfix/location view with consistent path-shorten and folding.
* [niuiic/quickfix.nvim](https://github.com/niuiic/quickfix.nvim) ⭐ 12 | 🐛 0 | 🌐 Lua | 📅 2024-11-01 - Extended functionality for quickfix, including store, restore, make, remove, etc.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Deployment

* [OscarCreator/rsync.nvim](https://github.com/OscarCreator/rsync.nvim) ⭐ 100 | 🐛 8 | 🌐 Lua | 📅 2024-08-08 - Automatically sync up/down project to a remote with rsync.
* [sachinsenal0x64/hot.nvim](https://github.com/sachinsenal0x64/hot.nvim) ⚠️ Archived - A hot reloader that works with any programming language.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Test

* [nvim-neotest/neotest](https://github.com/nvim-neotest/neotest) ⭐ 3,022 | 🐛 108 | 🌐 Lua | 📅 2025-11-08 - An extensible framework for interacting with tests within Neovim.
* [andythigpen/nvim-coverage](https://github.com/andythigpen/nvim-coverage) ⭐ 425 | 🐛 17 | 🌐 Lua | 📅 2024-12-18 - Displays coverage information in the sign column.
* [David-Kunz/jester](https://github.com/David-Kunz/jester) ⭐ 214 | 🐛 4 | 🌐 Lua | 📅 2025-01-15 - Easily run and debug Jest tests.
* [klen/nvim-test](https://github.com/klen/nvim-test) ⭐ 197 | 🐛 19 | 🌐 Lua | 📅 2024-01-08 - A wrapper for running tests.
* [nvim-neotest/neotest-jest](https://github.com/nvim-neotest/neotest-jest) ⭐ 147 | 🐛 5 | 🌐 Lua | 📅 2025-12-27 - Neotest adapter for running Jest tests.
* [quolpr/quicktest.nvim](https://github.com/quolpr/quicktest.nvim) ⭐ 104 | 🐛 4 | 🌐 C++ | 📅 2025-11-04 - Run your tests in split window or popup with live feedback.
* [MisanthropicBit/neotest-busted](https://github.com/MisanthropicBit/neotest-busted) ⭐ 16 | 🐛 8 | 🌐 Lua | 📅 2026-01-31 - Neotest adapter for running busted tests using Neovim as a Lua interpreter.
* [mr-u0b0dy/crazy-coverage.nvim](https://github.com/mr-u0b0dy/crazy-coverage.nvim) ⭐ 9 | 🐛 2 | 🌐 Lua | 📅 2026-02-14 - Display code coverage.
* [zkucekovic/tdd.nvim](https://github.com/zkucekovic/tdd.nvim) ⭐ 6 | 🐛 0 | 🌐 Lua | 📅 2025-11-05 - Opens or creates the matching PHPUnit test file for a given class, based on PSR-4 namespace mappings.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Code Runner

* [stevearc/overseer.nvim](https://github.com/stevearc/overseer.nvim) ⭐ 1,813 | 🐛 73 | 🌐 Lua | 📅 2026-02-11 - A task runner and job management plugin.
* [michaelb/sniprun](https://github.com/michaelb/sniprun) ⭐ 1,671 | 🐛 11 | 🌐 Rust | 📅 2025-12-30 - Run parts of code of any language directly from Neovim.
* [Vigemus/iron.nvim](https://github.com/Vigemus/iron.nvim) ⭐ 1,299 | 🐛 57 | 🌐 Lua | 📅 2026-01-05 - Interactive REPLs of over 30 languages embedded.
* [benlubas/molten-nvim](https://github.com/benlubas/molten-nvim) ⭐ 1,108 | 🐛 39 | 🌐 Python | 📅 2025-11-05 - Enables running code chunks via the Jupyter kernel. Output (including image output) is rendered in a floating window below the code.
* [CRAG666/code\_runner.nvim](https://github.com/CRAG666/code_runner.nvim) ⭐ 675 | 🐛 7 | 🌐 Lua | 📅 2026-02-13 - The best code runner you could have, with super powers.
* [rafcamlet/nvim-luapad](https://github.com/rafcamlet/nvim-luapad) ⭐ 671 | 🐛 5 | 🌐 Lua | 📅 2026-02-07 - Interactive scratchpad for running Lua code.
* [Zeioth/compiler.nvim](https://github.com/Zeioth/compiler.nvim) ⭐ 654 | 🐛 9 | 🌐 Lua | 📅 2025-08-14 - Compiler for building and running your code without having to configure anything.
* [Civitasv/cmake-tools.nvim](https://github.com/Civitasv/cmake-tools.nvim) ⭐ 522 | 🐛 25 | 🌐 Lua | 📅 2026-02-12 - CMake integration.
* [milanglacier/yarepl.nvim](https://github.com/milanglacier/yarepl.nvim) ⭐ 247 | 🐛 2 | 🌐 Lua | 📅 2026-02-04 - Yet Another REPL, flexible, supporting multiple paradigms to interact with REPLs, and native dot repeat without other dependencies.
* [EthanJWright/vs-tasks.nvim](https://github.com/EthanJWright/vs-tasks.nvim) ⭐ 207 | 🐛 1 | 🌐 Lua | 📅 2025-10-27 - Run and manage project jobs, supporting VSCode's `tasks.json` spec.
* [krady21/compiler-explorer.nvim](https://github.com/krady21/compiler-explorer.nvim) ⭐ 183 | 🐛 1 | 🌐 Lua | 📅 2026-02-09 - Asynchronous compilation using the [compiler-explorer](https://godbolt.org/) REST API.
* [is0n/jaq-nvim](https://github.com/is0n/jaq-nvim) ⭐ 179 | 🐛 11 | 🌐 Lua | 📅 2024-07-21 - Just Another Quickrun Plugin in Lua.
* [jedrzejboczar/toggletasks.nvim](https://github.com/jedrzejboczar/toggletasks.nvim) ⭐ 160 | 🐛 5 | 🌐 Lua | 📅 2023-03-08 - Task runner with JSON/YAML configs, using toggleterm.nvim and telescope.nvim.
* [google/executor.nvim](https://github.com/google/executor.nvim) ⭐ 158 | 🐛 8 | 🌐 Lua | 📅 2025-08-15 - Allows you to run command line tasks in the background and be notified of results.
* [Shatur/neovim-tasks](https://github.com/Shatur/neovim-tasks) ⭐ 124 | 🐛 4 | 🌐 Lua | 📅 2026-01-29 - A stateful task manager focused on integration with build systems.
* [MarcHamamji/runner.nvim](https://github.com/MarcHamamji/runner.nvim) ⭐ 51 | 🐛 2 | 🌐 Lua | 📅 2025-03-04 - A customizable Lua code runner.
* [dasupradyumna/launch.nvim](https://github.com/dasupradyumna/launch.nvim) ⭐ 50 | 🐛 14 | 🌐 Lua | 📅 2025-07-06 - A simple and quick task launcher which allows dynamically configuring tasks on the fly, with optional support for debugging.
* [al1-ce/just.nvim](https://github.com/al1-ce/just.nvim) ⭐ 45 | 🐛 6 | 🌐 Lua | 📅 2026-02-14 - Task runner for justfiles.
* [Zeioth/makeit.nvim](https://github.com/Zeioth/makeit.nvim) ⭐ 44 | 🐛 6 | 🌐 Lua | 📅 2025-06-24 - Makefile runner based on overseer.
* [chrisgrieser/nvim-justice](https://github.com/chrisgrieser/nvim-justice) ⭐ 35 | 🐛 0 | 🌐 Lua | 📅 2026-02-06 - Lightweight integration of the `just` task runner.
* [desdic/greyjoy.nvim](https://github.com/desdic/greyjoy.nvim) ⭐ 31 | 🐛 0 | 🌐 Lua | 📅 2025-12-24 - A modular task runner for Makefiles, VSCode tasks, kitchen etc.
* [pianocomposer321/officer.nvim](https://github.com/pianocomposer321/officer.nvim) ⭐ 22 | 🐛 3 | 🌐 Lua | 📅 2025-09-10 - Like dispatch.vim but using overseer.nvim.
* [idanarye/nvim-moonicipal](https://github.com/idanarye/nvim-moonicipal) ⭐ 19 | 🐛 1 | 🌐 Lua | 📅 2025-11-03 - Task runner with focus on rapidly changing personal tasks.
* [jaytyrrell13/static.nvim](https://github.com/jaytyrrell13/static.nvim) ⭐ 11 | 🐛 0 | 🌐 Lua | 📅 2023-12-29 - Run static site generator commands.
* [ok97465/ipybridge.nvim](https://github.com/ok97465/ipybridge.nvim) ⭐ 11 | 🐛 5 | 🌐 Lua | 📅 2026-01-21 - Run Python code, execute Jupyter cells, debug, and explore variables.
* [speelbarrow/spLauncher.nvim](https://github.com/speelbarrow/spLauncher.nvim) ⭐ 7 | 🐛 0 | 🌐 Lua | 📅 2024-07-02 - For launching tasks, I guess.
* [pewpewnor/pilot.nvim](https://github.com/pewpewnor/pilot.nvim) ⭐ 7 | 🐛 0 | 🌐 Lua | 📅 2026-02-07 - Run your projects and files quickly with keybindings, and configure how to run them on the fly.
* [niuiic/task.nvim](https://github.com/niuiic/task.nvim) ⭐ 6 | 🐛 0 | 🌐 Lua | 📅 2025-02-26 - Another highly configurable task manager that enables seamless interaction with tasks.
* [wsdjeg/code-runner.nvim](https://github.com/wsdjeg/code-runner.nvim) ⭐ 5 | 🐛 1 | 🌐 Lua | 📅 2025-12-18 - Async code runner with range support.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Neovim Lua Development

* [nvim-mini/mini.nvim#mini.doc](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-doc.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` for generation of help files from EmmyLua-like annotations. Allows flexible customization of output via hook functions.
* [nvim-mini/mini.nvim#mini.test](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-test.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` with framework for writing extensive Neovim plugin tests with support for hierarchical tests, hooks, parametrization, filtering, screen tests, "busted-style" emulation, customizable reporters, and more.
* [nvim-lua/plenary.nvim](https://github.com/nvim-lua/plenary.nvim) ⭐ 3,386 | 🐛 156 | 🌐 Lua | 📅 2025-07-26 - Plenary: full; complete; entire; absolute; unqualified. All the Lua functions I don't want to write twice.
* [MunifTanjim/nui.nvim](https://github.com/MunifTanjim/nui.nvim) ⭐ 2,023 | 🐛 30 | 🌐 Lua | 📅 2025-06-08 - UI Component Library.
* [folke/lazydev.nvim](https://github.com/folke/lazydev.nvim) ⭐ 1,451 | 🐛 6 | 🌐 Lua | 📅 2025-11-06 - Faster LuaLS setup.
* [kkharji/sqlite.lua](https://github.com/kkharji/sqlite.lua) ⭐ 566 | 🐛 21 | 🌐 Lua | 📅 2025-03-14 - SQLite/LuaJIT bindings.
* [jbyuki/one-small-step-for-vimkind](https://github.com/jbyuki/one-small-step-for-vimkind) ⭐ 536 | 🐛 7 | 🌐 Lua | 📅 2026-01-12 - An adapter for the Neovim Lua language that allows debugging any Lua code running within a Neovim instance.
* [OXY2DEV/helpview.nvim](https://github.com/OXY2DEV/helpview.nvim) ⭐ 381 | 🐛 1 | 🌐 Lua | 📅 2025-09-26 - A hackable and fancy `vimdoc/help` file viewer.
* [svermeulen/vimpeccable](https://github.com/svermeulen/vimpeccable) ⭐ 349 | 🐛 9 | 🌐 Lua | 📅 2022-04-24 - Commands to help write your .vimrc in Lua or any Lua based language.
* [bfredl/nvim-luadev](https://github.com/bfredl/nvim-luadev) ⭐ 283 | 🐛 2 | 🌐 Lua | 📅 2023-03-13 - REPL/debug console Lua plugins. The `:Luadev` command will open an scratch window which will show output from executing Lua code.
* [lumen-oss/lz.n](https://github.com/lumen-oss/lz.n) ⭐ 247 | 🐛 1 | 🌐 Lua | 📅 2026-02-17 - A simple lazy loading library for Neovim plugins.
* [ray-x/guihua.lua](https://github.com/ray-x/guihua.lua) ⭐ 184 | 🐛 5 | 🌐 Lua | 📅 2025-11-12 - A Lua UI library. Includes a fzy search bar, list view and tree view modules.
* [DrKJeff16/wezterm-types](https://github.com/DrKJeff16/wezterm-types) ⭐ 167 | 🐛 1 | 🌐 Lua | 📅 2026-02-17 - WezTerm config type annotations for Lua Language Server, including support for community plugins.
* [CWood-sdf/banana.nvim](https://github.com/CWood-sdf/banana.nvim) ⭐ 154 | 🐛 2 | 🌐 Lua | 📅 2025-12-09 - HTML renderer for plugin UIs.
* [tjdevries/vlog.nvim](https://github.com/tjdevries/vlog.nvim) ⭐ 143 | 🐛 6 | 🌐 Lua | 📅 2023-10-30 - Single file, no dependency, easy copy and paste log file to add to your Neovim Lua plugins.
* [gregorias/coop.nvim](https://github.com/gregorias/coop.nvim) ⭐ 143 | 🐛 0 | 🌐 Lua | 📅 2025-07-24 - Structured concurrency with Lua coroutines.
* [milisims/nvim-luaref](https://github.com/milisims/nvim-luaref) ⭐ 127 | 🐛 3 | 🌐 Vim script | 📅 2024-07-10 - A reference for built-in Lua functions.
* [BirdeeHub/lze](https://github.com/BirdeeHub/lze) ⭐ 105 | 🐛 1 | 🌐 Lua | 📅 2026-02-15 - A lazy-loading library for Neovim plugins.
* [jrop/morph.nvim](https://github.com/jrop/morph.nvim) ⭐ 100 | 🐛 0 | 🌐 Lua | 📅 2026-02-11 - A React-like renderer for building interactive buffers/TUIs.
* [YaroSpace/lua-console.nvim](https://github.com/YaroSpace/lua-console.nvim) ⭐ 89 | 🐛 1 | 🌐 Lua | 📅 2025-11-24 - A handy scratch pad / REPL / debug console for Neovim Lua development.
* [lumen-oss/luarocks-tag-release](https://github.com/lumen-oss/luarocks-tag-release) ⭐ 56 | 🐛 10 | 🌐 Lua | 📅 2026-02-17 - A GitHub action that publishes your Neovim plugins to LuaRocks.
* [anuvyklack/animation.nvim](https://github.com/anuvyklack/animation.nvim) ⭐ 46 | 🐛 0 | 🌐 Lua | 📅 2022-09-18 - Create animations.
* [svermeulen/nvim-lusc](https://github.com/svermeulen/nvim-lusc) ⭐ 16 | 🐛 1 | 🌐 Lua | 📅 2024-02-23 - Adds support for Structured Async/Concurrency in Lua.
* [chrisgve/databox.nvim](https://github.com/chrisgve/databox.nvim) ⭐ 12 | 🐛 0 | 🌐 Lua | 📅 2025-05-23 - Encrypted storage for Lua tables using [age](https://github.com/FiloSottile/age) ⭐ 21,327 | 🐛 13 | 🌐 Go | 📅 2026-02-02 or compatible encryption tools for cryptographic safety.
* [2KAbhishek/utils.nvim](https://github.com/2KAbhishek/utils.nvim) ⭐ 10 | 🐛 0 | 🌐 Lua | 📅 2025-07-27 - Powerful utilities to speed up plugin development.
* [nfrid/treesitter-utils](https://github.com/nfrid/treesitter-utils) ⭐ 9 | 🐛 0 | 🌐 Lua | 📅 2024-06-13 - Some useful Tree-sitter methods.
* [niuiic/omega.nvim](https://github.com/niuiic/omega.nvim) ⭐ 6 | 🐛 0 | 🌐 Lua | 📅 2025-03-13 - Missing functions for Lua plugin development.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Fennel

* [Olical/conjure](https://github.com/Olical/conjure) ⭐ 2,053 | 🐛 94 | 🌐 Fennel | 📅 2026-02-13 - Interactive evaluation (Clojure, Fennel, Janet, Racket, Hy, MIT Scheme, Guile).
* [Olical/aniseed](https://github.com/Olical/aniseed) ⭐ 645 | 🐛 7 | 🌐 Fennel | 📅 2025-06-12 - Configure and extend Neovim with Fennel.
* [rktjmp/hotpot.nvim](https://github.com/rktjmp/hotpot.nvim) ⭐ 386 | 🐛 11 | 🌐 Fennel | 📅 2025-12-23 - Seamless, transparent Fennel inside Neovim.
* [Olical/nfnl](https://github.com/Olical/nfnl) ⭐ 337 | 🐛 6 | 🌐 Fennel | 📅 2025-11-02 - Streamlined successor to Aniseed, compiling Fennel to Lua on file write.
* [udayvir-singh/tangerine.nvim](https://github.com/udayvir-singh/tangerine.nvim) ⭐ 226 | 🐛 9 | 🌐 Fennel | 📅 2024-10-18 - Tangerine provides a painless way to add Fennel to your config.
* [udayvir-singh/hibiscus.nvim](https://github.com/udayvir-singh/hibiscus.nvim) ⭐ 106 | 🐛 3 | 🌐 Fennel | 📅 2024-07-21 - Highly opinionated macros to elegantly write your config.
* [aileot/nvim-thyme](https://github.com/aileot/nvim-thyme) ⭐ 38 | 🐛 2 | 🌐 Fennel | 📅 2025-11-04 - Zero-overhead Fennel JIT compiler with safety rollbacks and [parinfer-rust](https://github.com/eraserhd/parinfer-rust) ⭐ 610 | 🐛 35 | 🌐 Rust | 📅 2026-01-03 integration.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Dependency Management

* [Saecki/crates.nvim](https://github.com/Saecki/crates.nvim) ⭐ 1,077 | 🐛 10 | 🌐 Lua | 📅 2025-08-23 - Rust dependency management for `Cargo.toml`.
* [vuki656/package-info.nvim](https://github.com/vuki656/package-info.nvim) ⭐ 587 | 🐛 26 | 🌐 Lua | 📅 2025-12-27 - Display latest package version as virtual text in package.json.
* [piersolenski/import.nvim](https://github.com/piersolenski/import.nvim) ⭐ 261 | 🐛 0 | 🌐 Lua | 📅 2025-11-12 - Import modules faster based on what you've already imported in your project.
* [JesperLundberg/projektgunnar.nvim](https://github.com/JesperLundberg/projektgunnar.nvim) ⭐ 20 | 🐛 0 | 🌐 Lua | 📅 2026-01-15 - C# dependency manager with support for handling references between projects and solution files.
* [Silletr/LazyDeveloperHelper](https://github.com/Silletr/LazyDeveloperHelper) ⭐ 11 | 🐛 0 | 🌐 Python | 📅 2026-02-13 - Python dependencies manager, with auto-adding to your `requirements.txt` file.
* [DrKJeff16/pipenv.nvim](https://github.com/DrKJeff16/pipenv.nvim) ⭐ 7 | 🐛 0 | 🌐 Lua | 📅 2026-02-17 - Asynchronous `Pipenv` manager with `spinner.nvim` integration.
* [cosmicbuffalo/gem\_install.nvim](https://github.com/cosmicbuffalo/gem_install.nvim) ⭐ 1 | 🐛 0 | 🌐 Lua | 📅 2026-02-09 - Install Ruby gems, trigger `bundle install` and `gem install` with progress and caching to prevent retries when installs fail.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Git

* [nvim-mini/mini.nvim#mini.diff](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-diff.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` to interactively visualize difference between buffer text and its reference. Provides toggleable detailed overview in text area, built-in apply/reset/textobject/goto mappings, and more.
* [nvim-mini/mini.nvim#mini.git](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-git.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` for enhanced Git integration with current Neovim process that implements tracking of Git related data, `:Git` user command, and various helpers to explore Git history.
* [lewis6991/gitsigns.nvim](https://github.com/lewis6991/gitsigns.nvim) ⭐ 6,567 | 🐛 35 | 🌐 Lua | 📅 2026-02-13 - Git integration: signs, hunk actions, blame, etc.
* [sindrets/diffview.nvim](https://github.com/sindrets/diffview.nvim) ⭐ 5,341 | 🐛 132 | 🌐 Lua | 📅 2024-08-02 - Single tabpage interface for easily cycling through diffs for all modified files for any Git rev.
* [NeogitOrg/neogit](https://github.com/NeogitOrg/neogit) ⭐ 5,139 | 🐛 169 | 🌐 Lua | 📅 2026-02-16 - A Magit clone that may change some things to fit the Vim philosophy.
* [kdheepak/lazygit.nvim](https://github.com/kdheepak/lazygit.nvim) ⭐ 2,187 | 🐛 49 | 🌐 Lua | 📅 2025-12-19 - Plugin for calling lazygit.
* [esmuellert/codediff.nvim](https://github.com/esmuellert/codediff.nvim) ⭐ 1,111 | 🐛 39 | 🌐 Lua | 📅 2026-02-16 - Side-by-side diff with two-tier highlighting (line + character level) using VSCode's algorithm implemented in C.
* [f-person/git-blame.nvim](https://github.com/f-person/git-blame.nvim) ⭐ 1,067 | 🐛 11 | 🌐 Lua | 📅 2025-11-05 - Show Git blame info.
* [tanvirtin/vgit.nvim](https://github.com/tanvirtin/vgit.nvim) ⭐ 836 | 🐛 16 | 🌐 Lua | 📅 2026-01-25 - Visual Git Plugin to enhance your Git experience.
* [SuperBo/fugit2.nvim](https://github.com/SuperBo/fugit2.nvim) ⭐ 463 | 🐛 14 | 🌐 Lua | 📅 2025-09-02 - Git GUI powered by [libgit2](https://libgit2.org).
* [aaronhallaert/advanced-git-search.nvim](https://github.com/aaronhallaert/advanced-git-search.nvim) ⭐ 388 | 🐛 3 | 🌐 Lua | 📅 2025-12-09 - Search your Git history by commit content, message and author with Telescope.
* [linrongbin16/gitlinker.nvim](https://github.com/linrongbin16/gitlinker.nvim) ⭐ 262 | 🐛 2 | 🌐 Lua | 📅 2026-01-28 - Maintained fork of "ruifm's gitlinker", refactored with bug fixes, ssh aliases, blame support and other improvements.
* [chrisgrieser/nvim-tinygit](https://github.com/chrisgrieser/nvim-tinygit) ⭐ 202 | 🐛 1 | 🌐 Lua | 📅 2026-02-06 - Lightweight and nimble Git client.
* [tveskag/nvim-blame-line](https://github.com/tveskag/nvim-blame-line) ⭐ 187 | 🐛 3 | 🌐 Vim Script | 📅 2025-03-03 - A small plugin that uses the virtual text to print Git blame info at the end of the current line.
* [axkirillov/unified.nvim](https://github.com/axkirillov/unified.nvim) ⭐ 125 | 🐛 5 | 🌐 Lua | 📅 2026-02-16 - Displaying inline unified diffs directly in your buffer.
* [chojs23/ec](https://github.com/chojs23/ec) ⭐ 111 | 🐛 0 | 🌐 Go | 📅 2026-02-16 - A TUI native Git mergetool with 3 panes.
* [moyiz/git-dev.nvim](https://github.com/moyiz/git-dev.nvim) ⭐ 107 | 🐛 2 | 🌐 Lua | 📅 2025-12-06 - Open remote Git repositories while editing.
* [trevorhauter/gitportal.nvim](https://github.com/trevorhauter/gitportal.nvim) ⭐ 90 | 🐛 0 | 🌐 Lua | 📅 2025-12-21 - Generate Git permalinks, open them in your browser, load files locally from permalinks, and more.
* [isak102/telescope-git-file-history.nvim](https://github.com/isak102/telescope-git-file-history.nvim) ⭐ 88 | 🐛 2 | 🌐 Lua | 📅 2026-02-16 - Open/preview contents of the current file at a specific commit, without using `git checkout`.
* [StackInTheWild/headhunter.nvim](https://github.com/StackInTheWild/headhunter.nvim) ⭐ 56 | 🐛 0 | 🌐 Lua | 📅 2025-10-22 - Fast and simple utility to hunt and resolve merge conflicts.
* [barrettruth/diffs.nvim](https://github.com/barrettruth/diffs.nvim) ⭐ 46 | 🐛 2 | 🌐 Lua | 📅 2026-02-18 - Syntax highlighting for diffs with Tree-sitter support for `vim-fugitive` and `&diff` buffers.
* [spacedentist/resolve.nvim](https://github.com/spacedentist/resolve.nvim) ⭐ 44 | 🐛 5 | 🌐 Lua | 📅 2026-01-25 - Resolve merge conflicts with ease.
* [jceb/jiejie.nvim](https://github.com/jceb/jiejie.nvim) ⭐ 42 | 🐛 1 | 🌐 Lua | 📅 2026-02-17 - Frontend for Jujutsu in the style of `fugitive`.
* [yus-works/csc.nvim](https://github.com/yus-works/csc.nvim) ⭐ 37 | 🐛 0 | 🌐 Lua | 📅 2025-10-15 - Conventional commit scope completion that learns from Git history.
* [2KAbhishek/co-author.nvim](https://github.com/2KAbhishek/co-author.nvim) ⭐ 36 | 🐛 0 | 🌐 Lua | 📅 2025-10-16 - Quickly add co-authors to commits.
* [AckslD/nvim-gfold.lua](https://github.com/AckslD/nvim-gfold.lua) ⭐ 32 | 🐛 0 | 🌐 Lua | 📅 2022-10-19 - Plugin using [gfold](https://github.com/nickgerace/gfold) ⭐ 384 | 🐛 8 | 🌐 Rust | 📅 2026-02-10 to switch repo and have statusline component.
* [yutkat/git-rebase-auto-diff.nvim](https://github.com/yutkat/git-rebase-auto-diff.nvim) ⭐ 32 | 🐛 0 | 🌐 Lua | 📅 2025-07-19 - Show diff automatically when Git rebase.
* [9seconds/repolink.nvim](https://github.com/9seconds/repolink.nvim) ⭐ 22 | 🐛 0 | 🌐 Lua | 📅 2023-12-08 - Generate shareable HTTP permalinks for various Git web frontends.
* [niuiic/git-log.nvim](https://github.com/niuiic/git-log.nvim) ⭐ 20 | 🐛 0 | 🌐 Lua | 📅 2025-02-26 - Check Git log of the selected code.
* [YouSame2/inlinediff-nvim](https://github.com/YouSame2/inlinediff-nvim) ⭐ 18 | 🐛 0 | 🌐 Lua | 📅 2026-02-11 - Provides a better inline Git diff view, meant to be used alongside your favorite Git plugin (e.g. `gitsigns`).
* [Yu-Leo/blame-column.nvim](https://github.com/Yu-Leo/blame-column.nvim) ⭐ 18 | 🐛 5 | 🌐 Lua | 📅 2025-04-16 - Show Git blame info.
* [Salanoid/gitlogdiff.nvim](https://github.com/Salanoid/gitlogdiff.nvim) ⭐ 15 | 🐛 0 | 🌐 Lua | 📅 2026-01-22 - Diff between multiple Git commits, similar to JetBrains's Git log.
* [404pilo/aicommits.nvim](https://github.com/404pilo/aicommits.nvim) ⭐ 11 | 🐛 5 | 🌐 Lua | 📅 2025-10-18 - Generate conventional commit messages using AI.
* [mrloop/telescope-git-branch.nvim](https://github.com/mrloop/telescope-git-branch.nvim) ⭐ 10 | 🐛 0 | 🌐 Lua | 📅 2024-07-08 - A telescope picker to find which files and preview what changes have been made to your Git branch across multiple commits.
* [Mauritz8/gitstatus.nvim](https://github.com/Mauritz8/gitstatus.nvim) ⭐ 9 | 🐛 8 | 🌐 Lua | 📅 2025-12-18 - Interactive Git status window with support for staging, unstaging, and committing files.
* [Enigama/remarks.nvim](https://github.com/Enigama/remarks.nvim) ⭐ 8 | 🐛 1 | 🌐 Lua | 📅 2026-01-17 - Personal developer notes attached to Git commits.
* [Sengoku11/commitpad.nvim](https://github.com/Sengoku11/commitpad.nvim) ⭐ 8 | 🐛 0 | 🌐 Lua | 📅 2026-02-17 - Write informative commits with persistent worktree-isolated drafts, visual 50/72 guides, and a Markdown buffer.
* [Kohei-Wada/yadm-git.nvim](https://github.com/Kohei-Wada/yadm-git.nvim) ⭐ 7 | 🐛 0 | 🌐 Lua | 📅 2026-02-14 - Seamless Git plugin support for yadm dotfiles.
* [wsdjeg/git.nvim](https://github.com/wsdjeg/git.nvim) ⭐ 7 | 🐛 1 | 🌐 Lua | 📅 2026-01-24 - An asynchronous Git command wrapper plugin, using `:Git` command instead of `:!git`.
* [BibekBhusal0/nvim-git-utils](https://github.com/BibekBhusal0/nvim-git-utils) ⭐ 6 | 🐛 0 | 🌐 Lua | 📅 2026-01-18 - Simple commands to make life easier while working with Git.
* [ajatdarojat45/commitmate.nvim](https://github.com/ajatdarojat45/commitmate.nvim) ⭐ 5 | 🐛 0 | 🌐 Lua | 📅 2025-12-24 - An AI-assisted commit message generator following common commit conventions.

### GitHub

* [pwntester/octo.nvim](https://github.com/pwntester/octo.nvim) ⭐ 3,116 | 🐛 227 | 🌐 Lua | 📅 2026-01-22 - Work with GitHub issues and PRs.
* [ldelossa/gh.nvim](https://github.com/ldelossa/gh.nvim) ⭐ 641 | 🐛 33 | 🌐 Lua | 📅 2025-01-21 - A fully featured GitHub integration for performing code reviews.
* [rawnly/gist.nvim](https://github.com/rawnly/gist.nvim) ⭐ 212 | 🐛 1 | 🌐 Lua | 📅 2026-02-11 - Create a GitHub Gist from the current file (powered by gh).
* [topaxi/pipeline.nvim](https://github.com/topaxi/pipeline.nvim) ⭐ 182 | 🐛 1 | 🌐 Lua | 📅 2026-02-06 - View and dispatch GitHub Actions workflow and GitLab CI pipeline runs.
* [2KAbhishek/octohub.nvim](https://github.com/2KAbhishek/octohub.nvim) ⭐ 79 | 🐛 0 | 🌐 Lua | 📅 2025-08-09 - Access all your gihub repos, stats and more in simple keystrokes.
* [claydugo/browsher.nvim](https://github.com/claydugo/browsher.nvim) ⭐ 15 | 🐛 0 | 🌐 Lua | 📅 2025-12-11 - Create commit pinned links to GitHub hosted files/lines.
* [3ZsForInsomnia/revman.nvim](https://github.com/3ZsForInsomnia/revman.nvim) ⭐ 7 | 🐛 0 | 🌐 Lua | 📅 2025-11-17 - Track PRs that need review automatically and open them in Octo.nvim.
* [comatory/gh-co.nvim](https://github.com/comatory/gh-co.nvim) ⭐ 4 | 🐛 0 | 🌐 Lua | 📅 2025-12-28 - Show the code owner(s) for files according to GitHub's `CODEOWNERS` specification.
* [cd-4/git-needy.nvim](https://github.com/cd-4/git-needy.nvim) ⭐ 3 | 🐛 0 | 🌐 Lua | 📅 2025-04-15 - Keeps a tally of workflows that need to be reviewed in your statusbar.

### GitLab

* [harrisoncramer/GitLab.nvim](https://github.com/harrisoncramer/GitLab.nvim) ⭐ 356 | 🐛 28 | 🌐 Lua | 📅 2026-01-31 - Review pull requests and manage other GitLab resources.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Motion

* [nvim-mini/mini.nvim#mini.jump](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-jump.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` for smarter jumping to a single character.
* [nvim-mini/mini.nvim#mini.jump2d](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-jump2d.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` for smarter jumping within visible lines via iterative label filtering. Supports custom jump targets (spots), labels, hooks, allowed windows and lines, and more.
* [nvim-mini/mini.nvim#mini.bracketed](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-bracketed.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` to go forward/backward with square brackets.
* [ggandor/leap.nvim](https://github.com/ggandor/leap.nvim) ⭐ 5,015 | 🐛 38 | 🌐 Fennel | 📅 2026-01-25 - A refined successor of Lightspeed, aiming to establish a widely accepted standard interface extension for moving around in Vim-like editors.
* [folke/flash.nvim](https://github.com/folke/flash.nvim) ⭐ 3,895 | 🐛 19 | 🌐 Lua | 📅 2025-10-28 - Navigate your code with search labels, enhanced character motions and Tree-sitter integration.
* [ggandor/lightspeed.nvim](https://github.com/ggandor/lightspeed.nvim) ⭐ 1,557 | 🐛 25 | 🌐 Fennel | 📅 2023-12-01 - A Sneak-like plugin offering unparalleled navigation speed via ahead-of-time displayed labels, that eliminate the pause between entering the search pattern and selecting the target.
* [tris203/precognition.nvim](https://github.com/tris203/precognition.nvim) ⭐ 1,309 | 🐛 13 | 🌐 Lua | 📅 2026-01-31 - Precognition uses virtual text and gutter signs to show available motions.
* [abecodes/tabout.nvim](https://github.com/abecodes/tabout.nvim) ⭐ 846 | 🐛 6 | 🌐 Lua | 📅 2024-12-10 - Jump out of bracket pairs, quotes, objects, etc.
* [chrisgrieser/nvim-spider](https://github.com/chrisgrieser/nvim-spider) ⭐ 837 | 🐛 0 | 🌐 Lua | 📅 2026-02-10 - Use the w, e, b motions like a spider. Considers camelCase and skips insignificant punctuation.
* [smoka7/hop.nvim](https://github.com/smoka7/hop.nvim) ⭐ 759 | 🐛 34 | 🌐 Lua | 📅 2025-08-22 - Hop is an EasyMotion-like plugin allowing you to jump anywhere in a document with as few keystrokes as possible.
* [Aaronik/Treewalker.nvim](https://github.com/aaronik/Treewalker.nvim) ⭐ 586 | 🐛 1 | 🌐 Lua | 📅 2025-12-28 - Move seamlessly around the abstract syntax tree.
* [ggandor/flit.nvim](https://github.com/ggandor/flit.nvim) ⭐ 405 | 🐛 18 | 🌐 Lua | 📅 2025-10-09 - Enhanced f/t motions for Leap.
* [cbochs/portal.nvim](https://github.com/cbochs/portal.nvim) ⭐ 368 | 🐛 7 | 🌐 Lua | 📅 2024-06-03 - Build upon and enhance existing jumplist motions (i.e. `<c-i>` and `<c-o>`).
* [rlane/pounce.nvim](https://github.com/rlane/pounce.nvim) ⭐ 364 | 🐛 7 | 🌐 Lua | 📅 2024-09-12 - An EasyMotion-like plugin for quick cursor movement using fuzzy search.
* [ggandor/leap-spooky.nvim](https://github.com/ggandor/leap-spooky.nvim) ⭐ 281 | 🐛 8 | 🌐 Lua | 📅 2024-02-08 - Spooky (Leap) actions at a distance.
* [woosaaahh/sj.nvim](https://github.com/woosaaahh/sj.nvim) ⭐ 128 | 🐛 0 | 🌐 Lua | 📅 2023-08-06 - Search based navigation combined with quick jump features.
* [liangxianzhe/nap.nvim](https://github.com/liangxianzhe/nap.nvim) ⭐ 102 | 🐛 1 | 🌐 Lua | 📅 2023-11-13 - Jump between next/previous buffer, tab, diagnostic, etc, with a single key.
* [rasulomaroff/telepath.nvim](https://github.com/rasulomaroff/telepath.nvim) ⭐ 70 | 🐛 1 | 🌐 Lua | 📅 2024-05-02 - Another Leap extension for performing remote actions with a different approach.
* [HawkinsT/pathfinder.nvim](https://github.com/HawkinsT/pathfinder.nvim) ⭐ 61 | 🐛 3 | 🌐 Lua | 📅 2025-11-17 - Enhances gf/gF/gx with look-ahead and smarter file, line/column number, and link resolution. Also provides visual targets for files/links, new motion commands, and link description retrieval.
* [backdround/neowords.nvim](https://github.com/backdround/neowords.nvim) ⭐ 60 | 🐛 2 | 🌐 Lua | 📅 2024-09-04 - Hops by any type of words. It gives fine control over `w`, `e`, `b`, `ge` movements.
* [backdround/improved-ft.nvim](https://github.com/backdround/improved-ft.nvim) ⭐ 43 | 🐛 1 | 🌐 Lua | 📅 2024-01-16 - Improve default `f`/`t` abilities.
* [kiyoon/repeatable-move.nvim](https://github.com/kiyoon/repeatable-move.nvim) ⭐ 18 | 🐛 0 | 🌐 Lua | 📅 2026-01-25 - Make any motion repeatable with `;` and `,` keys.
* [xiaoshihou514/squirrel.nvim](https://github.com/xiaoshihou514/squirrel.nvim) ⭐ 15 | 🐛 0 | 🌐 Lua | 📅 2024-01-04 - Quickly jump between Tree-sitter nodes.
* [timseriakov/spamguard.nvim](https://github.com/timseriakov/spamguard.nvim) ⭐ 11 | 🐛 0 | 🌐 Lua | 📅 2025-05-05 - Detects excessive key spamming (jjjj/kkkk) and suggests more efficient alternatives.
* [nolleh/warp.nvim](https://github.com/nolleh/warp.nvim) ⭐ 10 | 🐛 0 | 🌐 Lua | 📅 2026-02-04 - Jump based on labels to file paths, URLs, and Markdown links from any buffer.
* [Mr-LLLLL/treesitter-outer](https://github.com/Mr-LLLLL/treesitter-outer) ⭐ 9 | 🐛 0 | 🌐 Scheme | 📅 2024-06-10 - Jump to outer node with smart.
* [millerjason/neovimacs.nvim](https://github.com/millerjason/neovimacs.nvim) ⭐ 4 | 🐛 0 | 🌐 Vim Script | 📅 2025-01-18 - Provides Emacs movement and buffer keybindings while in insert mode.
* [cosmicbuffalo/eyeliner.nvim](https://github.com/cosmicbuffalo/eyeliner.nvim) ⭐ 3 | 🐛 0 | 🌐 Lua | 📅 2026-01-06 - Highlight jump destinations for `f`/`t` motions.

### Tree-sitter Based

* [mfussenegger/nvim-treehopper](https://github.com/mfussenegger/nvim-treehopper) ⭐ 457 | 🐛 7 | 🌐 Lua | 📅 2025-06-16 - Region selection with hints on the AST nodes of a document powered by Tree-sitter.
* [drybalka/tree-climber.nvim](https://github.com/drybalka/tree-climber.nvim) ⭐ 155 | 🐛 0 | 🌐 Lua | 📅 2025-12-26 - Easy navigation around the Tree-sitter's tree that works in multi-language files and in normal mode.
* [kiyoon/treesitter-indent-object.nvim](https://github.com/kiyoon/treesitter-indent-object.nvim) ⭐ 71 | 🐛 1 | 🌐 Lua | 📅 2025-10-31 - Context-aware indent textobject powered by Tree-sitter.
* [atusy/treemonkey.nvim](https://github.com/atusy/treemonkey.nvim) ⭐ 36 | 🐛 1 | 🌐 Lua | 📅 2025-06-08 - Region selection with Tree-sitter nodes.
* [subev/sibling-jump.nvim](https://github.com/subev/sibling-jump.nvim) ⭐ 15 | 🐛 0 | 🌐 Lua | 📅 2026-02-03 - Context-aware navigation between sibling Tree-sitter nodes.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Keybinding

* [nvim-mini/mini.nvim#mini.clue](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-clue.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` to show next key clues. Has opt-in triggers, shows next key information after customizable delay, allows hydra-like submodes, and more.
* [nvim-mini/mini.nvim#mini.keymap](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-keymap.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` with utilities to make special key mappings: multi-step actions (with built-in steps for "smart" `<Tab>`, `<S-Tab>`, `<CR>`, `<BS>`), combos (more general version of "better escape" like behavior).
* [folke/which-key.nvim](https://github.com/folke/which-key.nvim) ⭐ 6,939 | 🐛 38 | 🌐 Lua | 📅 2025-10-28 - Shows a popup with possible keybindings of the command you started typing.
* [mrjones2014/legendary.nvim](https://github.com/mrjones2014/legendary.nvim) ⚠️ Archived - Define your keymaps, commands, and autocommands as simple Lua tables, and create a legend for them at the same time (like VSCode's Command Palette), integrates with `which-key.nvim`.
* [max397574/better-escape.nvim](https://github.com/max397574/better-escape.nvim) ⭐ 776 | 🐛 6 | 🌐 Lua | 📅 2025-04-29 - Create shortcuts to escape insert mode without getting delay.
* [FeiyouG/commander.nvim](https://github.com/FeiyouG/commander.nvim) ⭐ 418 | 🐛 7 | 🌐 Lua | 📅 2024-06-08 - Create and manage keybindings and commands in a more organized manner and search them quickly through Telescope.
* [chrisgrieser/nvim-recorder](https://github.com/chrisgrieser/nvim-recorder) ⭐ 274 | 🐛 0 | 🌐 Lua | 📅 2026-02-06 - Simplifying and improving how you interact with macros.
* [nvimtools/hydra.nvim](https://github.com/nvimtools/hydra.nvim) ⭐ 267 | 🐛 8 | 🌐 Lua | 📅 2025-05-03 - Create custom submodes and menus. Port of Emacs Hydra. Maintained fork of anuvyklack/hydra.nvim.
* [tris203/hawtkeys.nvim](https://github.com/tris203/hawtkeys.nvim) ⭐ 238 | 🐛 6 | 🌐 Lua | 📅 2024-05-15 - Suggest new easy-to-hit keymaps and find issues with your current keymap configurations.
* [LionC/nest.nvim](https://github.com/LionC/nest.nvim) ⭐ 236 | 🐛 9 | 🌐 Lua | 📅 2022-10-28 - Lua utility to map keys concisely using cascading trees. Also allows binding Lua functions to keys.
* [Wansmer/langmapper.nvim](https://github.com/Wansmer/langmapper.nvim) ⭐ 231 | 🐛 1 | 🌐 Lua | 📅 2025-05-05 - Auto translating your mappings for non-English input methods.
* [mawkler/demicolon.nvim](https://github.com/mawkler/demicolon.nvim) ⭐ 114 | 🐛 0 | 🌐 Lua | 📅 2026-01-25 - Use `;` and `,` keys to also repeat jumps to diagnostics (e.g. `]d`) and to [nvim-treesitter-textobjects](https://github.com/nvim-treesitter/nvim-treesitter-textobjects?tab=readme-ov-file#text-objects-move) ⭐ 2,673 | 🐛 110 | 🌐 Tree-sitter Query | 📅 2026-01-28 (e.g. `]f`), in addition to repeating `t`/`T`/`f`/`F`.
* [zdcthomas/yop.nvim](https://github.com/zdcthomas/yop.nvim) ⭐ 84 | 🐛 3 | 🌐 Lua | 📅 2023-05-29 - Easily create your own operators (like `d` and `y`).
* [Nexmean/caskey.nvim](https://github.com/Nexmean/caskey.nvim) ⚠️ Archived - Utility to keymappings configuration using declarative cascading trees, optionally integrates with `which-key`.
* [Iron-E/nvim-cartographer](https://github.com/Iron-E/nvim-cartographer) ⭐ 55 | 🐛 0 | 🌐 Lua | 📅 2023-06-19 - A more convenient `:map`ping syntax for Lua environments.
* [TheBlob42/houdini.nvim](https://github.com/TheBlob42/houdini.nvim) ⭐ 41 | 🐛 1 | 🌐 Lua | 📅 2024-07-05 - Create shortcut to escape modes without delay.
* [slugbyte/unruly-worker.nvim](https://github.com/slugbyte/unruly-worker.nvim) ⭐ 38 | 🐛 1 | 🌐 Lua | 📅 2025-12-22 - A ridiculously fun alternative keymap for the workman keyboard layout, with lots of powerful features for working with yank, marks, macros, LSP, and more. Built and configured with Lua.
* [RutaTang/compter.nvim](https://github.com/RutaTang/compter.nvim) ⭐ 29 | 🐛 1 | 🌐 Lua | 📅 2023-06-01 - Power and extend the ability of `<C-a>` and `<C-x>` with customized patterns.
* [sontungexpt/bim.nvim](https://github.com/sontungexpt/bim.nvim) ⭐ 11 | 🐛 1 | 🌐 Lua | 📅 2025-11-23 - Enhances insert mode key mapping by showing typed keys in real time, without waiting for timeoutlen. It provides a responsive and intuitive insert-mode experience, ideal for complex input workflows like ime.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Mouse

* [notomo/gesture.nvim](https://github.com/notomo/gesture.nvim) ⭐ 536 | 🐛 0 | 🌐 Lua | 📅 2025-10-08 - Mouse gesture plugin.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Scrolling

* [karb94/neoscroll.nvim](https://github.com/karb94/neoscroll.nvim) ⭐ 1,969 | 🐛 11 | 🌐 Lua | 📅 2025-12-31 - Smooth scrolling.
* [declancm/cinnamon.nvim](https://github.com/declancm/cinnamon.nvim) ⭐ 396 | 🐛 8 | 🌐 Lua | 📅 2024-08-07 - Smooth scrolling for any movement command.
* [saghen/filler-begone.nvim](https://github.com/saghen/filler-begone.nvim) ⭐ 20 | 🐛 0 | 🌐 Lua | 📅 2025-10-30 - Prevents scrolling past the bottom of the buffer and showing unnecessary filler lines.
* [niuiic/scroll.nvim](https://github.com/niuiic/scroll.nvim) ⭐ 18 | 🐛 0 | 🌐 Lua | 📅 2024-05-24 - Smooth scrolling, custom smooth strategy.
* [rlychrisg/keepcursor.nvim](https://github.com/rlychrisg/keepcursor.nvim) ⭐ 11 | 🐛 0 | 🌐 Lua | 📅 2024-08-23 - A collection of functions to control how the screen is positioned around the cursor.

### Scrollbar

* [nvim-mini/mini.nvim#mini.map](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-map.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` to show floating window with buffer text overview, scrollbar, and highlights.
* [petertriho/nvim-scrollbar](https://github.com/petertriho/nvim-scrollbar) ⭐ 1,026 | 🐛 30 | 🌐 Lua | 📅 2025-11-17 - Extensible scrollbar that shows diagnostics and search results.
* [lewis6991/satellite.nvim](https://github.com/lewis6991/satellite.nvim) ⭐ 698 | 🐛 16 | 🌐 Lua | 📅 2026-01-22 - Decorate scrollbar.
* [dstein64/nvim-scrollview](https://github.com/dstein64/nvim-scrollview) ⭐ 682 | 🐛 4 | 🌐 Lua | 📅 2026-02-16 - Display interactive scrollbars.
* [gorbit99/codewindow.nvim](https://github.com/gorbit99/codewindow.nvim) ⭐ 477 | 🐛 27 | 🌐 Lua | 📅 2025-05-22 - Minimap plugin, that is closely integrated with Tree-sitter and the built-in LSP to display more information to the user.
* [Xuyuanp/scrollbar.nvim](https://github.com/Xuyuanp/scrollbar.nvim) ⭐ 281 | 🐛 9 | 🌐 Lua | 📅 2025-03-23 - Scrollbar.
* [wsdjeg/scrollbar.nvim](https://github.com/wsdjeg/scrollbar.nvim) ⭐ 23 | 🐛 1 | 🌐 Lua | 📅 2025-12-24 - Floating scrollbar.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Editing Support

* [nvim-mini/mini.nvim#mini.pairs](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-pairs.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` for autopairs which has minimal defaults and functionality to do per-key mapping.
* [nvim-mini/mini.nvim#mini.trailspace](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-trailspace.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` for automatic highlighting of trailing whitespace with functionality to remove it.
* [nvim-mini/mini.nvim#mini.operators](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-operators.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` with various text edit operators: replace, exchange, multiply, sort, evaluate.
* [nvim-mini/mini.nvim#mini.move](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-move.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` to move any selection (charwise, linewise, blockwise, current line in Normal mode) in any direction. Handles both `v:count` and undo history.
* [nvim-mini/mini.nvim#mini.ai](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-ai.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` for extending and creating `a`/`i` textobjects. It enhances some built-in textobjects, creates extensive set of new ones (like `a*`, `a<Space>`, `a?`, and more), and allows user to create their own (via Lua patterns or functions). Supports dot-repeat, different search methods, consecutive application, and more.
* [nvim-mini/mini.nvim#mini.splitjoin](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-splitjoin.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` to split and join arguments. Has customizable pre and post hooks. Works inside comments.
* [nvim-mini/mini.nvim#mini.basics](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-basics.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` with customizable configuration presets for common options, mappings, and autocommands.
* [windwp/nvim-autopairs](https://github.com/windwp/nvim-autopairs) ⭐ 3,938 | 🐛 17 | 🌐 Lua | 📅 2026-01-30 - A minimalist autopairs written by Lua.
* [nvim-treesitter/nvim-treesitter-context](https://github.com/nvim-treesitter/nvim-treesitter-context) ⭐ 3,118 | 🐛 18 | 🌐 Janet | 📅 2025-12-06 - Shows floating hover with the current function/block context.
* [folke/zen-mode.nvim](https://github.com/folke/zen-mode.nvim) ⭐ 2,095 | 🐛 15 | 🌐 Lua | 📅 2025-10-28 - Distraction-free coding.
* [windwp/nvim-ts-autotag](https://github.com/windwp/nvim-ts-autotag) ⭐ 2,053 | 🐛 8 | 🌐 Lua | 📅 2026-02-04 - Use Tree-sitter to autoclose and autorename XML, HTML, JSX tag.
* [jake-stewart/multicursor.nvim](https://github.com/jake-stewart/multicursor.nvim) ⭐ 1,387 | 🐛 0 | 🌐 Lua | 📅 2026-02-01 - Adds support for multiple cursors which work how you expect.
* [Wansmer/treesj](https://github.com/Wansmer/treesj) ⭐ 1,302 | 🐛 5 | 🌐 Lua | 📅 2025-12-08 - Splitting/joining blocks of code like arrays, hashes, statements, objects, dictionaries, etc. Using Tree-sitter. Inspired by greatest splitjoin.vim.
* [gbprod/yanky.nvim](https://github.com/gbprod/yanky.nvim) ⭐ 1,208 | 🐛 33 | 🌐 Lua | 📅 2026-02-09 - Improved Yank and Put functionalities.
* [monaqa/dial.nvim](https://github.com/monaqa/dial.nvim) ⭐ 1,046 | 🐛 17 | 🌐 Lua | 📅 2025-12-21 - Extended increment/decrement.
* [cshuaimin/ssr.nvim](https://github.com/cshuaimin/ssr.nvim) ⭐ 986 | 🐛 18 | 🌐 Lua | 📅 2024-09-07 - Tree-sitter based structural search and replace.
* [shortcuts/no-neck-pain.nvim](https://github.com/shortcuts/no-neck-pain.nvim) ⭐ 905 | 🐛 15 | 🌐 Lua | 📅 2026-02-17 - Center the currently focused buffer to the middle of your terminal.
* [nacro90/numb.nvim](https://github.com/nacro90/numb.nvim) ⭐ 840 | 🐛 1 | 🌐 Lua | 📅 2026-01-17 - Peek lines in a non-obtrusive way.
* [HiPhish/rainbow-delimiters.nvim](https://github.com/HiPhish/rainbow-delimiters.nvim) ⭐ 834 | 🐛 19 | 🌐 Lua | 📅 2026-02-16 - Rainbow delimiters with Tree-sitter.
* [debugloop/telescope-undo.nvim](https://github.com/debugloop/telescope-undo.nvim) ⭐ 788 | 🐛 5 | 🌐 Lua | 📅 2025-01-31 - A telescope extension to visualize your undo tree and fuzzy-search changes in it.
* [chrisgrieser/nvim-various-textobjs](https://github.com/chrisgrieser/nvim-various-textobjs) ⭐ 751 | 🐛 0 | 🌐 Lua | 📅 2026-02-10 - Bundle of more than 30 new text objects.
* [gbprod/substitute.nvim](https://github.com/gbprod/substitute.nvim) ⭐ 725 | 🐛 5 | 🌐 Lua | 📅 2026-02-17 - New operator motions to quickly replace and exchange text.
* [smoka7/multicursors.nvim](https://github.com/smoka7/multicursors.nvim) ⭐ 636 | 🐛 13 | 🌐 Lua | 📅 2025-02-26 - Provides a more intuitive way to edit repetitive text with multiple selections.
* [m4xshen/autoclose.nvim](https://github.com/m4xshen/autoclose.nvim) ⭐ 632 | 🐛 12 | 🌐 Lua | 📅 2025-07-21 - A minimalist autoclose plugin written in Lua.
* [altermo/ultimate-autopair.nvim](https://github.com/altermo/ultimate-autopair.nvim) ⭐ 566 | 🐛 22 | 🌐 Lua | 📅 2025-11-05 - Autopair with extensions.
* [smjonas/live-command.nvim](https://github.com/smjonas/live-command.nvim) ⭐ 539 | 🐛 10 | 🌐 Lua | 📅 2025-12-19 - Text editing with immediate visual feedback: preview commands such as `:norm`, `:g`, macros and more.
* [mizlan/iswap.nvim](https://github.com/mizlan/iswap.nvim) ⭐ 523 | 🐛 12 | 🌐 Lua | 📅 2024-08-10 - Interactively select and swap function arguments, list elements, and more. Powered by Tree-sitter.
* [andersevenrud/nvim\_context\_vt](https://github.com/andersevenrud/nvim_context_vt) ⭐ 410 | 🐛 5 | 🌐 Lua | 📅 2025-09-17 - Shows virtual text of the current context.
* [brenton-leighton/multiple-cursors.nvim](https://github.com/brenton-leighton/multiple-cursors.nvim) ⭐ 390 | 🐛 1 | 🌐 Lua | 📅 2026-01-02 - A multi-cursor plugin that works in normal, insert/replace, or visual modes, and with almost every command.
* [ckolkey/ts-node-action](https://github.com/CKolkey/ts-node-action) ⭐ 375 | 🐛 15 | 🌐 Lua | 📅 2026-01-16 - A framework for executing functional transformations on Tree-sitter nodes.
* [zbirenbaum/neodim](https://github.com/zbirenbaum/neodim) ⭐ 338 | 🐛 5 | 🌐 Lua | 📅 2025-01-09 - Dimming the highlights of unused functions, variables, parameters, and more.
* [keaising/im-select.nvim](https://github.com/keaising/im-select.nvim) ⭐ 326 | 🐛 7 | 🌐 Lua | 📅 2025-07-24 - Switching and restoring input method automatically depends on Neovim's edit mode.
* [filipdutescu/renamer.nvim](https://github.com/filipdutescu/renamer.nvim) ⭐ 314 | 🐛 10 | 🌐 Lua | 📅 2024-01-04 - VSCode-like renaming UI, written in Lua.
* [okuuva/auto-save.nvim](https://github.com/okuuva/auto-save.nvim) ⭐ 305 | 🐛 2 | 🌐 Lua | 📅 2026-02-07 - Automatically saves your work as often as needed and as seldom as possible. Customizable with smart defaults. Maintained fork of Pocco81/auto-save.nvim.
* [tomiis4/hypersonic.nvim](https://github.com/tomiis4/hypersonic.nvim) ⭐ 230 | 🐛 4 | 🌐 Lua | 📅 2024-08-11 - Provides explanation for RegExp.
* [gbprod/cutlass.nvim](https://github.com/gbprod/cutlass.nvim) ⭐ 222 | 🐛 2 | 🌐 Lua | 📅 2025-10-23 - Plugin that adds a 'cut' operation separate from 'delete'.
* [sQVe/sort.nvim](https://github.com/sQVe/sort.nvim) ⭐ 206 | 🐛 0 | 🌐 Lua | 📅 2026-01-28 - Sorting plugin that intelligently supports line-wise and delimiter sorting.
* [booperlv/nvim-gomove](https://github.com/booperlv/nvim-gomove) ⭐ 205 | 🐛 4 | 🌐 Lua | 📅 2022-07-19 - A complete plugin for moving and duplicating blocks and lines, with complete fold handling, reindenting, and undoing in one go.
* [nguyenvukhang/nvim-toggler](https://github.com/nguyenvukhang/nvim-toggler) ⭐ 190 | 🐛 3 | 🌐 Lua | 📅 2024-06-15 - Invert text, such as toggling between `true` and `false`.
* [nat-418/boole.nvim](https://github.com/nat-418/boole.nvim) ⭐ 183 | 🐛 12 | 🌐 Lua | 📅 2024-06-06 - Toggle booleans and common string values.
* [Wansmer/sibling-swap.nvim](https://github.com/Wansmer/sibling-swap.nvim) ⭐ 180 | 🐛 3 | 🌐 Lua | 📅 2025-05-29 - Different way to swapping arguments and other siblings with Tree-sitter.
* [AckslD/nvim-trevJ.lua](https://github.com/AckslD/nvim-trevJ.lua) ⭐ 171 | 🐛 6 | 🌐 Lua | 📅 2025-07-21 - Does the opposite of join-line (J) for arguments, powered by Tree-sitter.
* [gregorias/coerce.nvim](https://github.com/gregorias/coerce.nvim) ⭐ 162 | 🐛 0 | 🌐 Lua | 📅 2025-07-24 - Change keyword case.
* [willothy/moveline.nvim](https://github.com/willothy/moveline.nvim) ⭐ 153 | 🐛 6 | 🌐 Rust | 📅 2025-09-22 - Move lines and blocks up and down easily, with indenting handled automatically as you move. Written in Rust.
* [XXiaoA/atone.nvim](https://github.com/XXiaoA/atone.nvim) ⭐ 146 | 🐛 5 | 🌐 Lua | 📅 2025-11-14 - Undo tree for visualizing and managing undo history.
* [ZhiyuanLck/smart-pairs](https://github.com/ZhiyuanLck/smart-pairs) ⭐ 134 | 🐛 7 | 🌐 Lua | 📅 2025-11-23 - Ultimate smart pairs written by Lua.
* [ptdewey/yankbank-nvim](https://github.com/ptdewey/yankbank-nvim) ⭐ 124 | 🐛 0 | 🌐 Lua | 📅 2026-01-17 - Enable streamlined access to recent yanks and deletions in a quick-access popup menu.
* [OXY2DEV/foldtext.nvim](https://github.com/OXY2DEV/foldtext.nvim) ⭐ 118 | 🐛 1 | 🌐 Lua | 📅 2025-09-24 - Dynamic and stylized foldtext.
* [gbprod/stay-in-place.nvim](https://github.com/gbprod/stay-in-place.nvim) ⭐ 101 | 🐛 1 | 🌐 Lua | 📅 2023-01-23 - Prevent the cursor from moving when using shift and filter actions.
* [tummetott/unimpaired.nvim](https://github.com/tummetott/unimpaired.nvim) ⭐ 99 | 🐛 1 | 🌐 Lua | 📅 2025-10-16 - Lua port of [tpope/vim-unimpaired](https://github.com/tpope/vim-unimpaired) ⭐ 3,446 | 🐛 57 | 🌐 Vim Script | 📅 2025-08-16.
* [h-hg/fcitx.nvim](https://github.com/h-hg/fcitx.nvim) ⭐ 98 | 🐛 3 | 🌐 Lua | 📅 2025-12-28 - Switching and restoring fcitx state for each buffer separately.
* [SunnyTamang/select-undo.nvim](https://github.com/SunnyTamang/select-undo.nvim) ⭐ 96 | 🐛 1 | 🌐 Lua | 📅 2025-02-08 - Allow users to undo specific line/lines or partial selections without affecting the rest of the file.
* [bennypowers/splitjoin.nvim](https://github.com/bennypowers/splitjoin.nvim) ⭐ 82 | 🐛 3 | 🌐 Lua | 📅 2026-01-29 - Split and join various syntax structures.
* [Jxstxs/conceal.nvim](https://github.com/Jxstxs/conceal.nvim) ⭐ 76 | 🐛 1 | 🌐 Lua | 📅 2024-07-07 - Use Tree-sitter to conceal common boilerplate code.
* [nemanjamalesija/smart-paste.nvim](https://github.com/nemanjamalesija/smart-paste.nvim) ⭐ 74 | 🐛 1 | 🌐 Lua | 📅 2026-02-15 - Automatic indentation of pasted code using a three-tier indent strategy (indentexpr / Tree-sitter / heuristic).
* [chrisgrieser/nvim-puppeteer](https://github.com/chrisgrieser/nvim-puppeteer) ⭐ 73 | 🐛 1 | 🌐 Lua | 📅 2026-02-06 - Automatically convert strings to f-strings or template strings and back.
* [kiyoon/telescope-insert-path.nvim](https://github.com/kiyoon/telescope-insert-path.nvim) ⭐ 44 | 🐛 1 | 🌐 Lua | 📅 2025-12-20 - Insert file path in the current buffer using Telescope.
* [attilarepka/header.nvim](https://github.com/attilarepka/header.nvim) ⭐ 38 | 🐛 1 | 🌐 Lua | 📅 2025-11-25 - Add or update copyright and license headers in any source file.
* [XXiaoA/ns-textobject.nvim](https://github.com/XXiaoA/ns-textobject.nvim) ⭐ 36 | 🐛 4 | 🌐 Lua | 📅 2023-05-26 - Awesome textobject plugin works with nvim-surround.
* [Allendang/nvim-expand-expr](https://github.com/AllenDang/nvim-expand-expr) ⭐ 35 | 🐛 0 | 🌐 Lua | 📅 2021-08-14 - Expand and repeat expression to multiple lines.
* [altermo/iedit.nvim](https://github.com/altermo/iedit.nvim) ⭐ 35 | 🐛 0 | 🌐 Lua | 📅 2026-01-07 - Edit one occurrence of text and simultaneously have other selected occurrences edited in the same way.
* [wurli/split.nvim](https://github.com/wurli/split.nvim) ⭐ 34 | 🐛 1 | 🌐 Lua | 📅 2025-02-07 - Provides a mapping to split text by delimiter, giving an inverse of the native J command.
* [csessh/stopinsert.nvim](https://github.com/csessh/stopinsert.nvim) ⭐ 32 | 🐛 0 | 🌐 Lua | 📅 2025-08-01 - Automatically exit Insert mode after inactivity.
* [niuiic/divider.nvim](https://github.com/niuiic/divider.nvim) ⭐ 30 | 🐛 0 | 🌐 Lua | 📅 2024-11-18 - Custom code divider line.
* [zhisme/copy\_with\_context.nvim](https://github.com/zhisme/copy_with_context.nvim) ⭐ 28 | 🐛 4 | 🌐 Lua | 📅 2026-01-29 - Copy lines with file path and line number metadata for sharing code snippets with context.
* [qwavies/smart-backspace.nvim](https://github.com/qwavies/smart-backspace.nvim) ⭐ 26 | 🐛 0 | 🌐 Lua | 📅 2026-02-16 - Context-aware backspace which handles pairs, whitespace and indentation.
* [hinell/duplicate.nvim](https://github.com/hinell/duplicate.nvim) ⭐ 24 | 🐛 0 | 🌐 Lua | 📅 2023-10-23 - Duplicate lines and blocks of lines easily; undo and unfolding support; full OOP.
* [nxhung2304/lastplace.nvim](https://github.com/nxhung2304/lastplace.nvim) ⭐ 23 | 🐛 0 | 🌐 Shell | 📅 2025-06-30 - Intelligently restore your cursor position when reopening files.
* [rlychrisg/truncateline.nvim](https://github.com/rlychrisg/truncateline.nvim) ⭐ 21 | 🐛 0 | 🌐 Lua | 📅 2026-01-14 - Truncate long lines to keep track of where you are when the start gets lost off the left side of the screen.
* [tmillr/sos.nvim](https://github.com/tmillr/sos.nvim) ⭐ 21 | 🐛 12 | 🌐 Lua | 📅 2024-12-07 - Automatically save all your modified buffers according to a predefined timeout value.
* [daltongd/yanklock.nvim](https://github.com/daltongd/yanklock.nvim) ⭐ 20 | 🐛 0 | 🌐 Lua | 📅 2025-01-03 - Temporarily lock the paste register to `"0`, and use `d`, `c`, and `s` motions while keeping the most recent yanked content easily accessible.
* [necrom4/convy.nvim](https://github.com/necrom4/convy.nvim) ⭐ 19 | 🐛 1 | 🌐 Lua | 📅 2025-11-11 - Easily convert strings between various formats.
* [Wansmer/binary-swap.nvim](https://github.com/Wansmer/binary-swap.nvim) ⚠️ Archived - Swapping operands and operators in binary expressions: comparison and mathematical operations.
* [tigion/swap.nvim](https://github.com/tigion/swap.nvim) ⭐ 17 | 🐛 0 | 🌐 Lua | 📅 2025-10-08 - Quickly switch a word under the cursor or a pattern in the current line.
* [niuiic/part-edit.nvim](https://github.com/niuiic/part-edit.nvim) ⭐ 15 | 🐛 0 | 🌐 Lua | 📅 2026-01-16 - Edit a part of a file individually.
* [hinell/move.nvim](https://github.com/hinell/move.nvim) ⭐ 13 | 🐛 0 | 🌐 Lua | 📅 2023-10-25 - Move chunks of text around; fork of [fedepujol/move.nvim](https://github.com/fedepujol/move.nvim) ⭐ 363 | 🐛 8 | 🌐 Lua | 📅 2025-05-13.
* [saifulapm/commasemi.nvim](https://github.com/saifulapm/commasemi.nvim) ⭐ 12 | 🐛 0 | 🌐 Lua | 📅 2025-03-06 - Toggle comma and semicolon.
* [zongben/capsoff.nvim](https://github.com/zongben/capsoff.nvim) ⭐ 12 | 🐛 0 | 🌐 Lua | 📅 2024-12-27 - Turns off CapsLock when you leaving insert mode.
* [kobbikobb/move-lines.nvim](https://github.com/kobbikobb/move-lines.nvim) ⭐ 8 | 🐛 1 | 🌐 Lua | 📅 2025-01-01 - Moves lines selected in virtual mode.
* [hiberabyss/bzlops.vim](https://github.com/hiberabyss/bzlops.vim) ⭐ 4 | 🐛 0 | 🌐 Vim Script | 📅 2023-12-21 - Help to manage your bazel build rule.
* [TheLazyCat00/replace-nvim](https://github.com/TheLazyCat00/replace-nvim) ⭐ 1 | 🐛 0 | 🌐 Lua | 📅 2025-05-07 - Replace part of your code with the contents of the `+` register using textobjects.
* [\~nedia/auto-save.nvim](https://git.sr.ht/~nedia/auto-save.nvim) - Extremely simple auto saving on `InsertLeave` and `TextChanged`. Based on Pocco81/AutoSave but lighter.

### Comment

* [nvim-mini/mini.nvim#mini.comment](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-comment.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` for per-line commenting. Fully supports dot-repeat.
* [numToStr/Comment.nvim](https://github.com/numToStr/Comment.nvim) ⭐ 4,583 | 🐛 80 | 🌐 Lua | 📅 2024-08-19 - Smart and powerful comment plugin. Supports commentstring, motions, dot-repeat and more.
* [folke/todo-comments.nvim](https://github.com/folke/todo-comments.nvim) ⭐ 4,050 | 🐛 23 | 🌐 Lua | 📅 2025-11-10 - Highlight, list and search TODO comments in your projects.
* [danymat/neogen](https://github.com/danymat/neogen) ⭐ 1,620 | 🐛 44 | 🌐 Lua | 📅 2026-01-10 - A better annotation generator which supports multiple languages and annotation conventions.
* [JoosepAlviste/nvim-ts-context-commentstring](https://github.com/JoosepAlviste/nvim-ts-context-commentstring) ⭐ 1,279 | 🐛 22 | 🌐 Lua | 📅 2024-12-07 - Sets the `commentstring` option based on the cursor location in the file. The location is checked via Tree-sitter queries.
* [b3nj5m1n/kommentary](https://github.com/b3nj5m1n/kommentary) ⭐ 532 | 🐛 8 | 🌐 Lua | 📅 2023-11-29 - Commenting plugin written in Lua.
* [terrortylor/nvim-comment](https://github.com/terrortylor/nvim-comment) ⭐ 494 | 🐛 14 | 🌐 Lua | 📅 2024-05-29 - Toggle comments using the built-in commentstring option.
* [LudoPinelli/comment-box.nvim](https://github.com/LudoPinelli/comment-box.nvim) ⭐ 477 | 🐛 15 | 🌐 Lua | 📅 2024-08-10 - Clarify and beautify your comments using boxes and lines.
* [winston0410/commented.nvim](https://github.com/winston0410/commented.nvim) ⭐ 115 | 🐛 4 | 🌐 Lua | 📅 2022-03-12 - A commenting plugin which supports counts and multiple comment patterns and much more.
* [s1n7ax/nvim-comment-frame](https://github.com/s1n7ax/nvim-comment-frame) ⭐ 100 | 🐛 1 | 🌐 Lua | 📅 2025-08-05 - Adds a comment frame based on the source file.
* [Zeioth/dooku.nvim](https://github.com/Zeioth/dooku.nvim) ⭐ 49 | 🐛 0 | 🌐 Lua | 📅 2025-06-24 - Generate and open your HTML code documentation.
* [gennaro-tedesco/nvim-commaround](https://github.com/gennaro-tedesco/nvim-commaround) ⭐ 42 | 🐛 0 | 🌐 Lua | 📅 2023-01-06 - Fast and light commenting plugin written in Lua.
* [georgeharker/comment-tasks.nvim](https://github.com/georgeharker/comment-tasks.nvim) ⭐ 14 | 🐛 0 | 🌐 Lua | 📅 2025-10-27 - Keep your task manager up to date from TODO and FIXME comments in code.
* [alexmozaidze/tree-comment.nvim](https://github.com/alexmozaidze/tree-comment.nvim) ⭐ 10 | 🐛 1 | 🌐 Fennel | 📅 2025-11-19 - Highlight and configure TODO comments for [tree-sitter-comment](https://github.com/stsewd/tree-sitter-comment) ⭐ 164 | 🐛 12 | 🌐 C | 📅 2025-12-16.
* [LucasTavaresA/SingleComment.nvim](https://github.com/LucasTavaresA/SingleComment.nvim) ⭐ 9 | 🐛 1 | 🌐 Lua | 📅 2025-08-27 - Always single line, comment sensitive, indentation preserving commenting.

### Folding

* [kevinhwang91/nvim-ufo](https://github.com/kevinhwang91/nvim-ufo) ⭐ 2,880 | 🐛 46 | 🌐 Lua | 📅 2026-01-11 - Ultra fold with modern looking and performance boosting.
* [chrisgrieser/nvim-origami](https://github.com/chrisgrieser/nvim-origami) ⭐ 458 | 🐛 2 | 🌐 Lua | 📅 2026-02-10 - Fold with relentless elegance.
* [jghauser/fold-cycle.nvim](https://github.com/jghauser/fold-cycle.nvim) ⭐ 92 | 🐛 0 | 🌐 Lua | 📅 2025-08-31 - Cycle folds open or closed.
* [malbertzard/inline-fold.nvim](https://github.com/malbertzard/inline-fold.nvim) ⭐ 89 | 🐛 4 | 🌐 Lua | 📅 2023-08-12 - Hide certain elements inline like long CSS classes or `href` content.
* [soemre/commentless.nvim](https://github.com/soemre/commentless.nvim) ⭐ 40 | 🐛 0 | 🌐 Lua | 📅 2025-04-26 - Fold all comments to better visualize your code logic, and unfold them whenever needed.
* [yaocccc/nvim-foldsign](https://github.com/yaocccc/nvim-foldsign) ⭐ 39 | 🐛 0 | 🌐 Lua | 📅 2025-03-18 - Display folds on sign column.
* [netmute/foldsigns.nvim](https://github.com/netmute/foldsigns.nvim) ⭐ 4 | 🐛 0 | 🌐 Lua | 📅 2026-01-19 - Adds fold markers to sign column to make folds more visible while editing.
* [netmute/foldchanged.nvim](https://github.com/netmute/foldchanged.nvim) ⭐ 2 | 🐛 0 | 🌐 Lua | 📅 2026-01-19 - Adds a `FoldChanged` User event.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Formatting

* [nvim-mini/mini.nvim#mini.align](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-align.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` for aligning text interactively (with or without instant preview).
* [stevearc/conform.nvim](https://github.com/stevearc/conform.nvim) ⭐ 4,922 | 🐛 86 | 🌐 Lua | 📅 2026-01-18 - A lightweight formatting engine that plays nice with LSP.
* [sbdchd/neoformat](https://github.com/sbdchd/neoformat) ⭐ 2,052 | 🐛 130 | 🌐 Vim Script | 📅 2026-02-10 - A code formatting runner.
* [mhartington/formatter.nvim](https://github.com/mhartington/formatter.nvim) ⭐ 1,449 | 🐛 45 | 🌐 Lua | 📅 2025-05-29 - A format runner written in Lua.
* [nvimdev/guard.nvim](https://github.com/nvimdev/guard.nvim) ⭐ 512 | 🐛 0 | 🌐 Lua | 📅 2026-01-31 - Minimalist async formatting and linting plugin.
* [MunifTanjim/prettier.nvim](https://github.com/MunifTanjim/prettier.nvim) ⭐ 312 | 🐛 5 | 🌐 Lua | 📅 2025-04-08 - Prettier integration.
* [elentok/format-on-save.nvim](https://github.com/elentok/format-on-save.nvim) ⭐ 171 | 🐛 6 | 🌐 Lua | 📅 2025-07-20 - A synchronous formatter that combines both LSP and non-LSP formatting (e.g. `shfmt`, `stylua`, `prettier`). Focused specifically for format-on-save.
* [cappyzawa/trim.nvim](https://github.com/cappyzawa/trim.nvim) ⭐ 156 | 🐛 2 | 🌐 Lua | 📅 2025-12-30 - Trims trailing whitespace and lines.
* [emileferreira/nvim-strict](https://github.com/emileferreira/nvim-strict) ⭐ 39 | 🐛 1 | 🌐 Lua | 📅 2025-01-08 - Strict, native code style formatting which exposes deep nesting, overlong lines, trailing whitespace, trailing empty lines, TODOs and inconsistent indentation.
* [niuiic/format.nvim](https://github.com/niuiic/format.nvim) ⭐ 33 | 🐛 0 | 🌐 Lua | 📅 2025-08-02 - An asynchronous, multitasking, highly configurable formatting plugin.
* [tenxsoydev/tabs-vs-spaces.nvim](https://github.com/tenxsoydev/tabs-vs-spaces.nvim) ⭐ 26 | 🐛 1 | 🌐 Lua | 📅 2024-09-22 - Hint and fix deviating indentation.
* [wsdjeg/format.nvim](https://github.com/wsdjeg/format.nvim) ⭐ 15 | 🐛 1 | 🌐 Lua | 📅 2025-12-19 - An asynchronous code formatting plugin.
* [paul-louyot/toggle-quotes.nvim](https://github.com/paul-louyot/toggle-quotes.nvim) ⭐ 7 | 🐛 1 | 🌐 Lua | 📅 2024-11-29 - Toggle between quotes.
* [TheLazyCat00/simple-format](https://github.com/TheLazyCat00/simple-format) ⭐ 4 | 🐛 0 | 🌐 Lua | 📅 2025-12-18 - Replace text using custom regex and highlight group rules.
* [bennypowers/svgo.nvim](https://github.com/bennypowers/svgo.nvim) ⭐ 3 | 🐛 0 | 🌐 Lua | 📅 2023-11-17 - Optimize SVG files.
* [\~nedia/auto-format.nvim](https://git.sr.ht/~nedia/auto-format.nvim) - Sets up an autocommand to format on save, preferring `null-ls` over native LSP client formatting.

### Indent

* [nvim-mini/mini.nvim#mini.indentscope](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-indentscope.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` for visualizing and operating on indent scope. Supports customization of debounce delay, animation style, and different granularity of options for scope computing algorithm.
* [lukas-reineke/indent-blankline.nvim](https://github.com/lukas-reineke/indent-blankline.nvim) ⭐ 4,857 | 🐛 23 | 🌐 Lua | 📅 2026-02-17 - IndentLine replacement in Lua with more features and Tree-sitter support.
* [shellRaining/hlchunk.nvim](https://github.com/shellRaining/hlchunk.nvim) ⭐ 891 | 🐛 32 | 🌐 Lua | 📅 2025-12-15 - A Lua implementation of `nvim-hlchunk`, contains more features, such as highlight `{}` chunk, indent line, space blank etc.
* [NMAC427/guess-indent.nvim](https://github.com/NMAC427/guess-indent.nvim) ⭐ 605 | 🐛 16 | 🌐 Lua | 📅 2025-03-25 - Automatic indentation style detection.
* [nvimdev/indentmini.nvim](https://github.com/nvimdev/indentmini.nvim) ⭐ 280 | 🐛 1 | 🌐 Lua | 📅 2026-01-04 - A minimal and blazing fast indentline plugin by using the `nvim_set_decoration_provide` API function.
* [Darazaki/indent-o-matic](https://github.com/Darazaki/indent-o-matic) ⭐ 203 | 🐛 0 | 🌐 Lua | 📅 2025-11-24 - Dumb automatic fast indentation detection written in Lua.
* [saghen/blink.indent](https://github.com/saghen/blink.indent) ⭐ 185 | 🐛 6 | 🌐 Lua | 📅 2026-01-13 - Performant indent guides with scope on every keystroke.
* [VidocqH/auto-indent.nvim](https://github.com/VidocqH/auto-indent.nvim) ⭐ 89 | 🐛 0 | 🌐 Lua | 📅 2023-11-03 - Auto indent cursor when cursor at the first column and press `<TAB>` key like VSCode.
* [yaocccc/nvim-hlchunk](https://github.com/yaocccc/nvim-hlchunk) ⭐ 54 | 🐛 1 | 🌐 Vim Script | 📅 2025-08-18 - Highlight a `{}` chunk.
* [gh-liu/fold\_line.nvim](https://github.com/gh-liu/fold_line.nvim) ⭐ 54 | 🐛 1 | 🌐 Lua | 📅 2026-01-17 - Lines for indicating code folding, which could achieve an effect similar to indentline by `:set fdm=indent`.
* [Mr-LLLLL/cool-chunk.nvim](https://github.com/Mr-LLLLL/cool-chunk.nvim) ⭐ 28 | 🐛 1 | 🌐 Lua | 📅 2025-01-10 - Simpler and faster chunking with animations.
* [LucasTavaresA/simpleIndentGuides.nvim](https://github.com/LucasTavaresA/simpleIndentGuides.nvim) ⭐ 10 | 🐛 0 | 🌐 Lua | 📅 2024-11-24 - Indentation guides using the built-in variables.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Command Line

* [nvim-mini/mini.nvim#mini.cmdline](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-cmdline.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` for command line tweaks. Adds autocompletion with customizable delay, autocorrection for words with fixed candidates, and autopeek command range in a floating window.
* [gelguy/wilder.nvim](https://github.com/gelguy/wilder.nvim) ⭐ 1,471 | 🐛 63 | 🌐 Vim script | 📅 2024-07-17 - A plugin for fuzzy command line autocompletion.
* [notomo/cmdbuf.nvim](https://github.com/notomo/cmdbuf.nvim) ⭐ 135 | 🐛 0 | 🌐 Lua | 📅 2025-07-26 - Alternative command-line-window plugin.
* [vzze/cmdline.nvim](https://github.com/vzze/cmdline.nvim) ⭐ 22 | 🐛 0 | 🌐 Lua | 📅 2025-04-03 - Helix-like command line with fuzzy autocompletion.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Session

* [nvim-mini/mini.nvim#mini.sessions](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-sessions.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` for session management (read, write, delete).
* [rmagatti/auto-session](https://github.com/rmagatti/auto-session) ⭐ 1,773 | 🐛 15 | 🌐 Lua | 📅 2026-02-15 - A small automated session manager.
* [folke/persistence.nvim](https://github.com/folke/persistence.nvim) ⭐ 951 | 🐛 9 | 🌐 Lua | 📅 2025-10-28 - Simple automated session management.
* [Shatur/neovim-session-manager](https://github.com/Shatur/neovim-session-manager) ⭐ 612 | 🐛 15 | 🌐 Lua | 📅 2026-01-26 - A simple wrapper around :mksession.
* [olimorris/persisted.nvim](https://github.com/olimorris/persisted.nvim) ⭐ 526 | 🐛 0 | 🌐 Lua | 📅 2026-02-02 - Simple session management with Git branching, autosave/autoload and Telescope support.
* [jedrzejboczar/possession.nvim](https://github.com/jedrzejboczar/possession.nvim) ⭐ 393 | 🐛 13 | 🌐 Lua | 📅 2025-10-21 - Flexible session management with arbitrary persistent data stored as JSON.
* [gennaro-tedesco/nvim-possession](https://github.com/gennaro-tedesco/nvim-possession) ⭐ 283 | 🐛 3 | 🌐 Lua | 📅 2025-09-07 - The no-nonsense session manager.
* [coffebar/neovim-project](https://github.com/coffebar/neovim-project) ⭐ 280 | 🐛 3 | 🌐 Lua | 📅 2026-01-08 - Declarative project management, automatic saving of sessions, uses Telescope.
* [niuiic/multiple-session.nvim](https://github.com/niuiic/multiple-session.nvim) ⭐ 9 | 🐛 0 | 🌐 Lua | 📅 2024-05-25 - Provides multi-session management capabilities.
* [Akmadan23/local-session.nvim](https://github.com/Akmadan23/local-session.nvim) ⭐ 5 | 🐛 0 | 🌐 Lua | 📅 2026-01-26 - A fast, minimal and implicit current-working-directory-based session manager with easy to configure session files in Lua.
* [njayman/season.nvim](https://github.com/njayman/season.nvim) ⭐ 3 | 🐛 0 | 🌐 Lua | 📅 2025-11-24 - A lightweight plugin to manage session based on current working directory.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Remote Development

* [chipsenkbeil/distant.nvim](https://github.com/chipsenkbeil/distant.nvim) ⭐ 1,356 | 🐛 26 | 🌐 Lua | 📅 2024-10-17 - Edit files, run programs, and work with LSP on a remote machine from the comfort of your local environment.
* [jamestthompson3/nvim-remote-containers](https://github.com/jamestthompson3/nvim-remote-containers) ⭐ 928 | 🐛 11 | 🌐 Lua | 📅 2023-12-22 - Develop inside Docker containers, just like VSCode.
* [esensar/nvim-dev-container](https://github.com/esensar/nvim-dev-container) ⭐ 704 | 🐛 10 | 🌐 Lua | 📅 2026-02-13 - Provide functionality similar to VSCode's [remote container development](https://code.visualstudio.com/docs/remote/containers) plugin, with other functionalities that enable development in Docker containers.
* [nosduco/remote-sshfs.nvim](https://github.com/nosduco/remote-sshfs.nvim) ⭐ 381 | 🐛 17 | 🌐 Lua | 📅 2025-09-30 - Explore, edit, and develop on a remote machine via SSHFS.
* [miversen33/netman.nvim](https://github.com/miversen33/netman.nvim) ⭐ 369 | 🐛 50 | 🌐 Lua | 📅 2025-09-13 - Lua powered Network Resource Manager.
* [azratul/live-share.nvim](https://github.com/azratul/live-share.nvim) ⭐ 237 | 🐛 0 | 🌐 Lua | 📅 2025-05-03 - Provides remote collaboration capabilities from anywhere, making it ideal for pair-programming scenarios.
* [uhs-robert/sshfs.nvim](https://github.com/uhs-robert/sshfs.nvim) ⭐ 152 | 🐛 5 | 🌐 Lua | 📅 2026-01-21 - Mount remote systems via SSHFS with smart picker auto-detect (Telescope/Oil/Snacks/Neo-tree/fzf-lua/Yazi/Ranger etc.).
* [inhesrom/remote-ssh.nvim](https://github.com/inhesrom/remote-ssh.nvim) ⭐ 95 | 🐛 2 | 🌐 Lua | 📅 2026-02-09 - Duplicates the basic ground level functionality of VSCode's Remote-SSH plugin, with a focus on a local editing experience to avoid remote "lag". Browse remote files, edit "remote buffers" with a full local editing experience (LSP, Tree-sitter, Telescope integration, and a file watcher).
* [niuiic/remote.nvim](https://github.com/niuiic/remote.nvim) ⭐ 45 | 🐛 0 | 🌐 Lua | 📅 2024-05-11 - Edit remote files with local configuration.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Live Preview

* [kiyoon/jupynium.nvim](https://github.com/kiyoon/jupynium.nvim) ⭐ 743 | 🐛 10 | 🌐 Python | 📅 2025-12-26 - Selenium-automated Jupyter Notebook that is synchronised with Neovim in real-time.
* [gruvw/strudel.nvim](https://github.com/gruvw/strudel.nvim) ⭐ 393 | 🐛 4 | 🌐 JavaScript | 📅 2025-12-06 - Live coding controller for [strudel](https://strudel.cc).
* [brianhuster/live-preview.nvim](https://github.com/brianhuster/live-preview.nvim) ⭐ 340 | 🐛 23 | 🌐 Lua | 📅 2026-02-15 - Live preview HTML, Markdown and Asciidoc in the browser.
* [SUSTech-data/neopyter](https://github.com/SUSTech-data/neopyter) ⭐ 158 | 🐛 3 | 🌐 Lua | 📅 2026-01-12 - Edit in Neovim and preview/run in Jupyter Lab.
* [hat0uma/prelive.nvim](https://github.com/hat0uma/prelive.nvim) ⭐ 23 | 🐛 0 | 🌐 Lua | 📅 2025-10-05 - A simple luv-based development server with live reloading.
* [hat0uma/doxygen-previewer.nvim](https://github.com/hat0uma/doxygen-previewer.nvim) ⭐ 8 | 🐛 1 | 🌐 Lua | 📅 2025-09-17 - Live previewing of Doxygen documentation.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Split and Window

* [nvim-mini/mini.nvim#mini.bufremove](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-bufremove.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` for buffer removing (unshow, delete, wipeout) while saving window layout.
* [mrjones2014/smart-splits.nvim](https://github.com/mrjones2014/smart-splits.nvim) ⭐ 1,552 | 🐛 13 | 🌐 Lua | 📅 2026-02-13 - Smart, seamless, directional navigation and resizing of splits.
* [nvim-focus/focus.nvim](https://github.com/nvim-focus/focus.nvim) ⭐ 802 | 🐛 23 | 🌐 Lua | 📅 2026-02-08 - Auto-Focusing and Auto-Resizing Splits/Windows written in Lua! Vim splits on steroids.
* [nvim-zh/colorful-winsep.nvim](https://github.com/nvim-zh/colorful-winsep.nvim) ⭐ 650 | 🐛 1 | 🌐 Lua | 📅 2026-01-19 - A configurable color split line.
* [anuvyklack/windows.nvim](https://github.com/anuvyklack/windows.nvim) ⭐ 636 | 🐛 22 | 🌐 Lua | 📅 2023-07-08 - Automatically expand width of the current window. Maximizes and restore it. And all this with nice animations!
* [sindrets/winshift.nvim](https://github.com/sindrets/winshift.nvim) ⭐ 526 | 🐛 9 | 🌐 Lua | 📅 2024-05-20 - Rearrange your windows with ease.
* [altermo/nwm](https://github.com/altermo/nwm) ⭐ 337 | 🐛 1 | 🌐 Lua | 📅 2024-06-19 - X11 window manager.
* [yorickpeterse/nvim-window](https://github.com/yorickpeterse/nvim-window) ⭐ 172 | 🐛 0 | 🌐 Lua | 📅 2026-01-20 - Easily jump between windows.
* [nyngwang/NeoNoName.lua](https://github.com/nyngwang/NeoNoName.lua) ⭐ 29 | 🐛 2 | 🌐 Lua | 📅 2023-06-01 - Layout preserving buffer deletion.
* [jyscao/ventana.nvim](https://github.com/jyscao/ventana.nvim) ⭐ 21 | 🐛 0 | 🌐 Lua | 📅 2025-11-23 - Convenient flips and shifts for your windows layout.
* [MisanthropicBit/winmove.nvim](https://github.com/MisanthropicBit/winmove.nvim) ⭐ 16 | 🐛 2 | 🌐 Lua | 📅 2026-01-22 - Easily move, swap, and resize windows.
* [wsdjeg/tabman.nvim](https://github.com/wsdjeg/tabman.nvim) ⭐ 14 | 🐛 1 | 🌐 Lua | 📅 2026-02-01 - Navigate between tabs and the windows they contain.
* [aronjohanns/smooth-resize.nvim](https://github.com/aronjohanns/smooth-resize.nvim) ⭐ 12 | 🐛 1 | 🌐 Lua | 📅 2026-01-23 - Smooth, continuous window resizing with the default window resizing mappings.
* [ycdzj/win-mover.nvim](https://github.com/ycdzj/win-mover.nvim) ⭐ 11 | 🐛 0 | 🌐 Lua | 📅 2025-01-10 - Window mover that avoids moving side windows.
* [mkajsjo/windowcolumns.nvim](https://github.com/mkajsjo/windowcolumns.nvim) ⭐ 8 | 🐛 0 | 🌐 Lua | 📅 2025-06-07 - Column-first window management.
* [\~henriquehbr/ataraxis.lua](https://sr.ht/~henriquehbr/ataraxis.lua) - A zen mode for improving code readability.

### Tmux

* [aserowy/tmux.nvim](https://github.com/aserowy/tmux.nvim) ⭐ 773 | 🐛 16 | 🌐 Lua | 📅 2025-03-19 - Tmux integration features pane movement and resizing.
* [hkupty/nvimux](https://github.com/hkupty/nvimux) ⭐ 451 | 🐛 4 | 🌐 Lua | 📅 2022-05-19 - Use Neovim as a tmux replacement.
* [numToStr/Navigator.nvim](https://github.com/numToStr/Navigator.nvim) ⭐ 431 | 🐛 14 | 🌐 Lua | 📅 2024-07-07 - Smoothly navigate between Neovim splits and tmux panes.
* [declancm/windex.nvim](https://github.com/declancm/windex.nvim) ⭐ 61 | 🐛 1 | 🌐 Lua | 📅 2022-07-12 - Collection of window functions which includes moving between, closing and maximizing Neovim splits and tmux panes.
* [EvWilson/slimux.nvim](https://github.com/EvWilson/slimux.nvim) ⭐ 31 | 🐛 0 | 🌐 Lua | 📅 2025-11-13 - Send content from the current buffer to a configurable tmux pane.
* [danielpieper/telescope-tmuxinator.nvim](https://github.com/danielpieper/telescope-tmuxinator.nvim) ⭐ 25 | 🐛 0 | 🌐 Lua | 📅 2023-12-17 - Integration for tmuxinator with telescope.nvim.
* [karshPrime/tmux-compile.nvim](https://github.com/karshPrime/tmux-compile.nvim) ⭐ 24 | 🐛 0 | 🌐 Lua | 📅 2025-06-03 - Set up same key, like F5, to run any compile/run command per language, like `make` for C and `cargo build` for Rust, and have the project run or compile in a new tmux pane or window.
* [kiyoon/tmux-send.nvim](https://github.com/kiyoon/tmux-send.nvim) ⭐ 18 | 🐛 0 | 🌐 Lua | 📅 2026-01-24 - Copy and paste buffer content or file path in either `nvim-tree`, `neo-tree` or `oil.nvim` to another tmux pane.
* [juselara1/tmutils.nvim](https://github.com/juselara1/tmutils.nvim) ⭐ 16 | 🐛 0 | 🌐 Lua | 📅 2024-12-21 - Tmux utilities that enable sending lines, capturing content, creating terminals, and managing REPLs.
* [karshPrime/only-tmux.nvim](https://github.com/karshPrime/only-tmux.nvim) ⭐ 10 | 🐛 0 | 🌐 Lua | 📅 2024-06-18 - Expand the functionality of `:only` with tmux panes in the same window, with either moving them to a new window or closing them.
* [salorak/libtmux.nvim](https://github.com/salorak/libtmux.nvim) ⭐ 6 | 🐛 0 | 🌐 Lua | 📅 2026-02-15 - Thin wrapper for using the `tmux` API.
* [jkeresman01/tmux-switch.nvim](https://github.com/jkeresman01/tmux-switch.nvim) ⭐ 5 | 🐛 1 | 🌐 Lua | 📅 2025-10-09 - Provides fuzzy session switching for Tmux.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Game

* [Eandrju/cellular-automaton.nvim](https://github.com/Eandrju/cellular-automaton.nvim) ⭐ 2,076 | 🐛 12 | 🌐 Lua | 📅 2025-01-31 - It lets you execute aesthetically pleasing, cellular automaton animations based on the content of the current buffer.
* [alec-gibson/nvim-tetris](https://github.com/alec-gibson/nvim-tetris) ⭐ 211 | 🐛 7 | 🌐 Lua | 📅 2024-01-17 - Bringing Emacs' greatest feature to Neovim - Tetris.
* [seandewar/actually-doom.nvim](https://github.com/seandewar/actually-doom.nvim) ⭐ 128 | 🐛 3 | 🌐 C | 📅 2025-08-26 - Editing text is boring; play DOOM instead!.
* [seandewar/nvimesweeper](https://github.com/seandewar/nvimesweeper) ⭐ 108 | 🐛 1 | 🌐 Lua | 📅 2024-06-29 - Play Minesweeper in your favourite text editor.
* [rktjmp/playtime.nvim](https://github.com/rktjmp/playtime.nvim) ⭐ 87 | 🐛 2 | 🌐 Fennel | 📅 2025-09-23 - A collection of games such as Freecell, Shenzhen Solitaire and The Emissary.
* [jim-fx/sudoku.nvim](https://github.com/jim-fx/sudoku.nvim) ⭐ 79 | 🐛 1 | 🌐 Lua | 📅 2023-12-11 - Classic sudoku puzzle.
* [seandewar/killersheep.nvim](https://github.com/seandewar/killersheep.nvim) ⭐ 75 | 🐛 1 | 🌐 Lua | 📅 2025-03-20 - A port of killersheep.
* [alanfortlink/blackjack.nvim](https://github.com/alanfortlink/blackjack.nvim) ⭐ 69 | 🐛 0 | 🌐 Lua | 📅 2024-07-28 - Classic Black Jack game.
* [piersolenski/skifree.nvim](https://github.com/piersolenski/skifree.nvim) ⭐ 18 | 🐛 0 | 🌐 Lua | 📅 2025-11-24 - Play the Windows 3.1 SkiFree game.
* [csessh/aoc.vim](https://github.com/csessh/aoc.nvim) ⭐ 8 | 🐛 1 | 🌐 Lua | 📅 2025-12-01 - Simple little elf who fetches Advent of Code puzzle input for you.

### Competitive Programming

* [kawre/leetcode.nvim](https://github.com/kawre/leetcode.nvim) ⭐ 1,973 | 🐛 56 | 🌐 Lua | 📅 2025-09-21 - Solve Leetcode problems.
* [xeluxee/competitest.nvim](https://github.com/xeluxee/competitest.nvim) ⭐ 569 | 🐛 16 | 🌐 Lua | 📅 2025-05-13 - A plugin to automate testcases management and checking for Competitive Programming contests.
* [p00f/cphelper.nvim](https://github.com/p00f/cphelper.nvim) ⭐ 149 | 🐛 3 | 🌐 Lua | 📅 2026-01-14 - Helper for competitive programming written in Lua.
* [2KAbhishek/exercism.nvim](https://github.com/2KAbhishek/exercism.nvim) ⭐ 37 | 🐛 0 | 🌐 Lua | 📅 2025-08-04 - Browse and solve Exercism problems.
* [barrettruth/cp.nvim](https://github.com/barrettruth/cp.nvim) ⭐ 7 | 🐛 2 | 🌐 Lua | 📅 2026-02-18 - Competitive programming workflow for popular contest platforms (CodeForces, CSES, etc.) Includes automatic test scraping, I/O view, and diff panel.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Workflow

* [m4xshen/hardtime.nvim](https://github.com/m4xshen/hardtime.nvim) ⭐ 3,696 | 🐛 13 | 🌐 Lua | 📅 2025-09-13 - Helping you establish good command workflow and habit.
* [saxon1964/neovim-tips](https://github.com/saxon1964/neovim-tips) ⭐ 443 | 🐛 1 | 🌐 Lua | 📅 2026-02-06 - Provides hundreds of built-in tips, tricks and shortcuts, with a custom picker interface and the ability to add your own tips.
* [ecthelionvi/NeoComposer.nvim](https://github.com/ecthelionvi/NeoComposer.nvim) ⚠️ Archived - Simplify macro management, enhance productivity, and create harmonious workflows.
* [letieu/jira.nvim](https://github.com/letieu/jira.nvim) ⭐ 218 | 🐛 5 | 🌐 Lua | 📅 2026-01-16 - Manage Jira tasks with a beautiful UI.
* [yagiziskirik/AirSupport.nvim](https://github.com/yagiziskirik/AirSupport.nvim) ⭐ 10 | 🐛 0 | 🌐 Lua | 📅 2023-05-25 - Searchable reminder window for your custom shortcuts and commands.

### Stats Tracking

* [gisketch/triforce.nvim](https://github.com/gisketch/triforce.nvim) ⭐ 267 | 🐛 3 | 🌐 Lua | 📅 2026-02-11 - Gamified stat tracker with XP, levels, achievements, and activity heatmaps for your coding sessions with lualine integration.
* [gaborvecsei/usage-tracker.nvim](https://github.com/gaborvecsei/usage-tracker.nvim) ⭐ 135 | 🐛 3 | 🌐 Lua | 📅 2024-03-10 - Track your Neovim usage and visualize statistics easily.
* [ptdewey/pendulum-nvim](https://github.com/ptdewey/pendulum-nvim) ⭐ 108 | 🐛 1 | 🌐 Go | 📅 2026-01-31 - Track time spent coding and glean insights through on-demand time reports.
* [QuentinGruber/pomodoro.nvim](https://github.com/QuentinGruber/pomodoro.nvim) ⭐ 46 | 🐛 1 | 🌐 Lua | 📅 2025-11-24 - Use the Pomodoro Technique with built-in session tracking and break reminders.
* [SunnyTamang/pendulum.nvim](https://github.com/SunnyTamang/pendulum.nvim) ⭐ 14 | 🐛 1 | 🌐 Lua | 📅 2024-08-22 - Simple timer for creating time based productive sessions for coders, competitive programmers, developers etc.
* [ravsii/timers.nvim](https://github.com/ravsii/timers.nvim) ⭐ 14 | 🐛 1 | 🌐 Lua | 📅 2025-10-13 - Timer manager, a clean Lua API, supporting multiple timers, persistence, UI, and plugin integrations.
* [Rtarun3606k/takatime](https://github.com/Rtarun3606k/takatime) ⭐ 14 | 🐛 2 | 🌐 Go | 📅 2026-02-18 - Privacy-first WakaTime alternative using Go and MongoDB.

### Automation

* [jghauser/mkdir.nvim](https://github.com/jghauser/mkdir.nvim) ⭐ 233 | 🐛 1 | 🌐 Lua | 📅 2022-07-23 - Automatically create missing directories when saving files.
* [mateuszwieloch/automkdir.nvim](https://github.com/mateuszwieloch/automkdir.nvim) ⭐ 30 | 🐛 0 | 🌐 Lua | 📅 2025-03-31 - Automatically create non-existent parent directories when writing a file.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Database

* [kndndrj/nvim-dbee](https://github.com/kndndrj/nvim-dbee) ⭐ 1,219 | 🐛 75 | 🌐 Go | 📅 2025-07-25 - Interactive database client.
* [zongben/dbout.nvim](https://github.com/zongben/dbout.nvim) ⭐ 26 | 🐛 0 | 🌐 Lua | 📅 2025-10-22 - Manage database connections and run SQL queries directly with JSON results.
* [zerochae/dbab.nvim](https://github.com/zerochae/dbab.nvim) ⭐ 23 | 🐛 3 | 🌐 Lua | 📅 2026-02-09 - Lightweight database client with a modern UI and async execution.
* [tashikomaaa/neomongo.nvim](https://github.com/tashikomaaa/neomongo.nvim) ⭐ 7 | 🐛 0 | 🌐 Lua | 📅 2025-11-03 - Explore, query, and edit MongoDB collections directly through a Telescope-powered dashboard.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Preconfigured Configuration

* [nvim-lua/kickstart.nvim](https://github.com/nvim-lua/kickstart.nvim) ⭐ 29,470 | 🐛 60 | 🌐 Lua | 📅 2026-01-27 - A launch point for your personal Neovim configuration.
* [siduck76/NvChad](https://github.com/siduck76/NvChad) ⭐ 27,877 | 🐛 1 | 🌐 Lua | 📅 2026-02-07 - An attempt to make Neovim's CLI as functional as an IDE while retaining beauty with less bloat.
* [LazyVim/LazyVim](https://github.com/LazyVim/LazyVim) ⭐ 25,090 | 🐛 59 | 🌐 Lua | 📅 2025-11-11 - Full-fledged IDE powered by **lazy.nvim** to make it easy to customize and extend your config.
* [LunarVim/LunarVim](https://github.com/LunarVim/LunarVim) ⭐ 19,224 | 🐛 33 | 🌐 Lua | 📅 2025-06-05 - This project aims to help one transition away from VSCode, and into a superior text editing experience.
* [AstroNvim/AstroNvim](https://github.com/AstroNvim/AstroNvim) ⭐ 14,116 | 🐛 1 | 🌐 Lua | 📅 2026-02-17 - An aesthetic and feature-rich config that is extensible and easy to use with a great set of plugins.
* [ayamir/nvimdots](https://github.com/ayamir/nvimdots) ⭐ 3,372 | 🐛 13 | 🌐 Lua | 📅 2026-02-15 - A well-configured and structured configuration with NixOS support.
* [shaunsingh/nyoom.nvim](https://github.com/shaunsingh/nyoom.nvim) ⭐ 1,571 | 🐛 30 | 🌐 Fennel | 📅 2023-11-05 - Blazing fast, configurable, minimal and "lispy" config written in Fennel.
* [CosmicNvim/CosmicNvim](https://github.com/CosmicNvim/CosmicNvim) ⭐ 1,146 | 🐛 2 | 🌐 Lua | 📅 2026-02-17 - CosmicNvim is a lightweight and opinionated config for web development, specifically designed to provide a COSMIC programming experience!
* [dam9000/kickstart-modular.nvim](https://github.com/dam9000/kickstart-modular.nvim) ⭐ 945 | 🐛 4 | 🌐 Lua | 📅 2025-06-14 - This is a fork of nvim-lua/kickstart.nvim that moves from a single file to a multi file configuration.
* [artart222/CodeArt](https://github.com/artart222/CodeArt) ⭐ 903 | 🐛 9 | 🌐 Lua | 📅 2024-12-06 - A fast general-purpose IDE written entirely in Lua with an installer for Linux/Windows/macOS and built-in `:CodeArtUpdate` command for updating it.
* [ldelossa/nvim-ide](https://github.com/ldelossa/nvim-ide) ⭐ 869 | 🐛 14 | 🌐 Lua | 📅 2025-07-27 - A full featured IDE layer heavily inspired by VSCode.
* [NormalNvim/NormalNvim](https://github.com/NormalNvim/NormalNvim) ⭐ 696 | 🐛 4 | 🌐 Lua | 📅 2025-12-01 - Configuration focused on stability for your daily work.
* [crivotz/nv-ide](https://github.com/crivotz/nv-ide) ⭐ 644 | 🐛 1 | 🌐 Lua | 📅 2026-02-05 - Custom configuration oriented for Full-Stack developers (Rails, Ruby, PHP, HTML, CSS, SCSS, JavaScript).
* [hackorum/VapourNvim](https://github.com/hackorum/VapourNvim) ⭐ 561 | 🐛 17 | 🌐 Lua | 📅 2023-03-31 - Configuration for the ultimate Vim IDE-like experience.
* [doctorfree/nvim-lazyman](https://github.com/doctorfree/nvim-lazyman) ⭐ 420 | 🐛 9 | 🌐 HTML | 📅 2025-11-21 - Configuration manager and a modular configuration on its own. Supports over 40 preconfigured configurations.
* [mrcjkb/kickstart-nix.nvim](https://github.com/mrcjkb/kickstart-nix.nvim) ⭐ 392 | 🐛 2 | 🌐 Lua | 📅 2026-01-26 - A simple [Nix flake](https://wiki.nixos.org/wiki/Flakes) template repo for Neovim derivations, with the goal of simplifying the migration from existing Neovim configurations.
* [pgosar/CyberNvim](https://github.com/pgosar/CyberNvim) ⭐ 375 | 🐛 2 | 🌐 Lua | 📅 2025-02-20 - The world's simplest and most extensible Neovim distribution.
* [nvim-mini/MiniMax](https://github.com/nvim-mini/MiniMax) ⭐ 319 | 🐛 2 | 🌐 Lua | 📅 2026-02-17 - A collection of self-contained and extensively commented configurations which mostly use MINI tools.
* [Shaobin-Jiang/IceNvim](https://github.com/Shaobin-Jiang/IceNvim) ⭐ 295 | 🐛 3 | 🌐 Lua | 📅 2026-01-23 - A beautiful, powerful and customizable config that is blazingly fast.
* [Abstract-IDE/Abstract](https://github.com/Abstract-IDE/Abstract) ⭐ 206 | 🐛 2 | 🌐 Lua | 📅 2026-02-17 - Configuration to achieve the power of Modern IDE.
* [shaeinst/roshnivim](https://github.com/shaeinst/roshnivim) ⭐ 206 | 🐛 2 | 🌐 Lua | 📅 2026-02-17 - A predefined config to save you thousands of hours to setup Neovim as an IDE.
* [adoyle-h/one.nvim](https://github.com/adoyle-h/one.nvim) ⭐ 177 | 🐛 0 | 🌐 Lua | 📅 2025-11-02 - All-in-one config framework in Lua.
* [chrisgrieser/nvim-kickstart-python](https://github.com/chrisgrieser/nvim-kickstart-python) ⚠️ Archived - A launch point for your Neovim configuration (for Python).
* [cstsunfu/.sea.nvim](https://github.com/cstsunfu/.sea.nvim) ⭐ 148 | 🐛 0 | 🌐 Lua | 📅 2025-08-03 - A modular configuration with a beautiful UI and some useful features such as a pomodoro clock and window numbers.
* [linrongbin16/lin.nvim](https://github.com/linrongbin16/lin.nvim) ⭐ 90 | 🐛 0 | 🌐 Lua | 📅 2026-02-16 - A highly configured Neovim distribution integrated with tons of utilities for development, inspired by `spf13-vim`.
* [crispybaccoon/chaivim](https://github.com/crispybaccoon/chaivim) ⭐ 73 | 🐛 0 | 🌐 Lua | 📅 2024-11-21 - Easily configurable distro with solid defaults and a cozy editor experience.
* [imbacraft/dusk.nvim](https://github.com/imbacraft/dusk.nvim) ⭐ 55 | 🐛 0 | 🌐 Lua | 📅 2024-06-02 - A lightweight, aesthetically minimal config, written in Lua, able to provide for web and Java development.
* [sontungexpt/stinvim](https://github.com/sontungexpt/stinvim) ⭐ 49 | 🐛 1 | 🌐 Lua | 📅 2025-11-22 - Configuration for Full-Stack developers.
* [drybalka/clean.nvim](https://github.com/drybalka/clean.nvim) ⭐ 39 | 🐛 0 | 🌐 Lua | 📅 2024-01-29 - Cleaning up the default key mappings and plugins and leaving only the bare essentials to build upon.
* [legobeat/l7-devenv](https://github.com/legobeat/l7-devenv) ⭐ 25 | 🐛 34 | 🌐 JavaScript | 📅 2025-12-01 - Security-focused IDE with a hackable (in the right way) framework based on Neovim and shell.
* [StratOS-Linux/StratVIM](https://github.com/StratOS-Linux/StratVIM) ⭐ 13 | 🐛 1 | 🌐 Lua | 📅 2026-01-04 - A full-fledged Neovim distribution included by default in [StratOS-Linux](https://github.com/StratOS-Linux).
* [cunderw/nvim](https://github.com/cunderw/nvim) ⭐ 11 | 🐛 0 | 🌐 Lua | 📅 2024-04-02 - A custom, IDE-like configuration for JS/TS, Go, and Java development.
* [jrychn/moduleVim](https://github.com/jrychn/ModuleVim) ⭐ 8 | 🐛 0 | 🌐 Lua | 📅 2025-10-31 - A very easy to use for backend and frontend, install LSP automatically.
* [abdellatif-temsamani/adev.nvim](https://github.com/abdellatif-temsamani/adev.nvim) ⭐ 4 | 🐛 3 | 🌐 Lua | 📅 2026-02-16 - The over-engineered Neovim distribution for developers who want everything.
* [TheItcor/MoaiVim](https://github.com/TheItcor/MoaiVim) ⭐ 4 | 🐛 0 | 🌐 Lua | 📅 2025-11-23 - A minimalist config that emulates a lightweight IDE.
* [SpaceVim/SpaceVim](https://spacevim.org) - A community-driven modular Vim/Neovim distribution, inspired by `spacemacs`.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## External

These tools are used externally to Neovim to enhance the experience.

### Version Manager

* [MordechaiHadad/bob](https://github.com/MordechaiHadad/bob) ⭐ 2,007 | 🐛 28 | 🌐 Rust | 📅 2026-02-14 - A cross-platform, easy to use Neovim version manager.
* [NTBBloodbath/nvenv](https://github.com/NTBBloodbath/nvenv) ⭐ 61 | 🐛 2 | 🌐 V | 📅 2025-05-14 - A lightweight and blazingly fast Neovim version manager.
* [y3owk1n/nvs](https://github.com/y3owk1n/nvs) ⭐ 28 | 🐛 0 | 🌐 Go | 📅 2026-02-17 - Another Neovim version manager with config switcher.

### Plugin Template

* [ellisonleao/nvim-plugin-template](https://github.com/ellisonleao/nvim-plugin-template) ⭐ 449 | 🐛 2 | 🌐 Lua | 📅 2025-10-08 - Another Neovim plugin template, using GitHub's template feature.
* [m00qek/plugin-template.nvim](https://github.com/m00qek/plugin-template.nvim) ⭐ 135 | 🐛 2 | 🌐 Lua | 📅 2023-12-17 - A plugin template that setups test infrastructure and GitHub Actions.
* [gennaro-tedesco/boilit](https://github.com/gennaro-tedesco/boilit) ⭐ 84 | 🐛 0 | 🌐 Go | 📅 2022-11-22 - Create boilerplate structure plugins.
* [chrisgrieser/nvim-pseudometa-plugin-template](https://github.com/chrisgrieser/nvim-pseudometa-plugin-template) ⭐ 39 | 🐛 0 | 🌐 Shell | 📅 2026-02-11 - Template for new Neovim plugins.
* [2KAbhishek/template.nvim](https://github.com/2KAbhishek/template.nvim) ⭐ 19 | 🐛 0 | 🌐 Lua | 📅 2025-08-05 - Opinionated template for starting plugin dev quickly.
* [jkeresman01/spring-initializr.nvim](https://github.com/jkeresman01/spring-initializr.nvim) ⭐ 16 | 🐛 109 | 🌐 Lua | 📅 2026-02-07 - Scaffold Spring Boot projects with a Telescope-powered UI.
* [DrKJeff16/nvim-plugin-boilerplate](https://github.com/DrKJeff16/nvim-plugin-boilerplate) ⭐ 12 | 🐛 0 | 🌐 Shell | 📅 2026-02-17 - A documented template for new plugins generated by a script. Includes tests, CI utilities, etc.

### OS-specific

* [m15a/flake-awesome-neovim-plugins](https://github.com/m15a/flake-awesome-neovim-plugins) ⭐ 62 | 🐛 0 | 🌐 Nix | 📅 2026-02-17 - Nix flake that provides a collection of `awesome-neovim` plugins as Nix packages.
* [chrisgrieser/alfred-neovim-utilities](https://github.com/chrisgrieser/alfred-neovim-utilities) ⭐ 43 | 🐛 0 | 🌐 JavaScript | 📅 2026-02-15 - Search Neovim plugins and online `:help` via Alfred (macOS).
* [massix/termux.nvim](https://github.com/massix/termux.nvim) ⭐ 25 | 🐛 1 | 🌐 Lua | 📅 2024-02-22 - Interact with Termux APIs, useful to gather various information about your Android phone to display in the statusline (e.g. battery level).
* [iamironz/android-nvim-plugin](https://github.com/iamironz/android-nvim-plugin) ⭐ 13 | 🐛 0 | 🌐 Lua | 📅 2026-02-10 - Android build, deploy, and logcat commands with Gradle integration.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Wishlist

Have a problem a plugin can solve? Add it to the [nvim-lua wishlist](https://github.com/nvim-lua/wishlist) ⭐ 249 | 🐛 39 | 📅 2020-09-29.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## UI

* [nvim-mini/mini.nvim#mini.notify](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-notify.md) ⭐ 8,745 | 🐛 35 | 🌐 Lua | 📅 2026-02-17 - Module of `mini.nvim` to show one or more highlighted notifications in a single window. Provides maker of `vim.notify()` implementation and sets up automated LSP progress updates.
* [folke/noice.nvim](https://github.com/folke/noice.nvim) ⭐ 5,608 | 🐛 30 | 🌐 Lua | 📅 2025-11-03 - Highly experimental plugin that completely replaces the UI for messages, cmdline and the popupmenu.
* [rcarriga/nvim-notify](https://github.com/rcarriga/nvim-notify) ⭐ 3,520 | 🐛 73 | 🌐 Lua | 📅 2025-09-06 - A fancy, configurable, notification manager.
* [mcauley-penney/visual-whitespace.nvim](https://github.com/mcauley-penney/visual-whitespace.nvim) ⭐ 437 | 🐛 0 | 🌐 Lua | 📅 2026-02-07 - See whitespace characters in Visual selections, like VSCode.
* [ghillb/cybu.nvim](https://github.com/ghillb/cybu.nvim) ⭐ 325 | 🐛 0 | 🌐 Lua | 📅 2026-01-23 - Displays a notification window with context when cycling buffers.
* [matbme/JABS.nvim](https://github.com/matbme/JABS.nvim) ⭐ 282 | 🐛 12 | 🌐 Lua | 📅 2023-05-28 - Pretty and minimal buffer switcher window.
* [LukasPietzschmann/telescope-tabs](https://github.com/LukasPietzschmann/telescope-tabs) ⭐ 281 | 🐛 1 | 🌐 Lua | 📅 2025-09-01 - Quickly navigate between tabs using telescope.
* [toppair/reach.nvim](https://github.com/toppair/reach.nvim) ⭐ 244 | 🐛 5 | 🌐 Lua | 📅 2022-11-21 - Buffer, mark, tabpage switcher.
* [sitiom/nvim-numbertoggle](https://github.com/sitiom/nvim-numbertoggle) ⭐ 215 | 🐛 2 | 🌐 Lua | 📅 2025-11-21 - Automatically toggle between relative and absolute line numbers.
* [CosmicNvim/cosmic-ui](https://github.com/CosmicNvim/cosmic-ui) ⭐ 171 | 🐛 1 | 🌐 Lua | 📅 2025-01-27 - Cosmic-UI is a simple wrapper around specific Vim functionality.
* [OXY2DEV/ui.nvim](https://github.com/OXY2DEV/ui.nvim) ⭐ 154 | 🐛 3 | 🌐 Lua | 📅 2026-02-14 - A blueprint/template/guide for customizing the UI.
* [jrop/tuis.nvim](https://github.com/jrop/tuis.nvim) ⭐ 129 | 🐛 0 | 🌐 Lua | 📅 2026-01-15 - A collection of interactive TUIs which provides rich, interactive UIs to various CLIs.
* [xieyonn/spinner.nvim](https://github.com/xieyonn/spinner.nvim) ⭐ 83 | 🐛 1 | 🌐 Lua | 📅 2026-02-14 - Extensible spinner framework for animated spinners in statusline, tabline, winbar, buffer, cmdline, or next to the cursor.
* [ariel-frischer/bmessages.nvim](https://github.com/ariel-frischer/bmessages.nvim) ⭐ 59 | 🐛 3 | 🌐 Lua | 📅 2025-01-10 - Replace the default `:messages` window with a configurable, auto-updating buffer.
* [wsdjeg/calendar.nvim](https://github.com/wsdjeg/calendar.nvim) ⭐ 40 | 🐛 1 | 🌐 Lua | 📅 2026-01-30 - A simple floating calendar with extensions support.
* [nkakouros-original/numbers.nvim](https://github.com/nkakouros-original/numbers.nvim) ⭐ 38 | 🐛 0 | 🌐 Lua | 📅 2025-02-11 - Toggle relativenumber whenever it makes sense.
* [cpea2506/relative-toggle.nvim](https://github.com/cpea2506/relative-toggle.nvim) ⭐ 37 | 🐛 1 | 🌐 Lua | 📅 2025-07-13 - Toggles smoothly between number and relative numbers, supporting various number combinations, highly customizable.
* [markgandolfo/lightswitch.nvim](https://github.com/markgandolfo/lightswitch.nvim) ⭐ 22 | 🐛 1 | 🌐 Lua | 📅 2025-06-29 - Toggle various options using the `nui.nvim` library.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Starter Templates

* [tokiory/neovim-boilerplate](https://github.com/tokiory/neovim-boilerplate) ⭐ 121 | 🐛 0 | 🌐 Lua | 📅 2025-06-23 - Starter boilerplate for making new configurations.
* [frans-johansson/lazy-nvim-starter](https://github.com/frans-johansson/lazy-nvim-starter) ⭐ 96 | 🐛 1 | 🌐 Lua | 📅 2023-10-26 - Starter boilerplate with lazy plugin manager.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Vim

* [Vimawesome](https://vimawesome.com/) - Showcases various plugins for Vim and has a [Neovim tag](https://vimawesome.com/?q=tag:neovim) for other Neovim-related plugins.
* [akrawchyk/awesome-vim#tools](https://github.com/akrawchyk/awesome-vim#tools) ⭐ 2,114 | 🐛 6 | 📅 2025-06-06 - A short list of Vim plugins and helpful guides.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Resource

* [Neovimcraft](https://neovimcraft.com) - A site dedicated to searching specific plugins and guides for building plugins in Lua.
* [Dotfyle](https://dotfyle.com) - A site for sharing and discovering Neovim configs and plugins.
* [NeoLand](https://neoland.dev) - A beautifully crafted website for Neovim resources.
* [Weyaaron/nvim-training](https://github.com/Weyaaron/nvim-training) ⭐ 119 | 🐛 4 | 🌐 Lua | 📅 2026-01-18 - A beginner-friendly tool for training your 'muscle memory' using small, repeatable tasks.
* [Nvim.app](https://nvim.app) - A modern search interface for Neovim plugins with fuzzy search, filtering, and self-service updates for plugin authors.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->
