## htmxについて
htmx は、JavaScript を使用せずに HTML から直接最新のブラウザ機能にアクセスできるようにする library です。
Javascript書くのが面倒だけどAJAX通信などを行いたいときに使えます。


## 使用している主な技術
<img src="https://img.shields.io/badge/-Htmx-D3DC43.svg?logo=htmx&style=flat"> <img src="https://img.shields.io/badge/Javascript-276DC3.svg?logo=javascript&style=flat">

## ドキュメント
日本語のドキュメントです。
https://runebook.dev/ja/docs/htmx/-index-

| 機能                   | HTMX                                     | Fetch API (JavaScript)                               |
|----------------------|------------------------------------------|------------------------------------------------------|
| **リクエスト送信**       | `hx-get="URL"`                           | `fetch(URL)`                                         |
| **HTTPメソッド指定**     | `hx-post="URL"`                          | `fetch(URL, { method: 'POST' })`                     |
| **イベントトリガー**     | `hx-trigger="event"`                     | イベントリスナー内でFetchを呼び出す: `element.addEventListener('event', () => fetch(URL))` |
| **拡張機能有効化**      | `hx-ext="extension"`                     | N/A（Fetch APIには直接的な拡張機能の概念はない）         |
| **テンプレート利用**     | `<script type="text/mustache-template">` | テンプレートリテラルまたはライブラリを使用                 |
| **パラメータ追加**      | `hx-params="foo=bar"`                    | `fetch(URL, { method: 'GET', body: 'foo=bar' })`    |
| **レスポンス処理**      | HTML属性による自動処理                    | `.then(response => response.json()).then(data => { /* 処理 */ })` |
| **ヘッダー追加**        | `hx-headers='{"Header":"Value"}'`        | `fetch(URL, { headers: { 'Header': 'Value' } })`    |
| **エラーハンドリング**   | HTMXイベント (`htmx:afterRequest` など)  | `.catch(error => { /* エラー処理 */ })`              |



## 準備
1. ```https://github.com/ShuyaOda/modernfront```　を開き Codeを押下しDownloadZipを押下する

![image](https://github.com/ShuyaOda/modernfront/assets/159111947/84973820-a94c-4387-ac2c-81fee0b96cdb)

2. 解凍して任意の場所に張り付ける(デスクトップに張り付けてます)

![image](https://github.com/ShuyaOda/modernfront/assets/159111947/e3c81fcd-68b8-419c-bfe3-e9f20f373cbe)

3. modernfront-htmxファイルを右クリックし、その他のオプション→Codeで開くを押下し下記の画面になれば準備OKです。

![image](https://github.com/ShuyaOda/modernfront/assets/159111947/cb811b22-bd58-425c-8d73-a36268daaafe)





## 使い方
- ファイルを右クリックしてフルパスでコピーして適当なブラウザーに張り付ければ見れます。(例ではGoogle Chrome)
![image](https://github.com/ShuyaOda/modernfront/assets/159111947/98491c73-3ee8-4c8c-a649-4d9021e8ede7)

※ vscodeで修正した場合、画面を更新すると反映されます。





