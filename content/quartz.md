---
title: Quartzを使ってObsidianで管理するマークダウンをGithub Pagesにデプロイする
tags:
  - Quartz
  - Obsidian
  - Note-Taking
---
[Quartz](https://quartz.jzhao.xyz/)を使うことでObsidian PublishのようにObsidianで管理するマークダウンを静的サイトとしてデプロイできる. 以下を参考に作業をした.

- [How to publish Obsidian notes with Quartz on Github Pages](https://notes.nicolevanderhoeven.com/How+to+publish+Obsidian+notes+with+Quartz+on+GitHub+Pages)
- [Obsidian + Quartz + Github Page を使ってサイト公開](https://note.com/devlive/n/n3250edc2ee8f)

作業としては、
- QuartzをcloneしたレポジトリとObsidianのVaultのレポジトリを作成
- QuartzのレポジトリをVaultのレポジトリのサブモジュールに追加する
	- Obsidianの設定でサブモジュールも含めて自動コミットされるように設定する
- Github Pagesにデプロイするためのワークフローを追加する

画像はVault内の`Quartz/content/assets`に作成するようにし、[CrawlLinks](https://quartz.jzhao.xyz/plugins/CrawlLinks)プラグインでパスを解決するようにすると表示された. (Files and linksで`Relative path to file`にした.)

とりあえず、Github Pagesで見れるようになったので、
- ドメインの設定
- レイアウトとスタイル調整

をそのうち実施する.
