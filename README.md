## 七四式電子観測儀拡張版 / ElectronicObserverExtended (EOE)
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2FCAWAS%2FElectronicObserverExtended.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2FCAWAS%2FElectronicObserverExtended?ref=badge_shield)


現在鋭意開発中の艦これ補助ブラウザです。  


## 実装されている機能

![](https://github.com/andanteyk/ElectronicObserver/wiki/media/mainimage2.png)

各機能はそれぞれウィンドウとして独立しており、自由にドッキング・タブ化するなどしてレイアウト可能です。  
以下では概略を紹介します。**詳しくは[Wikiを参照](https://github.com/andanteyk/ElectronicObserver/wiki)してください。**  

* 内蔵ブラウザ(スクリーンショット, ズーム, ミュートなど)
* 艦隊(状態(遠征中, 未補給など), 制空戦力, 索敵能力)
    * 個艦(Lv, HP, コンディション, 補給, 装備スロット)
    * 艦隊一覧(全艦隊の状態を一目で確認できます)
    * グループ(フィルタリングで艦娘情報を表示)
* 入渠(入渠艦, 残り時間)
* 工廠(建造中の艦名, 残り時間)
* 司令部(提督情報, 資源情報)
* 羅針盤(次の進路, 敵編成・獲得資源等のイベント予測)
* 戦闘(戦闘予測・結果表示)
* 情報(中破絵未回収艦一覧, 海域ゲージ残量など)
* 任務(達成回数/最大値表示)
* 図鑑(艦船/装備図鑑)
* 装備一覧
* 通知(遠征・入渠完了, 大破進撃警告など)
* レコード(開発・建造・ドロップ艦の記録など)
* ウィンドウキャプチャ(他プログラムのウィンドウを取り込む)

なお、全ての機能において艦これ本体の送受信する情報に干渉する操作は行っていません。


## About ElectronicObserverExtended / 拡張版について

ElectronicObserverExtended implements Plugin APIs introduced by [tsanie's fork](https://github.com/tsanie/ElectronicObserver). This allows developers to add functionalities that can be distributed in a .dll file.

To maintain compatibility with plugins developed for tsanie's fork, ElectronicObserverExtended chains a FiddlerCore proxy in front of Nekoxy. ElectronicObserverExtended with no plugins installed should behave exactly the same as the original ElectronicObserver, except:

* It by default uses UTF-8 as file encoding.
* It always respect system proxy settings, as designed by FiddlerCore.

[Download Extended / 拡張版のダウンロード](https://ci.appveyor.com/project/CNA-Bld/electronicobserverextended/build/artifacts)


## ダウンロード

[リリースページ](https://github.com/andanteyk/ElectronicObserver/releases) もしくは [配布ブログ](http://electronicobserver.blog.fc2.com/) を参照してください。

[更新内容・履歴はこちらで確認できます。](https://github.com/andanteyk/ElectronicObserver/wiki/ChangeLog)  


## 開発者の皆様へ

[開発のための情報はこちらに掲載しています。](https://github.com/andanteyk/ElectronicObserver/wiki/ForDev)  

[Other/Information/](https://github.com/andanteyk/ElectronicObserver/tree/develop/ElectronicObserver/Other/Information) に艦これのAPIや仕様についての情報を掲載しています。  
ご自由にお持ちください。但し内容は保証しません。  

[ライセンスは MIT License です。](https://github.com/andanteyk/ElectronicObserver/blob/master/LICENSE)  


## 使用しているライブラリ

* [DynamicJson](http://dynamicjson.codeplex.com/) (JSON データの読み書き) - [Ms-PL](https://github.com/andanteyk/ElectronicObserver/blob/master/Licenses/Ms-PL.txt)
* [DockPanel Suite](http://dockpanelsuite.com/) (ウィンドウレイアウト) - [MIT License](https://github.com/andanteyk/ElectronicObserver/blob/master/Licenses/DockPanelSuite.txt)
* [Nekoxy](https://github.com/veigr/Nekoxy) (通信キャプチャ) - [MIT License](https://github.com/andanteyk/ElectronicObserver/blob/master/Licenses/Nekoxy.txt)
    * [TrotiNet](http://trotinet.sourceforge.net/) - [GNU Lesser General Public License v3.0](https://github.com/andanteyk/ElectronicObserver/blob/master/Licenses/LGPL.txt)
        * [log4net](https://logging.apache.org/log4net/) - [Apache License version 2.0](https://github.com/andanteyk/ElectronicObserver/blob/master/Licenses/Apache.txt)
* [SwfExtractor](https://github.com/andanteyk/SwfExtractor) (swf からファイル抽出) - [MIT License](https://github.com/andanteyk/ElectronicObserver/blob/master/Licenses/SwfExtractor.txt)
	* [LZMA SDK (Software Development Kit)](http://www.7-zip.org/sdk.html) - Public Domain
* [FiddlerCore](http://www.telerik.com/fiddler/fiddlercore) - [End User License Agreement for FiddlerCore](https://github.com/CAWAS/ElectronicObserverExtended/blob/extended/Licenses/FiddlerCore.txt)



[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2FCAWAS%2FElectronicObserverExtended.svg?type=large)](https://app.fossa.io/projects/git%2Bgithub.com%2FCAWAS%2FElectronicObserverExtended?ref=badge_large)

## 連絡先など

* 配布サイト:[ブルネイ工廠電気実験部](http://electronicobserver.blog.fc2.com/) (バグ報告・要望等はこちらにお願いします)
* 開発:[Andante](https://twitter.com/andanteyk)
* 拡張版開発:[中国ホワイト（アルバム）学院](https://github.com/CAWAS)