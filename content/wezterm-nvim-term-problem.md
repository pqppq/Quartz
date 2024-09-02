---
title: Weztermとneovimを使っているときに、terminal modeで変数が出力される
tags:
  - neovim
  - wezterm
---
[Command for setting user vars is being printed before each command #5007](https://github.com/wez/wezterm/issues/5007)

Wezterm + Tmux + Neovimでターミナルモードを使うときに、コマンドの前後で`SetUserVar=WEZTERM_PGOR=...`というような変数が毎回出力されてしまう.

- wezterm 20240203-110809-5046fc22
- Tmux v3.4
- NVIM v0.10.1
	- Build type: Release
	- LuaJIT 2.1.1713773202

![[assets/Pasted image 20240901122927.png]]