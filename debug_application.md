#アプリのデバッグの仕方
<details>
<summary>
WEBアプリ（Javascript)
</summary>
<div>
　　PC →CHROMEのデバッガー（PC）
   
　　モバイル
	重要→android 
		https://qiita.com/kfunnytokyo/items/b19ce8b8ef7792841f22

	iPhone
	WINの場合
	https://qiita.com/riversun/items/6646ea1afdd17b96a5b2
	MACの場合
	https://qiita.com/unsoluble_sugar/items/2a3d06631a6b8259dc44
	(※ sourcemapが読み込まれず webpack.config.jsに
　　　　　devtool: 'inline-source-map'追記しビルドしたjavascriptにsource-mapを書き出す）
</div>
</details>
<details>
<summary>
	ReactNaive
</summary>
<div>
		ブラウザでデバッグ
			run in web Browser
			↓
			chrome のデバッグツール
		https://qiita.com/takaishota/items/96802dc7e522aeba058b

		android端末（シュミレーター ）でデバッグ
			PC上で　adb接続
https://tech.la-fra.com/2018/07/29/post-204/
https://developer.android.com/studio/releases/platform-tools

		android Studioからシミュレータをインストール
		サードパーティのシュミレーター 
			NOXPLAYER
			GenyMotion
		などをインストールし　開発モードにする

</div>
</details>
