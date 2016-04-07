---
layout: post
title: 深層学習を読んだ
---

## 深層学習を読んだ

この本 -> [深層学習](http://www.amazon.co.jp/%E6%B7%B1%E5%B1%A4%E5%AD%A6%E7%BF%92-%E6%A9%9F%E6%A2%B0%E5%AD%A6%E7%BF%92%E3%83%97%E3%83%AD%E3%83%95%E3%82%A7%E3%83%83%E3%82%B7%E3%83%A7%E3%83%8A%E3%83%AB%E3%82%B7%E3%83%AA%E3%83%BC%E3%82%BA-%E5%B2%A1%E8%B0%B7-%E8%B2%B4%E4%B9%8B/dp/4061529021)

機械学習の基礎知ってる || ニューラルネットワークなら説明できるぞ  
という人ならなんとなく理解できそう。

難しすぎず、易しすぎず、結構面白かったです。

## TensorFlowを使おう

僕は基礎研究や大学数学が苦手な雑魚なので、概ね理解できたらuser側に徹して行こうと思います。

というわけで今更ながらTensorFlowを使ってみます。

まずは導入。

### TensorFlow Install

公式ドキュメントに倣い？virtualenvを使いましょう。  
virtualenvのオプションとかは適当に。  
ちなみにMacです

~~~sh
$ sudo pip install --upgrade virtualenv
$ virtualenv --system-site-packages ~/tensorflow
$ . ~/tensorflow/bin/activate
(tensorflow)$ pip install --upgrade https://storage.googleapis.com/tensorflow/mac/tensorflow-0.7.1-cp27-none-any.whl
~~~

最後の`pip install`のpathはversionが変わると思われるので、公式をみましょう。

これでTensorFlowが使えるようになりました。  
以降virtualenvの実行/停止は  

~~~sh
(tensorflow)$ deactivate
$ . ~/tensorflow/bin/activate
~~~

で切り替えられます。

次回以降、ちゃんと使っていきます（使うとはいってない）。
