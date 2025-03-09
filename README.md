# Camp Buddy 非公式日本語パッチ

## 概要

BLitsによるBLノベルゲーム、[Camp Buddy](https://www.blitsgames.com/product/camp-buddy-digital-download/) の非公式日本語パッチです。

### 注意事項

 * パッチにはゲームのデータは含まれていません。ゲーム自体は[ダウンロードページ](https://www.blitsgames.com/product/camp-buddy-demo/)からダウンロードして下さい。
 * このパッチは Demo ver1.3 に対応しています。

## 設定方法

### 方法１ : Gitを使う

Gitを使う場合はこちらの方法で設定して下さい。

`Camp_Buddy_Demo-1.3-pc` > `game` フォルダ内で下記コマンドを実行して下さい。

```
$ git clone git@github.com:IceBlue15/Camp_Buddy_Demo_tl.git tl
```

### 方法２ : Zipでダウンロードする

Gitを使わない場合はこちらの方法で設定して下さい。

1. 本ページの[Code]ボタン > [Download ZIP] を選択し zip ファイルをダウンロード
1. `Camp_Buddy_Demo-1.3-pc` > `game` フォルダ内に解凍
1. フォルダ名を `Camp_Buddy_tl-main` から `tl` に変更

### 設定後のフォルダ構成

フォルダ構成が以下のようになればOKです。

```
Camp_Buddy_Demo-1.3-pc
 └ game/
     └ tl/
         ├ japanese/
         ├ None/
         │  ├ fonts/
         │  └ setting.rpy
         └ README.md
```

### 言語切り替え

このゲームはプレイ中に言語を切り替えることはできません。
ゲームを終了し、 `None` フォルダ内の `setting.rpy` をテキストエディタで下記のように編集して下さい。

##### 日本語プレイ用の設定

```
init python:

    config.language = "japanese"
```

##### 英語プレイ用の設定

```
init python:

    config.language = "None"
```

編集したらファイルを上書き保存し、ゲームを起動して下さい。

## パッチの削除方法

ゲームを終了し、`tl` フォルダを削除して下さい。

## Font License

* [Noto Sans CJK JP](https://www.google.com/get/noto/#sans-jpan) is lisenced under the [SIL Open Font License, Version 1.1](http://scripts.sil.org/cms/scripts/page.php?item_id=OFL).
