# test_githubpages
GitHub Pages を試す。

# 公開 URL
https://stakiran.github.io/test_githubpages/

# GitHub Pages 仕様
from https://help.github.com/articles/what-is-github-pages/

- private repo の場合でも、GitHub Page は常に Public 
- Usage Limit: こいつら超えたらメールで警告出しますんで
  - データサイズは 1GB 超えないでね
  - 通信は月 100GB を超えないでね
  - ビルド(Jekyllを使った場合1push=1build)は10回/hまでにしてね
- 内容についても制限があるよ
  - まあ規約とかガイドラインに違反するなってことなんだけど、主なこと挙げとくと...
  - 暴力的、反社会的コンテンツ
  - 性的なコンテンツ
  - スパム
  - 名誉毀損
  - get rich quick scheme(儲け話)
  - 身元詐称

# 設定方法
Settings > Options > GitHub Pages

- Source: 公開する物件をどこに置くか
  - master: master ブランチに置いたものをそのまま使う
  - docs: master ブランチの docs フォルダ配下に置いたものをそのまま使う
- Theme: Jekyll を使った場合のテーマを選べる

## Jekyll？
ページを公開するためには index.html など HTML を自分で書く必要がある。

が、Jekyll という仕組みは、Markdown ファイルを push しておくと対応する HTML を生成してくれる。いわゆる静的サイトジェネレータってやつ。

マニュアルは https://help.github.com/articles/using-jekyll-as-a-static-site-generator-with-github-pages/ この辺見ればいいっぽい？

