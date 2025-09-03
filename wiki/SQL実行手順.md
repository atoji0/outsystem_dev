# SQL実行手順

データベース接続ツール「A5:SQL Mk-2」の基本的な使い方を記載しています。

## データベース接続ツールのセットアップ

1. A5:SQL Mk-2のサイトから、x64 editionのzipファイルをダウンロードおよび解凍を行う。
　https://a5m2.mmatsubara.com/

2. A5M2.exeを起動すると、最初の画面で以下の設定を行い、起動ボタンを選択する。
   - ワークスペース情報の保存 : 設定ファイル(ポータブルモード)
   - 起動時に表示する ： Off

![alt text](https://raw.githubusercontent.com/atoji0/outsystem_dev/main/wiki/image/SQL実行手順/image.png?TOKEN=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)

3. 2回ほど確認ダイアログが表示されるため、OKボタンを選択する。その後、データベースの追加と削除が開かれるので、追加ボタンを選択し、Oracle Databaseを選択する。
※初回起動以降は、メニューから[データベース]-[データベースの追加と削除]で設定可能。

![alt text](https://raw.githubusercontent.com/atoji0/outsystem_dev/main/wiki/image/SQL実行手順/image-1.png?TOKEN=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)

![alt text](https://raw.githubusercontent.com/atoji0/outsystem_dev/main/wiki/image/SQL実行手順/image-2.png?TOKEN=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)

4. 代理認証ID申請書に記載されているホスト名、サービス名、ポート番号、ユーザID、パスワードを入力し、テスト接続を実施後、OKボタンを選択する。その後、データベース別名を指定し、OKボタンを選択する。

![alt text](https://raw.githubusercontent.com/atoji0/outsystem_dev/main/wiki/image/SQL実行手順/image-3.png?TOKEN=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)

![alt text](https://raw.githubusercontent.com/atoji0/outsystem_dev/main/wiki/image/SQL実行手順/image-4.png?TOKEN=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)

## SQL実行手順

1. 左側に出てくるデータベースツリーから接続するDBを選択し、ユーザーIDとパスワードを入力て接続する。

![alt text](https://raw.githubusercontent.com/atoji0/outsystem_dev/main/wiki/image/SQL実行手順/image-5.png?TOKEN=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)

2. SQL実行オプションを開き、「実行位置＝先頭から全て」　「SQL区切り文字＝";"」を選択する。

![alt text](https://raw.githubusercontent.com/atoji0/outsystem_dev/main/wiki/image/SQL実行手順/image-6.png?TOKEN=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)

3. 赤枠部分にSQLを記入し、先頭にカーソルを置き、[Ctrl]-[Enter]で記載した全てのSQLを実行する。

![alt text](https://raw.githubusercontent.com/atoji0/outsystem_dev/main/wiki/image/SQL実行手順/image-7.png?TOKEN=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)