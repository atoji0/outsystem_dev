# Extension作成

OutSystemsにて、Oracle DBに接続し、Entityを作成する。

1. Service StudioからExtensionを作成し、Integration Studioを起動する。その際、モジュール名は「アプリコード(3桁)_アプリ略称_DB」とする。

![alt text](https://raw.githubusercontent.com/atoji0/outsystem_dev/main/wiki/image/Extension作成/image.png)

2. ログイン画面が表示されるので、対象サーバー名、ユーザー名、パスワードを入力する。

![alt text](https://raw.githubusercontent.com/atoji0/outsystem_dev/main/wiki/image/Extension作成/image-1.png)

3. ツリーメニューの「Extension - Entities」を右クリックし、「Connect to External Table or View…」を選択する。

![alt text](https://raw.githubusercontent.com/atoji0/outsystem_dev/main/wiki/image/Extension作成/image-2.png)

4. ウィザードの内容に従い、対象となるDatabase Connection、Database Name、Table Nameを選択する。

![alt text](https://raw.githubusercontent.com/atoji0/outsystem_dev/main/wiki/image/Extension作成/image-3.png)
![alt text](https://raw.githubusercontent.com/atoji0/outsystem_dev/main/wiki/image/Extension作成/image-4.png)
![alt text](https://raw.githubusercontent.com/atoji0/outsystem_dev/main/wiki/image/Extension作成/image-5.png)
![alt text](https://raw.githubusercontent.com/atoji0/outsystem_dev/main/wiki/image/Extension作成/image-6.png)

5. OutSystemsで利用する際に表示される外部データベース名が表示され、登録が完了となる。

![alt text](https://raw.githubusercontent.com/atoji0/outsystem_dev/main/wiki/image/Extension作成/image-7.png)
![alt text](https://raw.githubusercontent.com/atoji0/outsystem_dev/main/wiki/image/Extension作成/image-8.png)

6. 以下のルールに従い、Entityの修正を行う。

   - サロゲートキーは「Text型」から「Long Integer型」に変更し、「Auto Generated」にチェックを付ける。
   - Table or View Default Nameのスキーマ名を削除し、オブジェクト名称のみとする。

7. 「1-Click Publish」を実行し、デプロイを行う。

　　- FileメニューからVerify and Save、もしくは[F4]を選択し、エラーがないか確認する。
　　- その後、Save→Publish→Configureの順で実行していく。Configureを押すと、Sevice Centerが起動する。
