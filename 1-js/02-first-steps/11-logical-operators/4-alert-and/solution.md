答え: `1`, 次に `undefined`。

```js run
alert( alert(1) && alert(2) );
```

`alert` の呼び出しは `undefined` を返します(メッセージを表示するだけなので、意味のある返却はありません)。

そのため、 `&&` が左のオペランドを検査(`1` を出力)し、すぐに停止します。なぜなら、`undefined` は偽値だからです。そして `&&` は偽値を探し、それを返します。
