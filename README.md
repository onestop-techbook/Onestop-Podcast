# Re:VIEWテンプレート

## 概要説明
ワンストップ　Podcast

## この本の目的
アウトプットの一つの形として、Podcastがあります。
情報源としても、様々な技術について知る手段としても、Podcastはいいですね。
本は満員電車の中は開きづらいですが、Podcastはイヤホンで聞けるので。
そして、発信してみるのも楽しいものです。

## 概要目次
ワンストップPoscast

テクニカルパート
・聞く側
　・Podcastの説明
　・なぜ聞くのか
　・どう聞くのか(ソフト、
　・どうやって探す？(コミュニティ、スパキャス(DiscordのPodcasterのコミュニティ)
・始め方
　・配信方法
　・方針ぎめ(ひとり語り？ゲスト？、方針？
　・ネタ出し
　・機材　ハード、ソフト
・続け方
　・継続の壁
　・ゲストの探し方？がんばる？つぶやいたらいっぱい来た
　・収録ノウハウ(ゲストノート、事前に聞いておくこと。
　・収録場所(オンライン、オフライン、ラボ、会議室？注意点、反響、救急車問題、大通り避ける、電車避ける)
　・収録時に気をつけていること。進行のテクニック
　・インタビュースキル(鉄板質問
　・マイクテクニック(声の出し方、波形を見るとか)
　・編集テクニック
アンケート：
 ・なにをやっているか
 ・なぜやっているのか
 ・これから始めたい人にひとこと。
 ・宣伝＆URL

## 執筆・配布スケジュール
募集開始・環境構築　4月27日  
章目次確定：5月末日  
本文初稿：6月15  
レビュー＆追記：6月末日  
入稿:7月5日
発行　技書博(7/27蒲田Pio)
を大枠なスケジュールとします。(多少前後します)

## 著者紹介兼あとがき
Contributers.re内に、テンプレートに従って記入ください。

## 執筆にあたってのお願い
CIでコンパイルが通ることを確認してください。エラーのまま放置はなるべくやめてください。

Confrictが発生した場合は、解決お願いします。

push -f等はやめましょう。（歴史を書き換えてはいけません。

相談事：
Issue立ててください。

雑談、ざっくばらんな相談については、Slackがあります。
参加方法は、親方まで。https://twitter.com/oyakata2438/
## Re:VIEWの書き方

[Re:VIEWチートシート](https://gist.github.com/erukiti/c4e3189dda179a0f0b73299fb5787838) を作ってみたので、参考にしてみてください。

## CI
https://app.wercker.com/oyakata2438/Onestop-Podcast/runs
でPDFが書きだされます。
一番上のBuildをクリックすると展開されるので、
Output Artifactをクリックして、Download artifactをクリックすると、
tarで固めたpdfがダウンロードできます。

## インストール

細かい準備(TeX入れたり)は[『技術書をかこう！』](https://github.com/TechBooster/C89-FirstStepReVIEW-v2)に準じます。

### WindowsでReviewを使う方法

https://qiita.com/implicit_none/items/398c6e0bbedc8b160621
暗黙の型宣言さんが詳しく書いてくれてます。あるいは、技術同人誌を書こう‐アウトプットのススメ‐をご覧ください。

### Dockerを使う方法

Dockerを使うのが一番手軽です。

```sh
$ docker run --rm -v `pwd`:/work vvakame/review /bin/sh -c "cd /work/articles ; review-pdfmaker config.yml"
```

### Docker使わずビルド

```sh
cd articles ; review pdfmaker config.yml
```

> Visual Studio Code で `Onestop-meeting` フォルダーを開くと、ビルドタスク `Build PDF with Re:VIEW` を使ってこのコマンドを実行できます。

### 権利

ベースには、[TechBooster/ReVIEW\-Template: TechBoosterで利用しているRe:VIEWのテンプレート（B5/A5/電子書籍）](https://github.com/TechBooster/ReVIEW-Template) を使っています。

  * 設定ファイル、テンプレートなど制作環境（techbooster-doujin.styなど）はMITライセンスです
    * 再配布などMITライセンスで定める範囲で権利者表記をおねがいします
