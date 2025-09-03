# SQL実行手順

データベース接続ツール「A5:SQL Mk-2」の基本的な使い方を記載しています。

## データベース接続ツールのセットアップ

1. **ダウンロードと解凍**  
   A5:SQL Mk-2のサイトから、x64 editionのzipファイルをダウンロードおよび解凍を行う。  
   [公式サイト](https://a5m2.mmatsubara.com/)

2. **初回起動と設定**  
   A5M2.exeを起動し、以下の設定を行い、起動ボタンを選択する：
   - ワークスペース情報の保存: **設定ファイル(ポータブルモード)**
   - 起動時に表示する: **Off**

   ![初回設定画面](https://raw.githubusercontent.com/atoji0/outsystem_dev/main/wiki/image/SQL実行手順/image.png)

3. **データベースの追加**  
   初回起動時、2回ほど確認ダイアログが表示されるため、OKボタンを選択する。その後、データベースの追加と削除が開かれるので、**追加ボタン**を選択し、**Oracle Database**を選択する。  
   ※初回起動以降は、メニューから[データベース] - [データベースの追加と削除]で設定可能。

   ![データベース追加画面1](https://raw.githubusercontent.com/atoji0/outsystem_dev/main/wiki/image/SQL実行手順/image-1.png)  
   ![データベース追加画面2](https://raw.githubusercontent.com/atoji0/outsystem_dev/main/wiki/image/SQL実行手順/image-2.png)

4. **接続情報の入力**  
   代理認証ID申請書に記載されている以下の情報を入力する：
   - ホスト名
   - サービス名
   - ポート番号
   - ユーザID
   - パスワード  

   テスト接続を実施後、OKボタンを選択する。その後、データベース別名を指定し、OKボタンを選択する。

   ![接続情報入力画面1](https://raw.githubusercontent.com/atoji0/outsystem_dev/main/wiki/image/SQL実行手順/image-3.png)  
   ![接続情報入力画面2](https://raw.githubusercontent.com/atoji0/outsystem_dev/main/wiki/image/SQL実行手順/image-4.png)

## SQL実行手順

1. **データベースに接続する**  
   左側に出てくるデータベースツリーから接続するDBを選択し、ユーザーIDとパスワードを入力して接続する。

   ![データベース接続画面](https://raw.githubusercontent.com/atoji0/outsystem_dev/main/wiki/image/SQL実行手順/image-5.png)

2. **SQL実行オプションを設定する**  
   SQL実行オプションを開き、以下の設定を行う：
   - **実行位置**: 先頭から全て
   - **SQL区切り文字**: ";"

   ![SQL実行オプション設定画面](https://raw.githubusercontent.com/atoji0/outsystem_dev/main/wiki/image/SQL実行手順/image-6.png)

3. **SQLを記述して実行する**  
   赤枠部分にSQLを記述する。SQL文の先頭にカーソルを置き、`Ctrl + Enter`で記載した全てのSQLを実行する。

   ![SQL記述と実行画面](https://raw.githubusercontent.com/atoji0/outsystem_dev/main/wiki/image/SQL実行手順/image-7.png)
