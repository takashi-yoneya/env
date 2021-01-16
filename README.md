# プログラム開発環境について
当方が推奨するプログラムを開発するための各種環境について纏めます。

## 総合開発環境
- VSCODE
Microsoft製のソースコードエディタです。とても使いやすいので、導入必須です。  
参考:https://qiita.com/zhikto/items/b255cc9c00fd42862d5e

## オススメPythonライブラリ
Pythonは優秀なライブラリが多いことでも有名です。下記のライブラリは案件でもよく使われるものなので
ぜひ慣れておくとよいでしょう。
- selenium  
ブラウザを自動操作するスクレイピングには必須のライブラリです。
- requests  
ブラウザを自動操作しないスクレピングには必須のライブラリです。
APIの実行にも使用できます。
- pandas  
大量のデータを扱うのが得意なライブラリです。データの入出力から、フィルタリング、検索など
様々な機能があります。
- eel  
デスクトップアプリをhtmlベースで簡単に作成できるライブラリです。
- pyinstaller  
作成したソースコードをpythonなしで実行できるようにするためのライブラリです。
- pytest  
テストを効率的に実行できるようにするためのライブラリです。
- dotenv  
環境変数をソースコードに記述せずに、.envというファイルにまとめて記述して呼び出せるようにするためのライブラリです。  
インストールは、python-dotenv　と指定する必要があります。
- logging  
ログ出力を簡単にできるようにするためのライブラリです。
以下GITHUBにこのライブラリを簡単に使用できるようにしたものをUPしているので  
ご活用ください。  
https://github.com/marutoraman/logger

## ソースコードの保管・バージョン管理(Git)
プログラムのバージョン管理が簡単に行えるツールです。当方のカリキュラムではGithubにソースコードを保管します。
以下に簡単なGitの使い方をまとめてありますので参考にしていただければと思います。  
https://github.com/marutoraman/git-study/blob/main/README.md

## Python仮想環境
案件でプログラムを作成する場合は、案件毎に仮想的な開発環境を構築することが望ましいです。  
こうすることで、プロジェクト間の無用な干渉を気にする必要がなくなります。  

仮想環境は、以下のコマンドで作成できます。  
[venv]の部分は作成する仮想環境のフォルダ名なので、何でも良いのですが  
慣例的にvenvとすることが多いです。  
｀python -m venv [venv]｀

作成したvenvフォルダ内のvenv/Scripts/python.exeをpythonのインタープリタに設定し  
ターミナルを起動してください。  
コマンドの初めに(venv)と表示されていたら、仮想環境が有効になっているので  
その状態でpipでモジュールをインストールやpython実行を行ってください。  
説明動画(音無し):https://i.gyazo.com/073fe373278d20464e907f8f0a085608.mp4

## テスト
プログラムを書く上でテストはとても重要です。 
テストを蔑ろにすると、品質が悪くなり、後から修正が多発するので  
結果的に多くの時間がかかることになります。  

当方は、1つのpyファイルに対して、1つのtest用のpyファイルを作成してテストすることを推奨しています。  
以下の動画で詳しく解説しています。  
https://youtu.be/68YLZ_o08B8

## サーバー環境
ローカルPCだけでなく、サーバーで実行したいという要件は、よくあります。
GCP、Azure、Firebase、herokuなどの様々な環境がありますが
将来性や拡張性を考えて当方はAWSを推奨しております。

最初はかなり難しいと感じるかもしれませんが、一度覚えれば、似たようなことの繰り返しなので  
ぜひ覚えて欲しいところです。

## DBクライアント
Djangoの開発を行う場合は、必然的にDBとの連携が必要になります。  
Djangoの管理画面からもDBの内容は参照可能ですが  
使い勝手が悪い他、エンジニアとしてはDBの中身を見て判断できることが望ましいため  
DBクライアントのインストールを推奨しています。

様々はDBクライアントがありますが、当方は、以下のツールを使用しています。  
https://forest.watch.impress.co.jp/library/software/heidisql/

## タスク管理
Trelloというカード方式のタスク管理ツールが案件でも良く使われています。  
https://trello.com/

## クラウドメモ管理
Stockというメモアプリがシンプルで使いやすいです。  
クラウドに保存されるので、どこからでも参照できますし、PCに万が一のことがあっても安心です。  　
https://www.stock-app.jp/

## リモート操作ソフト
案件では、提供したプログラムが想定道理動作しない等の場合に  
リモートで対応するのが早い場合も多いです。  
TeamViewerというツールが有名なので、インストールしておくと良いでしょう。  
お客側にも同じくツールをインストールしてもらい、ID/PASSを共有してもらうことで  
リモート可能なります。ファイルの転送も可能です。

## 画面キャプチャ、動画を共有したい場合
Gyazoというツールが非常に優秀です。キャプチャした画像、動画が自動的にクラウドにアップされるので  
そのURLを共有するだけで、画面の共有が可能です。  
https://gyazo.com/



