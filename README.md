# Color Preview for Obsidian

Obsidianのエディタおよび閲覧モードで、カラーコード（Hex, RGB, HSL等）を自動検知し、そのすぐ右側に色のプレビュー（小さな四角）を表示するプラグインです。

## 主な機能

* **完全自動認識**: 記法を工夫することなく、普段通りカラーコードを入力するだけでプレビューが表示されます。
* **マルチフォーマット対応**:
* Hex: `#ff0000`, `#f00`, `#ff0000ff`
* RGB/RGBA: `rgb(255, 0, 0)`, `rgba(255, 0, 0, 0.5)`
* HSL/HSLA: `hsl(0, 100%, 50%)`


* **全モード対応**:
* **Live Preview**: 入力中にリアルタイムで表示。
* **Reading View**: 閲覧モードでもしっかり表示。
* **Flashcards**: `Spaced Repetition` 等のプラグインによる学習画面でもプレビューを表示。


* **レスポンシブデザイン**: 四角のサイズは `1em` （文字サイズ）に設定されているため、見出しや本文など、フォントサイズに合わせて自動で調整されます。

## インストール方法

1. `main.js`と`manifest.json`をダウンロード
2. `保管庫root/.obsidian/plugin`にフォルダ，`color_preview`を作成
3. 作成した`color_preview`にダウンロードした`main.js`と`manifest.json`を移動
4. Obsidianの設定からプラグイン一覧をリロードして有効化してください。

## 使い方

ノートの中にカラーコードを書くだけです。

```markdown
この色は #ea609e です。
背景色は rgb(40, 44, 52) に設定されています。

```

入力した瞬間に、コードの右側にその色の小さな四角形が出現します。

## 開発スタック

* **Language**: TypeScript
* **Engine**: CodeMirror 6 (Editor Extensions)
* **Bundler**: esbuild

---

## ライセンス

MIT License
