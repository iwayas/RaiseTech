- サンプルアプリケーションを今日見せた作業と同じように起動（デプロイ）してみましょう。起動できたら、ブラウザでアクセスしてみましょう。
<img width="1440" alt="lecture03" src="https://github.com/iwayas/RaiseTech/assets/66251668/dc5262a4-3d38-47b0-b00e-f287e1ca3a8b">

- AP サーバーについて調べてみましょう。
APサーバ（アプリケーションサーバ）とは、Web3層構造と呼ばれるWebシステムで、アプリケーションプログラムを動作させるサーバのことです。APサーバはWebアプリケーションサーバとも呼ばれています。

- AP サーバーの名前とバージョンを確認してみましょう。
$ puma --ver で確認。
puma version 5.6.5

- AP サーバーを終了させた場合、引き続きアクセスできますか？結果を確認して、また AP サーバーを起動してください。
$ bundle exec pumactl halt で停止。
アクセスできず、下記エラーが表示される。
Oops No application seems to be running here!
$ rails s で再度起動し、アクセス出来たことを確認。

- DB サーバーについて調べてみましょう。
DBサーバ（データベースサーバ）とは、データを一元管理し、データの検索、更新、保存、バックアップを行うサーバのことです。Web3層構造のWebシステムでは最下層に位置し、APサーバからの要求に基づきデータの検索やデータの更新（追加、修正、削除）を行っています。

- サンプルアプリケーションで使った DB サーバー（DB エンジン）の名前と、今 Cloud9 で動作しているバージョンはいくつか確認してみましょう。
$ mysql --version で確認。
mysql Ver 8.0.34 for Linux on x86_64 (MySQL Community Server - GPL)

- DB サーバーを終了させた場合、引き続きアクセスできますか？
$ sudo service mysqld stop で終了。下記エラーが表示され、アクセス不可となった。
Can't connect to local MySQL server through socket '/var/lib/mysql/mysql.sock' (2)

- Rails の構成管理ツールの名前は何でしたか？確認してみてください。
Bundler version 2.3.14

- 今回の課題から学んだことを報告してください。
Web3層構造についての理解が深まり、それぞれの役割の違いや関連性を知ることができました。
