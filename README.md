# note自動化AI組織（Claude Code用テンプレート）

Claude Codeで、リサーチ・記事作成・タイトル・校正チェック・集客の5役を分業させ、
note記事を自動で仕上げるためのテンプレートです。詳しい解説は下記のページを参照してください。

https://smitch-ai-works.github.io/no20-claude-code-ai-note-organization/

## 使い方

```
git clone https://github.com/smitch-ai-works/no20-claude-code-ai-note-organization.git note-ai-team
cd note-ai-team
claude
```

Claude Code が起動したら、`/note_start` と入力してください。テーマを聞かれるので答えると、
5人のAIが順番に動き、記事本文・タイトル案3つ・SNS告知文が仕上がります。

## 中身

```
.
├── CLAUDE.md                     ← 全体ルール（トーン・NGワード等）
└── .claude/
     ├── agents/
     │    ├── researcher.md       ← リサーチ担当
     │    ├── writer.md           ← 記事作成担当
     │    ├── title-maker.md      ← タイトル担当
     │    ├── proofreader.md      ← 校正チェック担当
     │    └── marketer.md         ← 集客担当
     └── skills/
          └── note_start/
               └── SKILL.md       ← 5人を順番に動かす手順書
```

## 自分のジャンルに合わせて書き換える

`CLAUDE.md` の「全体ルール」と、各エージェントファイルの中身を書き換えれば、
note以外（ブログ・SNS運用など）にもそのまま応用できます。
