# phoneme-japanese-romaji.json について

このファイルは、Synthesizer V エディタが音素自動生成に使用する
「日本語 - ローマ字 (JapaneseROMAJI)」の音素定義をJSON化したものです。

- 元データ: Synthesizer V 公式ドキュメント / エディタ内蔵の音素表 (JapaneseROMAJI)
- 用途: svp-viewer の「音素自動生成」機能が、かな歌詞をローマ字音素列へ変換する際に参照
- 形式: セクションごとに `phoneme`（音素記号）/ `example`（例: あ → a）を列挙

## 変換ルール（実装反映済み）

| かな | 音素 |
|------|------|
| ん | N |
| っ | cl（子音の前ではその子音の前詰め表現） |
| 長音 (ー) | 直前の母音の延長（例: あー → a a） |
| 拗音 (きゃ/しゅ/ちょ 等) | 1トークン: ky / sh / ch + 母音 (例: きゃ → kya) |

出典: Dreamtonics Synthesizer V 公式音素表 (JapaneseROMAJI)
本ファイルはツールの動作に必要な変換表として同梱しています。
