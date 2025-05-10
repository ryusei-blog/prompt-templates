AI用プロンプトを再利用可能なYAMLテンプレート集です。  
ブログ記事を書くすべてのライター・マーケター向けに設計。  
コピペするだけで構成作成から引用元探しまで時短できるプロンプトを色々と取り揃えていきます！

**各種プロンプトは、[こちらのページ](https://ryusei-blog.github.io/prompt-templates/)から簡単にコピーができます！**

## 📑 テンプレート一覧

| ファイル | 役割 / 使いどころ | プロンプト |
|--|--|--|
| `primary_source_finder.yml` | 渡されたMarkdown 記事から**引用・統計などが書かれた箇所を抽出　→　一次情報 URL を検索**し、Markdown テーブルで返す。ChatGPT o3に対して使うのがおすすめ。 | [open](https://ryusei-blog.github.io/prompt-templates/#psf) |
| `toc_outline_generator.yml` | ブログ記事の目次を作ってもらうためのプロンプト。合わせて、記事テーマを指定してください。 | [open](https://ryusei-blog.github.io/prompt-templates/#tog) |
| `prompt-drill-universal-template.yml` | AIに役割（role）と課題（task）を与えて、AI講師としてユーザーを教育させるためのプロンプトです。例えば「role: "ベテランSEOランナー"」と「task: "SEO初心者であるユーザーにSEOの問題を出題する"」といった使い方ができます。 | [open](https://ryusei-blog.github.io/prompt-templates/#pdut) |
| `fermi_estimator_prompt.yml` | 高度な推論能力を持つAIモデルへの指示に最適な、フェルミ推定をさせるためのプロンプトです。ユーザーは`task: ""`を設定するだけでOK。何か特定のテーマを与えて実行させてみましょう。 | [open](https://ryusei-blog.github.io/prompt-templates/#fep) |
| `fermi_insight_analyzer_prompt.yml` | 上記`fermi_estimator_prompt.yml`の出力結果をもとに、対象が感じていそうな課題や次に取りそうな行動を論理的に導出するプロンプトです。ビジネス戦略の仮説検証や施策立案の補助として活用できます。`fermi_estimator_prompt.yml`の実行直後にそのまま使えます。 | [open](https://ryusei-blog.github.io/prompt-templates/#fiap) |
| `strategy_implementation_prompt.yml` | 上記2つのフェルミ推定で得られた市場規模と課題分析をもとに、具体的な戦略設計・施策立案・実装ロードマップまでを一気通貫で導出するためのプロンプトです。ブログ記事や提案資料の骨子づくりに活用できます。 | [open](https://ryusei-blog.github.io/prompt-templates/#sip) |
| `client_acquisition_flow_prompt.yml` | ベテランの職能エージェントとして、フリーランスが案件を獲得し目標収益を実現するための行動計画を設計します。目標年収や月間稼働時間などを設定するだけで案件獲得を支援してくれます。 | [open](https://ryusei-blog.github.io/prompt-templates/#cafp) |
| `gpts_knowledge_setup.yml` | ChatGPTのGPTsの情報をインプットさせるためのセットアップ用プロンプトです。ChatGPTは自分の機能のくせにGPTsの仕様を全て把握していないため、それを分からせるための教育プロンプトです。 | [open](https://ryusei-blog.github.io/prompt-templates/#gks) |
| `hybrid-knowledge-template.md` | 自然文で書かれた仕様や事実リストを「粒度を保ったまま構造化」するためのハイブリッドYAMLテンプレートを提供します。structured形式で機械可読性を確保しつつ、raw_factsで元の情報を完全保存。AI活用・ドキュメント整備・ナレッジ管理に最適です。 | [open](https://ryusei-blog.github.io/prompt-templates/#hkt) |
