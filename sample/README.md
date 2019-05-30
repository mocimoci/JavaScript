# １ページ完結のminiコード

## 簡単な計算をする
*dentaku.html*

### DOM（document Object Model）
JavaScriptからHTMLの各要素を操作するための仕組み  
（document.bodyで、HTMLファイルのbodyタグの中身を取得、とか）
  
### 変数
値を一時的に格納する入れ物  

`var src = $("#srcArea").val();`  

「var」→「variable(変数)」の意味。「src」という変数を作る。  
「=」→右の値を、左の変数に入れる。　
  
`var res = eval(src);`  

eval() は文字列として表された JavaScript コードを式として評価する関数。  
()の中の文字を、プログラムとして解釈。計算式を入れれば計算してくれる。  

`$("#resArea").val(res);`  

変数「res」に格納されている値をテキストエリアに出力。  

| 説明 | コード |
|:-----------|:------------|
| フォームから値を取得 | $(セレクタ).val() |
| フォームに値を出力 | $(セレクタ).val(値) |
| DOMからHTMLを取得 | $(セレクタ).html() |
| DOMにHTMLを出力 | $(セレクタ).html(値) |
| DOMからテキストを取得 | $(セレクタ).text() |
| DOMにテキストを出力 | $(セレクタ).text(値) |

## 文字数をカウントする
*count.html*

`var res = src.length;`  

文字列の長さを取得

