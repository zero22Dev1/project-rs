メモ
--flexGrid
[FlexGrid](https://support.mescius.jp/hc/ja/articles/7062326065039--FlexGrid-for-WinForms-複数行の固定行-列ヘッダー-で-セルをカスタムマージする方法)



デンソーHTのやり方
[デンソー](https://www.denso-wave.com/ja/adcd/support/technical/webmanual/bht_intro/man_setup_transfer_07.html)
	1.	FTPサーバーの準備：
	•	WindowsのIIS（Internet Information Services）などのFTPサーバーソフトウェアをインストールし、起動します。
	•	FTPサーバーのホームディレクトリに、BHTにダウンロードするアプリケーションプログラム（拡張子：PD4）を配置します。 
	2.	BHTの設定：
	•	[SF]キーと[1]キーを同時に押しながら電源を入れ、システムメニューを起動します。 
	•	[SET SYSTEM] > [TCP/IP] > [SET TCP/IP] > [DEVICE]を選択し、[TCP/IP DEVICE]を[COM1]、[LINK LAYER]を[ETHERNET]に設定します。 
	•	同じく[IP ADDRESS]で、BHTのIPアドレス、サブネットマスク、デフォルトゲートウェイを設定します。すべて「0.0.0.0」と設定すると、DHCPが有効になります。 
	•	[SET FTP] > [SERVER]を選択し、FTPサーバーのIPアドレス、ユーザーID、パスワード、デフォルトディレクトリを入力します。 
	3.	アプリケーションのダウンロード：
	•	システムメニューで[FTP] > [DOWNLOAD]を選択し、FTPダウンロードメニューを起動します。 
	•	[DIR/FILE]にダウンロードするプログラムのディレクトリとファイル名を入力し、[ENT]キーを押してダウンロードを開始します。 
	•	ダウンロードが完了すると、完了メッセージが表示されます。

詳細な手順や注意点については、デンソーウェーブの技術情報ページをご参照ください。  
