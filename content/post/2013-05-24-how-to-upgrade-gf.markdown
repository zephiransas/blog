---
categories:
- Java
- JavaEE
- GlassFish
comments: true
date: 2013-05-24T00:00:00Z
title: GlassFishのアップグレード方法
url: /blog/2013/05/24/how-to-upgrade-gf/
---

会社で使ってるJenkinsさんはGlassFish上で動いているんですが、これのアップグレードを行ったので、そのメモ。

具体的にはGlassFish 3.1.1からGlassFish 3.1.2へアップグレードしました。

## updatetoolのインストール
まずはアップグレードに使用するupdatetoolをインストールします。

方法はasadminと同じディレクトリにある、updatetoolを実行するだけ。

初めてupdatetoolコマンドを実行した際に、updatetoolをインストールするか聞いてきますので、yを押してインストールするだけです。

ちょっと時間がかかるので、アニメでも見ながらゆっくり待ちましょう。

## updatetoolからGlassFishのアップグレード
上記の手順でupdatetoolのインストールが終了したら、もう一度updatetoolコマンドを実行します。するとGUIが立ち上がって来ますので、以下のようにするだけ。

![updatetool](/images/20130524/updatetool.png)

あとは

``` bash
$ ./asadmin version
```

などで、アップグレードできていることを確認しましょう。
