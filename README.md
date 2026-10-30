# Mr. President 非公式日本語化

**Mr. President: The American Presidency, 2001-2020**（Steam 版）を日本語で遊ぶための非公式パッチです。

> [!IMPORTANT]
> - これは有志による**非公式**の日本語化です。開発元・販売元・GMT Games の**公認ではありません**。
> - 開発元からは「共有は構わないが、公認はしない・責任は負わない」との回答を得ています。
> - 日本語化による不具合を**開発元・販売元に問い合わせないでください**。おかしいと思ったら、まず日本語化を外して英語でも起きるか確かめてください。
> - 利用は自己責任でお願いします。

## 使い方

### 1. ダウンロード

1. このページ右側の **Releases** から、いちばん新しいリリース（Latest）を開く
2. **Assets** にある **`MrPresident_JA.zip`** をクリックしてダウンロード

### 2. 展開

1. ダウンロードした `MrPresident_JA.zip` を右クリック →「**すべて展開**」
2. 展開先はどこでも構いません（デスクトップなど）。`MrPresident_JA` フォルダが1つできます

> ZIP を開いたまま中の exe を直接実行すると、データが見つからず失敗します。必ず展開してから実行してください。

### 3. 日本語化する

1. **ゲームを終了**しておく（起動中だと日本語化できません）
2. `MrPresident_JA` フォルダの **`MrPresident_JA.exe`** をダブルクリック
3. 「Windows によって PC が保護されました」と出たら、「**詳細情報**」→「**実行**」を押す
   （署名のない exe なので表示されます）
4. 黒い画面が開き、次のように進みます（1〜2分）

   ```
   === Mr. President 日本語化（非公式） ===
   ゲーム: C:\Program Files (x86)\Steam\steamapps\common\Mr. President
   1/4 ゲームから文字のアセットを取り出しています…
   2/4 文字を日本語に置き換えています…
   3/4 日本語フォントを入れています…
   4/4 MOD を作っています…
   完了: 文字列表 6712 件・画面の文 839 か所・フォント 16 個を日本語化しました。
   ```

5. 「完了」と出たら Enter キーで閉じる
6. Steam からゲームを起動すると日本語で表示されます（ゲーム内の言語設定を変える必要はありません）

初回だけ、データの展開に使う部品（Oodle）を自動でダウンロードするため、インターネット接続が必要です。

### 元に戻す（英語に戻す）

ゲームを終了して、`MrPresident_JA` フォルダの **`restore.cmd`** をダブルクリックします。
日本語化 MOD（`Content\Paks\~mods\zz_MrPresident_JA_P.*`）が消えて英語に戻ります。

### ゲームがアップデートされたら

ゲームの更新で日本語化が外れたり、一部が英語に戻ったりすることがあります。
もう一度 **`MrPresident_JA.exe`** を実行してください。更新で英語の文が変わった所は、自動で英語のまま残します。

ただし、ゲームのエンジン自体が新しくなる大きな更新では、古い日本語化を入れたままだと**ゲームが起動しなくなる**ことがあります。
そのときは `restore.cmd` で外し、日本語化の新しい版（このページの Releases）を待ってください。

日本語化の新しい版が出たときは、新しい ZIP を展開して exe を実行するだけで上書きされます。

### 更新履歴

- **v2**（2026-10-31）: ゲームの更新（Unreal Engine 5.8）に対応。v1 を入れたままだと更新後のゲームが起動しないので、v2 の exe を実行し直してください
- **v1**（2026-10-28）: 最初の版

### うまくいかないとき

| 表示・症状 | 対処 |
|---|---|
| ゲームのフォルダが見つかりませんでした | `MrPresident_JA` フォルダごとゲームのフォルダ（`Mr. President`）の中に置いて実行する。または、コマンドプロンプトで `MrPresident_JA.exe --game "ゲームのフォルダ"` |
| ゲームが起動中です | ゲームを終了してから実行する |
| ファイルに書き込めませんでした | exe を右クリック →「管理者として実行」 |
| ゲームの更新後に起動しない・すぐ落ちる | 日本語化が古い版の可能性があります。`restore.cmd` で外せば起動します。新しい版の exe を実行し直してください |
| 一部が英語のまま | 翻訳していない所、またはゲームの更新で英語が変わった所です（詳細は exe と同じフォルダの `patch-log.txt`） |
| ゲームの表示や動作がおかしい | `restore.cmd` で英語に戻して同じことが起きるか確かめる。英語でも起きなければ日本語化の問題なので、開発元ではなくこのリポジトリの Issues へ |

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

Download `MrPresident_JA.zip` from **Releases**, extract it (do not run it from inside the ZIP), close the game, and run `MrPresident_JA.exe`. If Windows SmartScreen appears, click "More info" → "Run anyway". When it says it's done, press Enter and start the game. No in-game language setting is needed. An internet connection is required on the first run (to download Oodle).
The package contains no game files. The tool reads text assets from your installed copy of the game, replaces only the displayed text, and writes a mod to `Content\Paks\~mods\zz_MrPresident_JA_P.*`. Run `restore.cmd` to remove it, and re-run the exe after game updates.
After a major game update (new engine version) an old version of this mod can stop the game from starting; run `restore.cmd` and use the latest release.
v2 (2026-10-31) supports the game update to Unreal Engine 5.8.
