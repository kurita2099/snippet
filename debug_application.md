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
		
		アプリが実行されたらエミュレーターを選択し、command + Mを押してDeveloper Menuを起動
		
		　adb shell input keyevent 82　→実際のアンドロイド端末
		 
		
	VSCODE上でデバッグ
		https://qiita.com/t_okkan/items/2b6b94340b837189054c

</div>
</details>
<details>
<summary>
	ADB をUSBでなくWIFI経由でワイヤレスにする
</summary>
<div>
$adb tcpip 5555
#restarting in TCP mode port: 5555

adb connect 接続したい端末のIPアドレス:ポート番号
次にネットワーク経由で接続したい実機のIPアドレスと設定したポート番号を指定してあげます。
(実機のIPアドレスについてはDHCPから静的な割当に設定しておくと捗るかもしれません。)

$adb connect 192.168.??.??:5555

</div>
</details>
