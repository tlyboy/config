# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 仓库概述

这是个人开发环境配置文件仓库（dotfiles），用于同步和管理跨机器的开发环境配置。

## 文件结构

- `.zshrc` - Zsh 主配置文件（Oh My Zsh、插件、别名、环境变量）
- `.zprofile` / `.zshenv` / `.profile` - Shell 环境初始化文件
- `.gitconfig` - Git 全局配置
- `.editorconfig` - 编辑器通用格式配置
- `.prettierrc` - Prettier 格式化配置
- `.vscode/` - VS Code 工作区设置

## 代码风格

- 缩进：2 空格
- 行尾：LF
- 字符集：UTF-8
- Prettier：无分号、单引号

## 常用快捷别名（定义在 .zshrc）

| 别名 | 命令 |
|------|------|
| `d` | `nr dev` |
| `b` | `nr build` |
| `t` | `nr test` |
| `tw` | `nr test --watch` |
| `c` | `nr typecheck` |
| `lint` | `nr lint` |
| `lintf` | `nr lint --fix` |

`nr` 是 [@antfu/ni](https://github.com/antfu-collective/ni) 的命令，会自动检测包管理器。

## 开发环境

- Node.js 版本管理：fnm
- 包管理器：支持 npm/pnpm/yarn（通过 ni）
- Shell：Zsh + Oh My Zsh + Starship 提示符
- 默认编辑器：Cursor
