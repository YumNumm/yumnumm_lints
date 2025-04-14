# yumnumm_lints

[@YumNumm]の好みをまとめた dart lintパッケージ

> [!IMPORTANT]
> なお、本パッケージは[@YumNumm]の気まぐれで破壊的な変更を含むアップデートを行います。
> [@YumNumm]が関与しないコードで利用することは強く推奨しません。
>
> なお、pub.devに公開する予定もありません。

## how to use?

1. このリポジトリを `dev_dependencies` に追加

- 追加で [`custom_lint`]と[`altive_lints`]も導入してください
  - [`altive_lints`]はAltive社が作成しているLintパッケージです
    - custom_lint経由でいくつかのルールを適用するために利用しています
    - なお、[`custom_lint`]と[`altive_lints`]を`dev_dependencies`に追加しない場合、`custom_lint`のルールは適用されません

```yaml
dev_dependencies:
  altive_lints: ^1.19.1
  custom_lint: ^0.7.5
  yumnumm_lints:
    git:
      url: https://github.com/YumNumm/yumnumm_lints.git
      ref: main # Commit hashで指定してもOK
```

1. `analysis_options.yaml` に以下を追加

```yaml
include: package:yumnumm_lints/analysis_options.yaml
```

完了です! 開発頑張ってください!

[`altive_lints`]: https://pub.dev/packages/altive_lints
[`custom_lint`]: https://pub.dev/packages/custom_lint
[@YumNumm]: https://github.com/YumNumm
