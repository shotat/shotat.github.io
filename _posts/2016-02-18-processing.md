---
layout: post
title: MacにProcessingを導入
---

MacにProcessingを入れます。
Processingはデジタルアート的なものを比較的楽に作れる楽しい言語らしいです。

# Install
*Homebrew Cask*を使いましょう

[参考 - Macのセッティングが楽チンに！『Homebrew Cask』でソフトを簡単インストール](http://www.lifehacker.jp/2015/08/150823_homebrew_cask.htmla)

## Homebrew Caskのinstall

~~~sh
ruby -e "$(curl -fsSL https://raw.github.com/Homebrew/homebrew/go/install)"
brew tap caskroom/cask
brew install caskroom/cask/brew-cask
~~~

時間かかるかも
動かなかったら適宜ググってください

## Processingのinstall 

~~~sh
brew cask install Caskroom/cask/processing
~~~

普通のAppとして起動できるようになります。  
終わり
