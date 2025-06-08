## 外部APIの呼び出しのミニレポート
### Q3-1. 郵便番号APIについて説明せよ。
* エンドポイントと機能
  * https://zipcloud.ibsnet.co.jp/api/search
  * ユーザが入力した郵便番号に対応した住所を表示する
* リクエストとレスポンスのフォーマット
  * "?zipcode=" + document.getElementsByName("zipcode")[0].value
  * 例) { "message": null, "results": [...], "status": 200 }
### Q3-2. 各自で調査したAPIについて説明せよ。
* APIの名称と参照URL
  * httpbin
  * https://httpbin.org/
* エンドポイントと機能
  * https://httpbin.org/
  * httpのテストを行うことができる
* リクエストとレスポンスのフォーマット
  * document.getElementsByName("form_data")[0].value  // ユーザが入力した内容をURLに送るのみ
  * JSONやHTMLなど、リクエストに対応したレスポンスのフォーマットが返ってくる
### Q3-3. 感想
* 今回の課題で苦労したこと
  * リクエストの処理に苦労した
* 演習を通して理解できたこと
  * Fetch APIの使い方を理解できた
* Web APIの利便性や課題など
  * 低コストで開発しやすい反面、外部サービスへの依存度が高い
  * 非同期処理が行える反面、コールバック地獄にならないよう気を付ける必要がある
