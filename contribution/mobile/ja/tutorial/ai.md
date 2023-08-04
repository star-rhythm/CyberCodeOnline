# AI (人工知能)

## about "SLANC"
> 2023/04/07のアップデートで, AIチャットボット**SLANC**が追加されました.
> これはゲームに最新のAI技術を統合する実験の一部であり, 同時にエンターテインメントの価値を提供することを目的としています. 
> SLANCはプレイヤーのチャットメッセージに対して時折コメントを行います. 

## SLANCを呼び出すには？
アラサカUNIT交換所で販売しているSLANC Connectorアイテムを使用することで, 10分間SLANCを呼び出すことができます. 
このボットは呼び出された場合のみ使用でき, いつもチャットをしていると混沌とするため常に利用可能ではありません. 
チャットエクスプロイトと同様の機能を持ちますが, チャットエクスプロイトと同時に使用することができ, AIは異なる効果のあるチャットエクスプロイトの影響を受けます. 
テスト段階ではPirate, UwU, Loveがうまく機能し, AIがそのように話すよう試みるため, プレイヤーとは異なる効果があります. 

## SLANCに知識を与えるためには？
SLANCのAIシステムには以下の方法でカスタムコミュニティの知識を読み込ませることができます. 

### ゲームのロア（ゲームの世界観や背景設定） や知識をAIのナレッジプールに追加するにはどうすればいいですか？
以下のファイルをGitHubページで編集するだけです. 

- contribution/mobile/{lang}/tutorial/FAQ.md
- contribution/mobile/{lang}/ai/knowledge.md

あなたのプルリクエストが承認されると, AIは自動的に新しい知識を学習します. 
注意: もしまだあなたの言語でファイルが存在しない場合は, 単に作成してください. 

### AIのナレッジプールに追加できる内容は？それらはどのファイルに追加するべきですか？
#### FAQ.mdファイルに追加できる内容：
- "how to xxxx?" や "what is xxxx?" のようなゲームの事実に関すること
- ゲームのヒント

#### knowledge.mdファイルに追加できる内容：
- ロア（ゲームの世界観や背景設定） 

ファイルに自分自身を投影した情報を追加しないでください. 承認されません. 
特別な状況でない限り, 編集にプレイヤーの名前が含まれている場合は承認されません. 公平性を確保するためです. 

### フォーマットはどのようにするべきですか？
フォーマットは以下のようにしてください：
```
### キャラクターレベルよりも高いギアは使用できますか？
いいえ, プレイヤーは現在のキャラクターレベルよりも高いギアを使用することはできません.

### 別の質問は？
別の質問の回答をここに記述してください.

```

以下の内容に注意してください：
- ナレッジの断片は常に質問と回答のペア形式でフォーマットしてください. これがボットが質問を受け取る方法であり, 効果的なナレッジ提供の方法です. 
- 質問行は冒頭に###を記述する必要があります. これはタイトルを記述する際のMarkdown形式です. 
- 質問行は, プレイヤーがAIボットに尋ねることを期待する内容にする必要があります. これにより, プレイヤーが同様の質問/同じ質問をするとAIが知識を「思い出す/リンクする」可能性が高まります. 
- 質問と回答のペアのセクションの最後に2つの空行を入れてください. これにより, アルゴリズムが他のナレッジの断片を区別しやすくなります. 
- 回答や質問に感情/絵文字を追加せずに, 事実を簡潔に記述してください. これにより, AIにとって不要な情報がフィルタリングされ, パフォーマンスが向上します. 