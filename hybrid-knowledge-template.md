以下のYAMLデータを「粒度を保ったまま構造化する上位バージョン」として再構成してyaml-codeblock出力してください。分類カテゴリごとにまとめ、structured / raw_facts の両方を出力してください：
```yaml
{{ここに変換対象のyamlを記述}}
```

構造参考例：
```yaml
# ============================================================
# Hybrid Knowledge Template (generic)
# ------------------------------------------------------------
# - 目的: “粒度を保ったまま構造化する上位バージョン” を
#   あらゆるドメインの情報整理に再利用できる汎用フォーマット。
# - 構造: 各カテゴリごとに
#     1) structured  … 機械可読な key–value 形式
#     2) raw_facts   … 元の自然文を一切改変せず保持
#   をペアで配置することで、詳細粒度と再利用性を両立する。
# ============================================================

hybrid_doc:
  meta:
    title: "<ドキュメントのタイトル>"
    version: "1.0.0"
    language: "ja"
    description: >
      <このドキュメントの目的や適用範囲を簡潔に記述>
    last_updated: "<YYYY-MM-DD>"

  categories:
    #----------------------------------------
    - id: "<カテゴリ識別子: 例 overview, configuration, usage など>"
      name: "<カテゴリ名（日本語も可）>"

      structured:
        # *** ここに key–value 形式で要約・仕様を記述 ***
        # 例:
        #   feature_enabled: true
        #   max_limit: 100
        #   default_state: "off"
        # ※ ネストは自由。配列・オブジェクトいずれも可。
        <key>: <value>

      raw_facts:
        # *** ここに元の文章を文単位でそのまま列挙 ***
        - "<一次情報そのままの文章を記入>"
        - "<同上>"
        # 必要に応じて何行でも追加可

    #----------------------------------------
    # 追加カテゴリは‐ (ハイフン) で増やすだけ
    - id: "<another_category_id>"
      name: "<カテゴリ名>"

      structured:
        <key>: <value>

      raw_facts:
        - "<元の文>"
```

output_format:
```yaml

```
