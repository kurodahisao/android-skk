# 多言語改変版 SKK for Android

このソフトは,
[海月玲二氏の SKK for Android](http://ray-mizuki.la.coocan.jp/software/skk_jp.html) を
多言語入力用に少し改変したものです.
個人的に欲しい機能も加えています.

### 主な変更点

- 英字キーボードの多言語化 (後述)
- 日本語キーボードのポップアップ, 変換候補のデザインの変更
- 音声入力キー, マッシュルームキーの削除
- 一部機能の追加

## 概要

[minghai 氏の SKK for Android](https://minghai.hatenadiary.org/entry/20090502/p1) に
[海月玲二氏がフリック入力に改変したもの](http://ray-mizuki.la.coocan.jp/software/skk_jp.html)
を,
多言語で入力できるよう改変したキーボードです.
日本語入力は SKK のまま, Gboard のように多言語で入力できるキーボードを目指しています.

## インストール

[Release](https://github.com/xiupos/android-skk/releases)

ビルドには [hkusu 氏作成のワークフロー](https://qiita.com/hkusu/items/30843c34f569d9a14fef) を使っています.

### 動作環境

手元にあった以下の端末にて動作を確認しています.

- Sony Xperia 10 II (Android11),
- Sharp AQUOS Sense4 lite (Android11) 

それ以外の環境で動く保証はありません.
自己責任で確認をお願いします.

IOSに対応する予定はありません.

## 機能・使い方

> **最初に一回だけ, 変換辞書を内部ストレージに解凍する作業が必要です.**
設定画面から「辞書ファイル解凍」を選んでください．

以下に挙げる機能以外はほとんど改変していません.
SKK for Androidの機能に関する詳しい使い方は
[海月玲二氏のページ](http://ray-mizuki.la.coocan.jp/software/skk_jp.html) を参照してください.  

SKK自体の使い方については [ニコニコ大百科](https://dic.nicovideo.jp/a/skk) がわかりやすいです.


### 日本語

改変した機能は以下の通りです.

 - 音声入力キー, マッシュルームキーの削除
 - 矢印キーをフリックすることで上下左右に移動できる
 - スペースキーを左にフリックすることでシフトができる
 - カンマキーを下にフリックすることで `...` (ドット3つ)が入力できる
 - 小文字キーを上にフリックすることで `w` が入力できる
 - **や** キーを左右にフリックすることで `(` `)` が入力できる
 - **わ** キーを下にフリックすることで `~` が入力できる
 - ポップアップ, 変換候補を黒基調のデザインに変更

### ヨーロッパ諸言語

日本語キーボードの左下の **ABC** キーによって切り替えることができます.
ヨーロッパ諸言語は **スペース** キーを左右にフリックすることで切り替えられます.

また, **. ,** のキーを分離し, 
矢印キーをフリックすることで上下左右に移動できるようにしています.

想定している言語は以下の通りです.  
( **太字** は直接入力可能な言語,
その他はキーを長押しすることで入力可能な言語 )

  1. ギリシア文字キーボード: **現代ギリシア語**, 古典ギリシア語, [コプト文字](https://ja.wikipedia.org/wiki/%E3%82%B3%E3%83%97%E3%83%88%E6%96%87%E5%AD%97)  
    ギリシア文字を基に, 対応するコプト文字を配置.

  1. エスペラントキーボード: **エスペラント**, ポーランド語  
    QWERTY 配列にエスペラント特有の文字を追加, 不要な文字を削除し,
    ザメンホフの母国語であるポーランド語を配置.

  1. ラテン語キーボード: **ラテン語**, **英語**, フランス語, スペイン語, イタリア語, ポルトガル語, ラトヴィア語, チェコ語  
    QWERTY 配列に **·** を追加.
    上記言語に必要な装飾付き文字を配置.

  1. ドイツ語キーボード: **ドイツ語**, オランダ語, デンマーク語, ノルウェー語, スウェーデン語, オランダ語, 古英語, ルーン文字  
    QWERTY 配列に **ä ö ü** を追加.
    上記言語に必要な特殊文字, 装飾付き文字を配置.
    また対応する文字にルーン文字を配置.

  1. ロシア語キーボード: **ロシア語**, グラゴル文字  
    ロシア語配列に対応するグラゴル文字を配置
    (グラゴル文字の関係で一部の文字には初期キリル文字も配置).

それぞれのキーの配列は Gboard にあるものを参考にしています.
また, 長押しで入力できる文字の位置は Wikipedia などを参考に, 
音価や歴史的な経緯を踏まえて適当に配置していますが,
一部のキーはスペースなどの関係で隣のキーに割り当てているものもあります.

特定言語の無効化, 順番等を設定する機能はありません.

## 注意

**私は言語学の専門家ではありません**.
また, Android開発も初心者 (ラーメンタイマー程度の開発力) ですので,
気に入ったら Contribute して頂けると嬉しいです.

### TODO

  - ヨーロッパ諸言語キーボードの切り替え直後のキーが反応しない
  - 特定言語の無効化, 順番等を設定する機能
  - デザインがデフォルトのまま
  - 非ヨーロッパ言語の追加 (アラビア文字など)
  - ヨーロッパ諸言語キーボードのポップアップの調整
  - 追加機能を設定で有効・無効できるように (小文字キーの `w` など)
  - キーマップの追加

## 謝辞

2009年にSKKをAndroid用に実装し，ソースと詳説を公開してくださったminghai氏に感謝します．
また，minghai氏のAndroid用SKKを大幅に改良し，同じくソースと詳説を公開してくださった海月玲二氏に感謝します．

## リンク

- [minghai氏の SKK for Android](https://minghai.hatenadiary.org/entry/20090502/p1)
- [海月玲二氏の SKK for Android](http://ray-mizuki.la.coocan.jp/software/skk_jp.html)

## 正字正假名 (by KURODA Hisao)
 - 「わ」行から「ゐ」と「ゑ」を入力できるやうにした。
 - 以下の版でbuildできるやう改變を加へた。
```
   openjdk version "17.0.11" 2024-04-16
   OpenJDK Runtime Environment (build 17.0.11+9-Debian-1deb12u1)
   OpenJDK 64-Bit Server VM (build 17.0.11+9-Debian-1deb12u1, mixed mode, sharing)
   ------------------------------------------------------------
   Gradle 4.4.1
   ------------------------------------------------------------
```
 - （Java Security Policy の變更で?）辭書に access できないため AndroidManifest.xml に <provider.../> を追加し、application private 領域を Ghost Commander などから access できるやうにした。
    - ここに手動で辭書を置いてやれば辭書追加操作ができるやうになる。
    - npiii.l.jis (kstn.fc2web.com/seikana_zisyo.html) を utf8 に變換したものを npiii.l.txt として置いたが "SKK 辭書管理"→「辭書を追加」しても反映されないので、"SKK ユーザー辭書ツール" で npiii.l.txt を「インポート」してから「エクスポート」で一旦 skk_userdict.txt に保存し、これを改めて「辭書を追加」適用してやると、一先づ正字正假名環境にすることができた。
      - 目視確認の結果、 skk_userdict.txt と npiii.l.txt の違ひは sort されてゐるか否か。
      - moto g32(w)  Android version 11 で動作確認。
 - おそらく original の作者は、辭書に、
```
     # /#3/#2/
     #y /#2年/#3年/#0年/
     #おくえん /#3億圓/
     だい# /第#3/
```
   のやうな entry があった場合の動きについて、知らないか完全無視をしてゐる。
    - 力まかせに初めてのJavaを書いて、上例の一部が成功するやうにした。
```
      1978y → 一九七八年
      18c → 十八世紀
      112304560789120 → 百十二兆三千四十五億六千七十八萬九千百二十
```
    - 未だをかしな動きが目立つ上に時々落ちる…
