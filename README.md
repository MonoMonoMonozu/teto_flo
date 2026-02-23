# 🦊 flowchart_quest_withTeto

> 「こうしたいけどできない」をAIと話すだけで、PLAN A/B/C のフローチャートに仕上げてくれるアプリ。

**QuestQueries** は「真面目なことを、プチ冒険として。」をコンセプトにした実験的なAIツール集です。  
No.3 Teto Flow は、その汎用入口として作られました。

---

## ✨ どんなアプリ？

プロンプトを書かなくていい。フレームワークを知らなくていい。  
テトに話しかけるだけで、いつの間にか**PLAN A/B/C のフローチャート**ができています。

```
「マラソン練習したいけど続かなくて…」
    ↓ テトが友達感覚で深掘り
「じゃあこんな感じでどう？」（構成案を提示）
    ↓ OK を返すだけ
フローチャートが自動生成 → HTML でコピー保存
```

---

## 🚀 使い方

### 1. ファイルを開く

`index.html` をブラウザでダブルクリックするだけ。インストール不要。

### 2. APIキーを設定する

初回起動時にモーダルが表示されます。  
[Anthropic Console](https://console.anthropic.com/settings/keys) で取得した APIキー（`sk-ant-...`）を入力してください。

> ⚠️ **使用量の上限を設定することを強く推奨します。**  
> → [使用量上限の設定はこちら](https://console.anthropic.com/settings/limits)  
> キーはあなた自身の Anthropic アカウントに紐づいており、課金もあなたのアカウントに発生します。

### 3. テトと話す

自然な言葉で悩みを話しかけてください。  
テトが 2〜3 往復で深掘りし、PLAN A/B/C の構成案を提示します。  
「いいね」「これで」と返すと、自動でフローチャートが描画されます。

### 4. HTMLをコピーして保存

右パネルの **「📋 HTMLをコピー」** ボタンを押す  
→ メモ帳などに貼り付けて `.html` で保存  
→ ダブルクリックで開けばフローチャートが見られます

---

## 🛠️ 技術構成

| 項目 | 内容 |
|---|---|
| 実行環境 | ブラウザのみ（サーバー不要） |
| AI | Anthropic Claude API（claude-sonnet-4） |
| 図の描画 | [Mermaid.js](https://mermaid.js.org/) |
| フォント | Zen Kaku Gothic New / Space Mono（Google Fonts） |
| データ保存 | APIキーのみ localStorage に保存（会話履歴は保存しない） |

### ファイル構成

```
flowchart_quest_withTeto/
└── index.html   # アプリ本体（1ファイル完結）
```

---

## 🦊 テトについて

ナウシカとテトの関係性がベース。  
無口な相棒が突然話しかけてきて、一緒に問題を解いていく。  
押しつけず、でも深いところまで掘る。**2026年の初夢感。**

---

## 📋 QuestQueries シリーズ

| No. | 名前 | テーマ |
|---|---|---|
| No.1 | 星読み | 日々の振り返り × 占い |
| No.2 | マラソンクエスト | 走ることをゲーム化 |
| **No.3** | **Teto Flow** | **汎用フレームワーク入口** |

---

## ⚖️ ライセンス

MIT License  
Feel free to fork, remix, and use as a starting point for your own quests.

---

*「真面目なことを、プチ冒険として。」― QuestQueries*
