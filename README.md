# 第５回特別課題
## URLとは
「Uniform Resource Locator」の略で、 **ホームページの「住所」に相当する情報** のこと。    

例）`https://github.com/momokoshinkawa/kadai5/edit/main/README.md`  

スキーム名:  `https://`  
ホスト名、サブドメイン名:  `github.com`  
ドメイン名:  `github.com`  
ファイルまでのパス:  `/momokoshinkawa/kadai5/edit/main/README.md`  
ファイル名:  `README.md`   

## クエリ文字列とは
 **ウェブページのURLに追加情報やパラメータを伝えるための文字列** のこと。  
 ※パラメータ：外から渡す値
 
例　`https://example.com/search **?q=programming&category=web**`  

- 検索エンジンの検索結果ページではユーザーが検索したクエリ文字列がURLに含まれ、  
これによりサーバーはクエリ文字列を解析し適切な検索結果を返すことができる。  
- 「?」 以降の部分がクエリ文字列。    
- 「＆」 で繋げることで複数のパラメーターを設定することができる。
  
## パス変数（パスパラメーター）とは
URLのパスの一部として **特定のリソースを識別するために必要な情報を表すもの** 。 

例）`http://example.com/user/1`  
- 上記URLにおける「1」の部分。  
- よくあるのがユーザーIDとか記事IDなど。   
- 世の中の様々なサービスでパスパラメータを指定することで特定のユーザーの情報だったり、   
記事の情報だったりを表示するために活用されている。  

## クエリ文字列とパス変数の違いとは
|クエリ文字列 |パス変数　|
|---|---|
|・URLの末尾に追加され、疑問符文字（? ）で始まる。<br> ・GETリクエスト時に主に利用。<br> ・サーバーに対して追加の情報を渡し、絞り込みなどに利用する。　| ・URLのパス自体に情報を組み込むために使用され、<br>セミコロン文字（; ）で始まる。<br> ・ユーザーIDなど一意のリソースやアクションを表現するのに適している。 |

## HTTPメソッドとは
HTTPリクエストをする際に、 **通信のやり取りの要求を定義したもの** 。  

代表的なメソッド↓  

|メソッド名 |説明 |
|:---:|---|
|GET |ウェブサーバーからデータを取得する |
|POST |リソースの更新または新規作成を行う |
|PUT |既存リソースの全置換 |
|PATCH |リソースの部分的な更新を行うために使用  |
|DELETE |ウェブ上のデータを永続的に削除するための手段 |  

## リクエストヘッダーとは  

- HTTPリクエストの部品で **『お願いごとやお願い元に関するあれこれ』が書かれている**部分。    
- リクエストに関連する追加情報やメタデータを含む。
  
![image](https://github.com/momokoshinkawa/kadai5/assets/146909506/c70b170c-2994-4ab2-81d5-aa1b63175493)  
[参考](https://wa3.i-3-i.info/index.html)  


## レスポンスヘッダーとは

- HTTPレスポンス(HTTPリクエストに対する返答)の部品で **『ステータスラインに書ききれないレスポンスの情報』が書かれている**部分。   
- Webサーバーのソフトウェア情報、返信するデータの種類、データ圧縮方法などの情報を含む。    

![image](https://github.com/momokoshinkawa/kadai5/assets/146909506/d5399390-ecf6-4fa0-8fda-c20ebe2ffaef)　　
![image](https://github.com/momokoshinkawa/kadai5/assets/146909506/257315cd-31e4-4d43-890d-9d91940f6498)

[参考](https://wa3.i-3-i.info/index.html)  
[参考](2021)  

## レスポンスボディとは

- HTTPレスポンス(HTTPリクエストに対する返答)の部品で **『相手が欲しがってたファイルの中身』が書いてある**部分。   
- HTMLや画像などのデータを格納する。  


## HTTPステータスコードとは

上記で説明した **HTTPレスポンスのステータス行に結果として表示される３桁のコード**。  

|ステータスコード　|意味 |
|:---:|---|
|200 |OK　リクエスト成功  |
|201 |Created　リソースの作成成功   |
|400 |Bad Request　リクエストの構文やパラメータに間違いがある  |
|404 |Not Found　指定したリソースが見つからない   |
|500 |nternal Server Error　サーバ側に何らかの異常  |

## JSONとは

- 「JavaScript Object Notation」の略で、ファイルの書き方ルールのひとつ。
- JavaScriptと相性が良い。  
- Web開発、API通信、データ交換、設定ファイル、ログファイル、データベースのクエリ結果など、多くのコンテキストで使用されている。

具体例
```JSON
{
  "name": "Momoko Shinkawa",
  "age": 30,
  "city": "Osaka",
  "isStudent": false,
  "hobbies": ["Watching Movies", "Golf", "Eating"]
}
```





