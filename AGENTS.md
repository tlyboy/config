# AGENTS.md

This file provides guidance to AI agents when working with code in this repository.

## Repository Overview

This is a personal development environment configuration files repository (dotfiles), used for syncing and managing development environment configurations across machines.

## File Structure

- `.zshrc` - Zsh main configuration file (Oh My Zsh, plugins, aliases, environment variables)
- `.zprofile` / `.zshenv` / `.profile` - Shell environment initialization files
- `.gitconfig` - Git global configuration
- `.editorconfig` - Editor common format configuration
- `.prettierrc` - Prettier formatting configuration
- `.vscode/` - VS Code workspace settings

## Code Style

- Indentation: 2 spaces
- Line endings: LF
- Character set: UTF-8
- Prettier: no semicolons, single quotes

## Common Shortcut Aliases (defined in .zshrc)

| Alias | Command |
|-------|---------|
| `d` | `nr dev` |
| `b` | `nr build` |
| `t` | `nr test` |
| `tw` | `nr test --watch` |
| `c` | `nr typecheck` |
| `lint` | `nr lint` |
| `lintf` | `nr lint --fix` |

`nr` is a command from [@antfu/ni](https://github.com/antfu-collective/ni), which automatically detects the package manager.

## Development Environment

- Node.js version management: fnm
- Package managers: supports npm/pnpm/yarn (via ni)
- Shell: Zsh + Oh My Zsh + Starship prompt
- Default editor: Cursor
