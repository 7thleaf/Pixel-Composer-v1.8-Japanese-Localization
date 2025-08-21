# Pixel Composer v1.8 日本語化

このリポジトリは **Pixel Composer v1.8** 向けの日本語ローカライズデータです。翻訳対象は **`words.json`** と **`UI.json`** のみで、**`nodes.json` は未翻訳**です。

---

## 対応バージョン

* v1.8.x を想定（それ以外は未検証）

## 収録・対象

* `UI.json`（UI テキスト）
* `words.json`（各種文言）
* `nodes.json` は **未着手**

## 導入方法

1. 本リポジトリの日本語フォルダ（例：`ja/`）を、Pixel Composer のインストール先へ配置します。
   * *アプリを起動し、画面上部 `Help > Open local directory`を選択して出てくるフォルダのLocaleファイルの中に`ja`を配置
2. アプリを再起動し、`File > Preference > Interface > Interface Language` から **ja** を選択。
3. 再起動すると日本語化が反映されます。

### （任意）フォント設定

* 日本語表示には CJK 対応フォントを推奨（例：**Noto Sans JP**、**Source Han Sans**）。
* フォントを同梱/使用する場合は `ja/fonts/` に `.ttf/.otf` を置き、`ja/fonts/fonts.json` の `path` を実ファイル名に合わせてください。
* 日本語は単語間スペースを使わないため、`ja/config.json` に `{"per_character_line_break": true}` を入れると折り返しが安定します。

## 注意事項

* `AppData\Local\PixelComposer\locale\en.json` は起動時に上書きされるため、**直接編集しないでください**。
* v1.8 以外の環境では文言ずれ・挙動差が発生する可能性があります。

## 変更提案 / フィードバック

* 変更提案は **GitHub Issues** を立てるか、公式 Discord の **community** チャンネルにある **日本語化スレッド** へ書き込みをお願いします。

## 既知の問題

* 一部 UI の文が長い場合に折り返しやレイアウトが崩れることがあります（フォント/サイズ/`config.json` で調整してください）。

## アンインストール

* `data/locale/ja` フォルダを削除し、言語設定を英語へ戻してください。

## クレジット

* Translation by Tikuzenni
