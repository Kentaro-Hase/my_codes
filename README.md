# my_codes

## tracking_cyclone.py について
当スクリプトは気象庁55年長期再解析（JRA-55）（Ebita et al. 2011; Kobayashi et al. 2015）の海面更正気圧データを用いて低気圧の抽出およびトラッキングを行います。  
[爆弾低気圧データベース](http://fujin.geo.kyushu-u.ac.jp/meteorol_bomb/algorithm/index.php)の登録およびJRA-55の使用許可が事前に必要となります。  
当スクリプトを実行する際にはコマンドラインで以下のように入力して実行してください。  
$ python tracking_cyclone.py （NCARで登録したメールアドレス）　（NCARで登録したパスワード）  

また，当スクリプトはPython3を用いて実行しますが，標準モジュール以外に以下のモジュールを使用します。そのうち，pygribはWindows環境下でインストールすることができません。  
macOSあるいはLinux環境下でインストールしてください。  
numpy, pygrib, scipy

当スクリプトは，  
長谷健太郎・竹見哲也（2018）：日本域における春季の降水特定，日本気象学会2018年度春季大会  
で使用している低気圧の抽出・トラッキングの手法に基づいています。  
その為，春季に限定した低気圧の抽出・トラッキングとなっております。 　　
このアルゴリズムは[爆弾低気圧データベース](http://fujin.geo.kyushu-u.ac.jp/meteorol_bomb/algorithm/index.php)のアルゴリズムを参考に作成しました。  
