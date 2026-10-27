# Mr. President 非公式日本語化

**Mr. President: The American Presidency, 2001-2020**（Steam 版）を日本語で遊ぶための非公式パッチです。

> [!IMPORTANT]
> - これは有志による**非公式**の日本語化です。開発元・販売元・GMT Games の**公認ではありません**。
> - 開発元からは「共有は構わないが、公認はしない・責任は負わない」との回答を得ています。
> - 日本語化による不具合を**開発元・販売元に問い合わせないでください**。おかしいと思ったら、まず日本語化を外して英語でも起きるか確かめてください。
> - 利用は自己責任でお願いします。

## ダウンロード

右の **Releases** から、いちばん新しい `MrPresident_JA.zip` をダウンロードして展開してください。

## 使い方

1. ゲームを終了しておく
2. 展開した `MrPresident_JA` フォルダの **`MrPresident_JA.exe`** をダブルクリック
   - ゲームの場所を自動で探し、日本語化 MOD を作ってゲームの `~mods` フォルダに入れます（1〜2分）
3. ゲームを起動すると日本語で表示されます

- **ゲームが見つからないと言われたら**: `MrPresident_JA` フォルダごとゲームのフォルダ（`Mr. President`）の中に置いて実行してください。
- **ゲームがアップデートされたら**: もう一度 `MrPresident_JA.exe` を実行してください。更新で英語が変わった所は自動で英語のまま残ります。
- **元に戻す（英語に戻す）**: `restore.cmd` をダブルクリック

## 仕組み

- この配布物に**ゲームのデータは入っていません**。中身は訳文・日本語フォント・ツールだけです。
- ツールはあなたの PC のゲームから文字のデータを取り出し、文字だけを日本語に置き換えた MOD（`Content\Paks\~mods\zz_MrPresident_JA_P.*`）を作ります。ゲームの元のファイルは書き換えません。
- 初回の実行時、データの展開に使う retoc が圧縮ライブラリ（Oodle）を自動でダウンロードします。

## 翻訳について

- AI（Gemini）による翻訳に、ゲーム用語の用語集を当てて表記をそろえたものです。人手での確認は進行中です。
- 一部の画面に英語が残る所があります。

## 同梱物とライセンス

| 同梱物 | 用途 | ライセンス |
|---|---|---|
| BIZ UDPGothic | 日本語フォント | SIL Open Font License 1.1 |
| retoc | データの展開・MOD 作成 | MIT |
| UAssetAPI（exe に内蔵） | データの書き換え | MIT |

ライセンス文は ZIP の `licenses` フォルダにあります。

---

## English

Unofficial Japanese translation for **Mr. President: The American Presidency, 2001-2020** (Steam).

- This is an **unofficial** fan translation. It is **not endorsed** by the developer, the publisher, or GMT Games. The developer has said they don't mind it being shared, but they do not endorse it and take no responsibility for it.
- Please **do not report** problems caused by this translation to the developer or publisher.
- Use at your own risk.

Download `MrPresident_JA.zip` from **Releases**, extract it, close the game, and run `MrPresident_JA.exe`.
The package contains no game files. The tool reads text assets from your installed copy of the game, replaces only the displayed text, and writes a mod to `Content\Paks\~mods\zz_MrPresident_JA_P.*`. Run `restore.cmd` to remove it, and re-run the exe after game updates.
