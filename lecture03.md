- サンプルアプリケーションを今日見せた作業と同じように起動（デプロイ）してみましょう。起動できたら、ブラウザでアクセスしてみましょう。
<img src="https://github.com/iwayas/RaiseTech/blob/lecture03/lecture03-1.png">

- AP サーバーについて調べてみましょう。
<br> APサーバ（アプリケーションサーバ）とは、Web3層構造と呼ばれるWebシステムで、アプリケーションプログラムを動作させるサーバのことです。APサーバはWebアプリケーションサーバとも呼ばれています。

- AP サーバーの名前とバージョンを確認してみましょう。
<br> $ puma --ver で確認。
<br> puma version 5.6.5
<img src="https://github.com/iwayas/RaiseTech/blob/main/lecture03-3.png">

- AP サーバーを終了させた場合、引き続きアクセスできますか？結果を確認して、また AP サーバーを起動してください。
<br> $ bundle exec pumactl halt で停止。
<img src="https://github.com/iwayas/RaiseTech/blob/main/lecture03-4.png">
<br> アクセスできず、下記エラーが表示される。
<br> Oops No application seems to be running here!
<img src="https://github.com/iwayas/RaiseTech/blob/main/lecture03-5.png">
<br> $ rails s で再度起動し、アクセス出来たことを確認。

- DB サーバーについて調べてみましょう。
<br> DBサーバ（データベースサーバ）とは、データを一元管理し、データの検索、更新、保存、バックアップを行うサーバのことです。Web3層構造のWebシステムでは最下層に位置し、APサーバからの要求に基づきデータの検索やデータの更新（追加、修正、削除）を行っています。

- サンプルアプリケーションで使った DB サーバー（DB エンジン）の名前と、今 Cloud9 で動作しているバージョンはいくつか確認してみましょう。
<br> $ mysql --version で確認。
<br> mysql Ver 8.0.34 for Linux on x86_64 (MySQL Community Server - GPL)
<img src="https://github.com/iwayas/RaiseTech/blob/main/lecture03-6.png">

- DB サーバーを終了させた場合、引き続きアクセスできますか？
<br> $ sudo service mysqld stop で終了。下記エラーが表示され、アクセス不可となった。
<br> Can't connect to local MySQL server through socket '/var/lib/mysql/mysql.sock' (2)
<img src="https://github.com/iwayas/RaiseTech/blob/main/lecture03-7.png">
<img src="https://github.com/iwayas/RaiseTech/blob/lecture03/lecture03-2.png">

- Rails の構成管理ツールの名前は何でしたか？確認してみてください。
<br> Bundler version 2.3.14
<img src="https://github.com/iwayas/RaiseTech/blob/main/lecture03-8.png">

- 今回の課題から学んだことを報告してください。
<br> Web3層構造についての理解が深まり、それぞれの役割の違いや関連性を知ることができました。
