# Changelog

All notable changes to this project will be documented in this file.
Format: [Keep a Changelog](https://keepachangelog.com/en/1.1.0/) + [Semantic Versioning](https://semver.org/).

## [Unreleased]

### Added
- 初版公開: Synthesizer V .svp のブラウザ閲覧・編集ツール（単一HTML）
  - ピアノロール表示 / 編集（追加・移動・長さ・削除・複数選択・Undo/Redo）
  - 歌詞・音素編集（ダブルクリック/右クリックポップアップ、Tab連続入力）
  - まとめ歌詞入力（スペース/改行区切り・1文字ずつの順番割当）
  - 音素自動生成（公式JapaneseROMAJI音素表準拠）
  - 矩形波による再生プレビュー（メトロノーム・追従スクロール・停止モード切替）
  - 全体ビュー / 歌詞ストリップ / 複数トラック対応 (v1/v2/v3)
  - 自動保存 (localStorage) / .svp 書き出し
