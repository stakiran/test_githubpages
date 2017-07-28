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
    - それじゃ足りない？ じゃあ Release 機能使うなり別のホスティングサービス使うなりしてちょ
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

# Jekyll 試す
[Markdownで書かれたページをGitHub Pagesで公開する - @yoshiki_utakata](http://yoshikyoto.github.io/text/git/gh_pages_md.html) やら [Jekyll + github pages を使って git + markdown でサイト構築 | akkunchoi@github](http://akkunchoi.github.io/jekyll-github-blogging.html) を参考にしつつ、最低限の構成を試す。

todo
- [ ] CSS 適用する

## take1
markdown エンジン redcarpet はサポートされてないんだとー。

```
The page build completed successfully, but returned the following warning for the `master` branch:

You are currently using the 'redcarpet' Markdown engine, which is no longer supported by GitHub Pages and may cease working at any time. To ensure your site continues to build, remove the 'markdown' setting in your site's '_config.yml' file and confirm your site renders as expected. For more information, see https://help.github.com/articles/updating-your-markdown-processor-to-kramdown/.

For information on troubleshooting Jekyll see:

  https://help.github.com/articles/troubleshooting-jekyll-builds

If you have any questions you can contact us by replying to this email.
```
