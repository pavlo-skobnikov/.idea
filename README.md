# IdeaVim Configuration README

<!--toc:start-->

- [IdeaVim Configuration README](#ideavim-configuration-readme)
  - [Overview](#overview)
  - [Configuration Details](#configuration-details)
    - [General Options](#general-options)
    - [Plugins & Settings](#plugins-settings)
      - [Which-Key Extension](#which-key-extension)
      - [NERDTree Support](#nerdtree-support)
      - [Vim-Surround Emulation](#vim-surround-emulation)
      - [Argument Text Object](#argument-text-object)
  - [Mentions](#mentions)

<!--toc:end-->

## Overview

This README documents the configuration settings for IdeaVim, a Vim emulation plugin for JetBrains
IDEs. The configuration enhances the traditional Vim experience with IDE-specific integrations
and plugins.

## Configuration Details

### General Options

- **Handler Settings**: Vim is the default handler for Vim shortcuts, with some exceptions like
  `<C-y>` handled by IntelliJ IDEA.
- **Line Joining Behavior**: Utilizes IntelliJ's line joining method.
- **Leader Key**: Spacebar (` `) set as the leader key.
- **Mode Display**: Current Vim mode is displayed.
- **Clipboard Integration**: Clipboard register `*` is used for all yank, delete, change, and put
  operations.
- **Incremental Search**: Searches are performed as characters are entered.
- **Search Highlighting**: All search results are highlighted.
- **Case Sensitivity in Search**:
  - `ignorecase`: Search is case-insensitive.
  - `smartcase`: Case sensitivity is enabled if the search pattern contains upper-case letters.
- **Relative Line Numbers**: Line numbers are displayed relative to the current line.

### Plugins & Settings

#### Which-Key Extension

- **Activation**: Enables the which-key extension.
- **Timeout Setting**: Disabled, displaying the menu until a key is pressed.
- **Menu for Vim Actions**: Disabled for default Vim actions like `gg` or `zz`.

#### NERDTree Support

- **Activation**: Integrates NERDTree-like file navigation within the project view.

#### Vim-Surround Emulation

- **Activation**: Emulates vim-surround plugin.
- **Commands**: Includes `ys`, `cs`, and `ds` for manipulating "surroundings" of text segments.

#### Argument Text Object

- **Activation**: Adds text objects for arguments: `aA` (around arguments) and `iA` (inside arguments).

---

**Note:** For all the actual mappings, refer to [.ideavimrc](./.ideavimrc)

## Mentions

Thanks to:

- [@Marcoleni](https://github.com/MarcoIeni) and his
  [intellimacs](https://github.com/MarcoIeni/intellimacs) project. I wouldn't have had the
  required patience to search up all the action mappings in IntelliJ IDEA myself, so, I ended up
  using this repository as a reference for my own [.ideavimrc](./idea/.ideavimrc) configuration file.
