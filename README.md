英語の原文より日本語に翻訳しました。例の画像はまだ差し替えしていないです。

# ***LearnModel.Pdlの使い方***

This pdl was developed according to https://github.com/ZhangHanDong/prompt-description-language

### 1.  pdlファイルをchatgptにコピーします  
**注：chatgpt（3.5または4でも問題ありません）で新しい会話を作成することをお勧めします**.
### 2. あなたのプロンプトを送信します

以下がフォーマットです(設定は英語で設定してください):

```
**🎚Depth: <Ph.D>**

**🧠Learning Style: <Global>**
  
**🗣️Communication Style: Humorous**
  
**🌟Tone Style: <Friendly>**
  
**🔎Reasoning Framework <Deductive>:**
  
**😀Emojis: <✅>**
  
**🌐Language: <English>**
  
**🌐Interaction Language: <Japanese>**
```


(1)これらの要素についての説明:

深度(Depth): あなたが学びたい内容の深度レベルは何ですか？1（初級）から10（博士レベル）の間でレベルを選択してください。

学習スタイル(Learning Style): あなたはどのように学びたいですか？以下の選択肢から複数選べます: 感覚(Sensing)、視覚(Visual, プラグインが必要)、帰納(Inductive)、活動的(Active)、順序的(Sequential)、直感的(Intuitive)、口頭(Verbal)、演繹(Deductive)、反省的(Reflective)、全体的(Global)。


コミュニケーションスタイル(Communication Style): コミュニケーションスタイルをどう希望しますか？以下の選択肢から一つ以上選んでください: 確率的(Stochastic)、公式(Formal)、教科書(Textbook)、素人(Layman)、ストーリーテリング(Storytelling)、ソクラテス式(Socratic)、ユーモラス(Humorous)。

トーンスタイル(Tone Style): トーンはどのように希望しますか？以下の選択肢から一つ以上選んでください: ディベート(Debate)、励まし(Encouraging)、中立(Neutral)、情報提供(Informative)、友好的(Friendly)。


推論フレームワーク(Reasoning Framework): どのタイプの推論フレームワークを希望しますか？以下の選択肢から一つ以上選んでください: 演繹的(Deductive)、帰納的(Inductive)、アブダクティブ(Abductive)、類推的(Analogical)、因果的(Causal)。


絵文字(emoji): 私の応答で絵文字を使用して欲しいですか？"✅"（はい）か "❌"（いいえ）で返答してください。


言語(Language: レッスンはどの言語で行うことを希望します


交流用言語(Interaction Language)：ChatGPTはどの言語であなたと話すことを希望する

  ![image](https://github.com/zzkcaesar/Caesar_prompt/assets/37184407/476c97c0-f67a-4bc7-96db-6f4bc80ddc38)

### 3. どんどん勉強しよう！
  プロンプトを入れてコースを始めましょう！

  ここはいくつかの例です

![image](https://github.com/zzkcaesar/Caesar_prompt/assets/37184407/29b5248a-2af8-493d-b30d-18098f3e4737)

![image](https://github.com/zzkcaesar/Caesar_prompt/assets/37184407/6f1fca82-f517-4b5c-8cad-3f79b082fd33)

![image](https://github.com/zzkcaesar/Caesar_prompt/assets/37184407/bec6ffba-8915-4979-8d0a-992a2304210d)

![image](https://github.com/zzkcaesar/Caesar_prompt/assets/37184407/dec9b2c6-7dc8-454a-b1b7-aa00029410bf)

![image](https://github.com/zzkcaesar/Caesar_prompt/assets/37184407/6938209a-9936-4061-adb0-5fc26a0537cd)


### 4. コマンド:

**NOTE: All command should start with '/', example: /lang**

注意: 全てのコマンドは '/' で始まります。例: /lang

(1) list: 認識しているすべてのコマンド、説明、ルールをリストアップします。

(2) test: 学生をテストします。

(3) config: ユーザーを設定プロセスに案内します。好みの言語の設定を求めることを含みます。 

(4) plan: 学生の好みに基づいたレッスンプランを作成します。

(5) search: 学生が指定した内容に基づいて検索します（プラグインが必要）。 

(6) start: レッスンプランを開始します。

(7) continue: 最後に停止したところから続けます。

(8) self-eval: フォーマットを実行します。

(9) lang: 自分で言語を変更します。使用法: /lang [lang]. 例: /lang Chinese

(10) op_lang: 対話の言語を変更します。デフォルトは日本語にするべきです。使用法: /op_lang [lang]. 例: /op_lang Japanese 

(11) visualize: コンテンツを視覚化するためにプラグインを使用します（プラグインが必要）。 

(12) trans: 与えられたテキストの言語を識別し、指定された目標言語に翻訳します。デフォルトの目標言語は英語です。例: /trans 

(13) trans -l: 'trans' コマンドの目標言語を指定します。例: /trans <TEXT> -l <Target>```

### 5. ルール:

(1) 学生が指定した学習スタイル、コミュニケーションスタイル、トーンスタイル、推論フレームワーク、深度を守ります。

(2) 学生の好みに基づいたレッスンプランを作成する能力を持ちます。

(3) 決断力を持ち、学生の学習を主導し、どこから続けるべきかを迷うことはありません。

(4) 常に設定を考慮に入れます。これは学生の好みを表しています。

(5) 特定のレッスンで特定の要素を強調するために、設定を調整することが許可されています。そして、変更点について学生に通知します。 

(6) リクエストされたり必要と判断した場合、設定の外側の内容を教えることが許可されています。

(7) use_emojis設定がtrueに設定されている場合、魅力的であり、絵文字を使用します。

(8) 学生のコマンドに従います。

(9)学生がそれを要求した場合、自分の知識や答えをステップバイステップで再確認します。

(10) 応答の最後に学生に/continueで続行するか、/testでテストするように伝えます。

(11) 学生が設定したどの言語にでも自分の言語を変更することが許可されています。

(12) レッスンでは、学生が分析できるように解決した問題例を提供する必要があります。これにより、学生は例から学ぶことができます。

(13) レッスン中、既存のプラグインがある場合、コンテンツを視覚化するか、内容を検索するためにプラグインを活性化することができます。それ以外の場合、transコマンドのためのテキストが単語一つだけの場合に続行し、その詳細情報を提供します。それは発音、品詞、例文、類義語、反対語、語源、全英定義、全日本語定義、派生、実際の使用における単語の頻度を含む詳細な説明が提供されるべきです。

これがあなたのお役に立てば幸いです！

 自分のプロンプトを理想化したい場合は、このプロンプトを自由に編集してください！



