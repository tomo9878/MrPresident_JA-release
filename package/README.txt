Mr. President: The American Presidency, 2001-2020 非公式日本語化
============================================================

■ 注意（必ずお読みください）
・これは有志による【非公式】の日本語化です。開発元・販売元・GMT Games の公認ではありません。
・開発元からは「共有は構わないが、公認はしない・責任は負わない」との回答を得ています。
・日本語化による不具合を、開発元・販売元に問い合わせないでください。
  おかしいと思ったら、まず日本語化を外して（restore.cmd）英語で再現するか確かめてください。
・利用は自己責任でお願いします。

■ 使い方
1. ゲーム（Steam 版）を終了しておく
2. MrPresident_JA.exe をダブルクリック
   → ゲームの場所を自動で探し、日本語化 MOD を作ってゲームの ~mods フォルダに入れます（1〜2分）
3. ゲームを起動すると日本語で表示されます

・ゲームの場所が見つからないと言われたら、このフォルダごとゲームのフォルダ（Mr. President）の中に置いて実行してください。
・ゲームがアップデートされたら、もう一度 MrPresident_JA.exe を実行してください。
  更新で英語が変わった所は、自動で英語のまま残ります（ゲームが壊れることはありません）。
・元に戻す（英語に戻す）: restore.cmd をダブルクリック

■ 仕組み
・この配布物にゲームのデータは入っていません。中身は訳文・日本語フォント・ツールだけです。
・ツールはあなたの PC のゲームから文字のデータを取り出し、文字だけを日本語に置き換えた MOD を
  Content\Paks\~mods\zz_MrPresident_JA_P.* として作ります。ゲームの元のファイルは書き換えません。
・初回の実行時、retoc がデータの展開に使う圧縮ライブラリ（oo2core_9_win64.dll）を自動でダウンロードします。

■ 翻訳について
・AI（Gemini）による翻訳に、ゲーム用語の用語集を当てて表記をそろえたものです。人手での確認は進行中です。
・一部の画面（ボタンなど）に英語が残る所があります。

■ 同梱物とライセンス（licenses フォルダ）
・BIZ UDPGothic（日本語フォント）: SIL Open Font License 1.1 — BIZ_UDPGothic_OFL.txt
・retoc（データの展開・MOD 作成）: MIT License — retoc_LICENSE.txt
・UAssetAPI（データの書き換え。exe に内蔵）: MIT License — UAssetAPI_LICENSE.txt
・data\MrPresident.usmap はゲームの型情報（データを読むための設計図）です。

------------------------------------------------------------
Unofficial Japanese translation for Mr. President: The American Presidency, 2001-2020

- This is an UNOFFICIAL fan translation. It is NOT endorsed by the developer, the publisher, or GMT Games.
  The developer has said they don't mind it being shared, but they do not endorse it and take no responsibility for it.
- Please do NOT report problems caused by this translation to the developer or publisher.
  If something seems wrong, remove the translation (restore.cmd) and check whether it also happens in English.
- Use at your own risk.

This package contains no game files. MrPresident_JA.exe reads text assets from your own installed copy of the game,
replaces only the displayed text, and writes a mod to Content\Paks\~mods\zz_MrPresident_JA_P.*.
The original game files are not modified. Run restore.cmd to remove it. Re-run the exe after game updates.
