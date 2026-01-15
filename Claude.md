# English-Day

エンジニア向け英語学習リポジトリ。日々の業務で頻出する英語表現を1日1テーマで学習する。

## ディレクトリ構成

```
Day{N}/
  word.md      - 英単語・フレーズとその意味・ニュアンス
  question.md  - 日本語で書かれた英作文問題
  answer.md    - question.mdの解答（英文）
words_list.md  - 全Dayの単語をまとめたリスト
```

## 各ファイルの形式

### word.md
```markdown
# Day{N}: {単語/フレーズ}

- **意味**:
- **ニュアンス**:
- **例文**:
```

### question.md
```markdown
# Day{N} 問題

「{単語/フレーズ}」を使って、以下の日本語を英語に訳してください。

{日本語文}
```

### answer.md
```markdown
# Day{N} 解答

{英文}
```

## コマンド

### /word
新しいDayディレクトリと全ファイルを生成する。
- 次のDay番号を自動判定
- エンジニア業務で頻出の単語・フレーズを1つ選定
- word.md、question.md、answer.md を作成
- words_list.mdに追記

## 単語選定の基準

以下のシーンで使う英語を優先:
- コードレビュー
- 技術ドキュメント作成
- チームコミュニケーション（Slack、ミーティング）
- 障害対応・インシデント報告
- 設計議論
- プルリクエスト・Issue

## words_list.md の更新

/word実行時に以下の形式で追記:
```markdown
- Day{N}: {単語/フレーズ}
```
