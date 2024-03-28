---
title: ホーム
layout: home
nav_order: 1
---
# CFM Weather 0.4.0 マニュアル
CFM Weather は、コミュニティFM向けの災害情報を収集する、Windows用アプリです。

[気象庁防災情報XMLフォーマット形式電文の公開（PULL型）](https://xml.kishou.go.jp/xmlpull.html) を取得して表示します。  

## 対応する電文
「随時」と「地震火山」のAtomフィードで配信される、以下の電文を取得します。 
それぞれのフィードには、「長期フィード」と、「高頻度フィード」の2種類があり、設定で切り替えることができます。
- 随時　[高頻度フィード](https://www.data.jma.go.jp/developer/xml/feed/extra.xml)　[長期フィード](https://www.data.jma.go.jp/developer/xml/feed/extra_l.xml)
    - 気象警報・注意報（Ｈ２７）
    - 熱中症警戒アラート
- 地震火山　[高頻度フィード](https://www.data.jma.go.jp/developer/xml/feed/eqvol.xml)　[長期フィード](https://www.data.jma.go.jp/developer/xml/feed/eqvol_l.xml)
    - 震源・震度に関する情報
    - 津波警報・注意報・予報a
    - 噴火警報・予報
    - 火山現象に関する海上警報・海上予報
    - 火山の状況に関する解説情報

## 動作環境
- OS: Windows10 または Windows11
- CPUアーキテクチャ: x64 (ARM,X86には非対応)
- インターネット接続
- mailtoプロトコルに対応するメーラー (Thunderbird, Outlook, メール(WIndows標準) , New Outlook で動作確認済み)