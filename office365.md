# office365

- Microsoft Graph API
    - https://developer.microsoft.com/ja-jp/graph
    - 代表窓口。トップページ。あまり情報はない。
- Microsoft Graph API を使用する
    - https://developer.microsoft.com/ja-jp/graph/docs/concepts/use_the_api
    - URL形式、GET/POSTなどの説明
- Graph エクスプローラー
    - https://developer.microsoft.com/ja-JP/graph/graph-explorer
    - Graph API を試せる
    - デモユーザでのアクセスは可能。
    - 自分のIDでアクセスしようとすると「管理者の承認が必要」と言われてしまった。
- Microsoft Graph のクイック スタート
    - https://developer.microsoft.com/ja-JP/graph/quick-start
    - すぐに、プログラミング言語を選択するメニューになり、Pythonを選択する。
- Python アプリで Microsoft Graph を使ってみる
    - https://developer.microsoft.com/ja-jp/graph/docs/concepts/python
    - 認証ライブラリの選択:Microsoft Graph を呼び出すには、Microsoft クラウドの ID サービスである Azure Active Directory (Azure AD) から有効なアクセス トークンをアプリが取得し、そのトークンが Microsoft Graph REST API に対する各呼び出しの HTTP ヘッダーに渡される必要があります
    - とあり、ここで管理者IDが必要な気がする

- Microsoft Graph を呼び出すためのトークンの取得
    - https://developer.microsoft.com/ja-jp/graph/docs/concepts/auth_overview
    - Microsoft Graph を呼び出すために、アプリは Microsoft のクラウド ID サービス Azure Active Directory (Azure AD) からアクセス トークンを取得する必要があります。アクセス トークンには、アプリとアプリに付与されているアクセス許可に関する情報 (要求) が含まれています (このアクセス許可は、Microsoft Graph を通じて利用できるリソースと API に対応するものです)。アクセス トークンを取得するためには、アプリを Azure AD で認証できるようにすることと、そのアプリが必要とする Microsoft Graph リソースへのアクセスをユーザーまたは管理者が承認することが必要です。
    - まずは、認証を通過しないと、アクセスできないので、とても重要。
    - でも、書いていることが、よくわからん。。。
    - 結局、ユーザの権限でどこまでできるのか、管理者権限がどこから必要なのか。。。

- MICROSOFT GRAPH (UNIFIED API) を使いこなそう
    - https://tsmatz.wordpress.com/2015/06/22/office-365-unified-api/
    - 文章はわかりやすいが、認証関係は、さらっと触れているだけ。
        - Microsoft Graph の使い方：使い方は、いままでと同じです。OAuth Flow で access token を取得し、取得した access token を HTTP Header に付与して https://graph.microsoft.com に HTTP Request を投げるだけです。

- Microsoft GraphでOAuthのアクセストークンを更新する仕組みを作る
    - https://qiita.com/takuya-andou/items/3df23aeb77a79b15c9f8
    - 「5.起動確認」までは進んだが、「Connect to Microsoft Graph」のボタンを押すと、個人の認証のID選択、グロコミID/Passwdでの認証の後、「Need admin approval」と
言われてしまった。やはり、組織の管理者権限が必要なようだ。



- Office 365 API リファレンス
    - https://msdn.microsoft.com/ja-jp/office/office365/howto/rest-api-overview
- Outlook のメール、予定表、および連絡先を取得する Python アプリの記述
    - https://docs.microsoft.com/ja-jp/outlook/rest/python-tutorial




