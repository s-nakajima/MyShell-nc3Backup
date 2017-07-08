# バックアップシェル

## s-nakajima/MyShellへの追加方法

MyShell/composer.jsonに下記を追加
~~~~
"repositories": [
    {"type": "vcs", "url": "https://github.com/s-nakajima/MyShell-nc3Backup.git"}
],
~~~~

下記のコマンドを実行
~~~~
cd /var/www/MyShell
composer require s-nakajima/nc3-backup:@dev
~~~~


## nc3Backup
（ダウンロードしたシェルは中身を見てね）

※tar.gzでローカルにバックアップします。

<pre>
cd /var/www/MyShell/nc3Backup
bash nc3Backup.sh
</pre>

<pre>
cd /var/www/MyShell/nc3Backup
bash nc3Backup.sh all
</pre>


| 引数           | 説明                                  |
| -------------- | ------------------------------------- |
| all            | /var/www/app全てとデータベース(nc3というDB名)をバックアップする |
| なし           | /var/www/app/app/Pluginと/var/www/app/app/Config、データベース(nc3というDB名)のみバックアップする |

