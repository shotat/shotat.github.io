---
layout: post
title:  "JekyllとGitHub Pages"
date:   2016-02-15 22:00:02 +0900
categories: jekyll update
---

# JekyllでGitHub Pagesを作るぞ

## とりあえず作る
適当なディレクトリで
{% highlight sh %}
$ mkdir <hogehoge>
$ cd <hogehoge>
$ bundle init
{% endhighlight %}

生成された`Gemfile`に、以下を記述
{% highlight ruby %}
source "https://rubygems.org"

gem "github-pages"
gem "jekyll"
{% endhighlight %}

そして
{% highlight sh %}
$ bundle install
{% endhighlight %}

しばらく待つ。
終わったら以下のコマンドを実行

{% highlight sh %}
$ jekyll new <foobar>
$ cd <foobar>
$ jekyll serve
{% endhighlight %}

すると`localhost:4000`でいろいろプレビューできる

## GitHub Pagesとして公開

1. `<username>.github.io`リポジトリを作る(privateでもok)
2. さっきの<foobar>をmaster branchにpush
3. 反映されるまでじっと待つ
4. おしまい

いろいろカスタマイズして知見が増えたら続く




