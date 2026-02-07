# HYL セミナーサイト 追加手順

このリポジトリでは、**技術記事**と**セミナー告知**を分けて管理しています。以下の手順に沿って追加してください。

## 1. 技術系記事（運用 実践解説）の追加方法

**配置先**
- `/Users/curtis/github/financial-seminar/content/tech/`

**新規ファイル例**
```
/Users/curtis/github/financial-seminar/content/tech/2026-02-your-topic.md
```

**Front Matter（必須）**
```yaml
---
title: "記事タイトル"
date: 2026-02-07
---
```

**本文（例）**
```
## 概要
ここに内容を書きます。

## 注意点
本文を追加します。

※ 本記事は情報提供を目的としたものであり、特定の金融商品の売買や投資判断を推奨するものではありません。
```

**ポイント**
- `date` を入れると「公開日」に正しい日付が表示されます。
- 技術記事はトップページの「運用 実践解説」に自動表示されます。
- 画像を使う場合は `/Users/curtis/github/financial-seminar/pic_res/` に保存します。

---

## 2. セミナー告知の追加方法

**配置先**
- `/Users/curtis/github/financial-seminar/content/posts/seminar/`

**新規ファイル例**
```
/Users/curtis/github/financial-seminar/content/posts/seminar/2026-06-seminar-sample.md
```

**Front Matter（必須）**
```yaml
---
title: "セミナー名"
date: 2026-02-07

# セミナー情報
status: "upcoming"         # upcoming / past
categories: ["FX", "Options"]
event_date: 2026-06-20
event_time: "20:00–20:30"
location: "オンライン（Zoom）"
level: "初級〜中級"        # 任意
---
```

**本文（例）**
```
## セミナー概要 📌
概要を書きます。

## 対象者 🎯
- 対象者1
- 対象者2

## 開催形式 🧭
開催形式を書きます。

## 申込方法 ✉️
会社宛メール（sales@hyl-inc.com）または担当者（韓 昌）まで直接ご連絡ください。

## 進行形式 🔎
HYL市場戦略チーム作成の資料をもとに、参加者同士で自由に意見を交わし、実践的な知見の共有を行います。

## 参加費 💴
初級：33,000円  
ご参加いただいた方には、Amazonギフト券（30,000円分）を特典としてご用意しております。

## 資料 📄
当日資料は社内資料として取り扱い、セミナー終了後に内部メールで参加者へ送付します。

※ 本セミナーは情報提供および教育目的で実施されるものであり、特定の金融商品の売買や投資判断を推奨するものではありません。最終的な投資判断はご自身の責任において行ってください。
```

**ポイント**
- `status` を `upcoming` にすると開催予定に表示されます。
- `status` を `past` にすると過去開催として表示されます。
- `categories` は複数指定可能です。指定範囲は以下の3つです。
  - `Futures`
  - `FX`
  - `Options`
- 画像を使う場合は `/Users/curtis/github/financial-seminar/pic_res/` に保存します。

---

## 画像の挿入方法

**画像の保存先**
- `/Users/curtis/github/financial-seminar/pic_res/`

**Markdown での書き方（例）**
```
![図の説明](/financial-seminar/pic_res/your-image.png)
```

**注意**
- GitHub Pages 配下の公開 URL は `/financial-seminar/` なので、画像のパスは `/financial-seminar/pic_res/...` を使ってください。
