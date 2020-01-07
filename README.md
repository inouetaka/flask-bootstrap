

## ディレクトリ構成

┣ run.py   
┣ requirements.txt  
┣ .gitignore  
┣ config.py  
┣ instance/  
│    &emsp;&emsp;└ config.py  
└ app   
&emsp;&ensp;┣ \_\_init__.py  
&emsp;&ensp;┣ forms/  
&emsp;&ensp;┣ models/   
&emsp;&ensp;┣ views/   
&emsp;&ensp;┣ statics/  
&emsp;&ensp;└ templates/ 



ファイル/ディレクトリ|使い方
:--:|:--:
run.py|開発用サーバの実行用スクリプトでプロダクション用としては使わない。
requirements.txt|依存パッケージを記述。開発用と本番用を用意してもいいと思う。
config.py|アプリに必要な設定変数を記述。
instance/config.py|APIキーやDBのURI、バージョン管理に含まれない設定変数を記述
app|アプリを含むパッケージ
app/_\_init__.py|アプリの初期化用スクリプトで、様々なコンポーネントを読み込む
app/views/|ルートを定義
app/models/|アプリのモデル(のクラス)を定義するファイルもしくはディレクトリ
app/forms/|フォームを定義
app/static/|公開用のCSS, JavaScript, 画像等のアプリで公開すべきファイル置き場
app/templates/|テンプレート置き場(今回はbootstrap?)
