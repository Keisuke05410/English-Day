# English-Day

エンジニア向け英語学習リポジトリ。日々の業務で使える実践的なフレーズ・表現パターンを1日1つ学習する。

## 学習カテゴリ

以下のカテゴリから実践的なフレーズを選定:

- **定型表現（phrase）** - ビジネスでよく使う決まり文句
- **議論の型** - 議論を進める・深めるための表現
- **合意形成の型** - チームで合意を取るための表現
- **曖昧性処理** - 不明確な点を確認・明確化する表現
- **オーナーシップ移譲** - タスクや責任を渡す・受け取る表現
- **意思決定** - 決定を促す・伝える表現
- **反対と妥協** - 異論を唱える・折り合いをつける表現

## ディレクトリ構成

```
Day{N}/
  word.md      - フレーズとその意味・ニュアンス・使い方
  question.md  - 日本語で書かれた英作文問題
  answer.md    - question.mdの解答（英文）
words_list.md  - 全Dayのフレーズをまとめたリスト
questions.md   - 全Dayの問題をまとめたリスト
answers.md     - 全Dayの解答をまとめたリスト
```

## 各ファイルの形式

### word.md
```markdown
# Day{N}: {フレーズ}

- **カテゴリ**: {学習カテゴリ}
- **意味**:
- **ニュアンス**:
- **使用シーン**:
- **例文**:
```

### question.md
```markdown
# Day{N} 問題

以下の日本語を英語に訳してください。

{日本語文}
```

### answer.md
```markdown
# Day{N} 解答

{英文}
```

### questions.md
```markdown
# Questions

1. {Day1の問題}
2. {Day2の問題}
...
```

### answers.md
```markdown
# Answers

1. {Day1の解答}
2. {Day2の解答}
...
```

## コマンド

### /word
新しいDayディレクトリと全ファイルを生成し、GitHubにpushする。
- 次のDay番号を自動判定
- 学習カテゴリから実践的なフレーズを1つ選定
- word.md、question.md、answer.md を作成
- words_list.md、questions.md、answers.md に追記
- 変更をcommitしてpush（コミットメッセージ: "Add Day{N} content: {フレーズ}"）

## words_list.md の更新

/word実行時に以下の形式で追記:
```markdown
- Day{N}: [{カテゴリ}] {フレーズ}
```
