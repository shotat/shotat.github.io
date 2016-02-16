---
layout: post
title: jekyll-composeを使うぞ
---

# jekyll-composeとは
jekyllのpluginである。

=> [jekyll-compose - GitHub](https://github.com/jekyll/jekyll-compose)

# Install
Gemfileに記述しよう

~~~ ruby
source "https://rubygems.org"

gem "github-pages"
gem "jekyll"

# これ！！！！！！！！！！！！！！
group :jekyll_plugins do
  gem "jekyll-compose" 
end
~~~

以下のコマンドを実行し、jekyll-composeが有効になっていることを確認。

~~~ sh
bundle install
jekyll -h
#=> post, publish等のsubcommandが追加されている
~~~

# How to use
こんな感じです

~~~ sh
jekyll post 'hogehoge'
#=> _posts/yyyy-mm-dd-hogehoge.md が生成

jekyll draft 'foobar'
#=> _drafts/foobar.md が生成

jekyll publish '_drafts/foobar.md'
#=> _posts/2016-02-16-foobar.md に移動

jekyll unpublish '_posts/foobar.md'
#=> _drafts/foobar.md に戻る
~~~

# まとめ
* front matterやら日付をよしなにしてくれる機能はjekyllにデフォでは入ってないっぽいので一緒にいれるとよさそう
* 他にもいいpluginがたくさんあるかも


