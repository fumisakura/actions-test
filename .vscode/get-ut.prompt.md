---
agent: 'agent'
model: GPT-4.1 (copilot)
tools: ['search/codebase']
description: '現在のファイルで選択された関数のユニットテストを生成する'
---

次の関数のテストを書きます：

${selection}

適切なフレームワークを使ってテストスイートを生成してください。

- 依存がある場合、モックを利用します
- テストコードは`${fileBasenameNoExtension}.test$\`に追加します
- 意味のあるテストケース名をつけてください
- ${fileDirname} に'__tests__'フォルダが存在する場合、そちらにテストコードを追加してください

有効なコードのみを返してください
