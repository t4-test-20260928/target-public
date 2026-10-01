# target-public

**検証用の public な target repo。本物の仕事はしない。**

GitHub Actions セキュリティゲートの PR チェックが、public な source repo
（`gate-source-public`）から public な target repo へ required workflow として
届くかを確かめるために置いている。

> **⚠ `.github/workflows/insecure-sample.yml` は意図的に非準拠に書いたテスト用のファイル。**
> ゲートがそれを検出できるかを確かめるためだけに存在する。他のリポジトリにコピーしないこと。
> 実行されないよう止めてある（発火しない `branches:` フィルタ / job は `echo` のみ）。

仕様の正本は `t4-test-20260928/gate-source`（private）の `docs/spec.md`。
