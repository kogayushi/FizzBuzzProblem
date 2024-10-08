# FizzBuzz問題のリファクタリング問題

## FizzBuzz問題についての説明
整数値を入力として受け取り、以下のルールに従って結果を出力するプログラムを作成した。

1. 数が3で割り切れる場合は、数の代わりに”Fizz”と出力する。
2. 数が5で割り切れる場合は、数の代わりに”Buzz”と出力する。
3. 数が3と5両方で割り切れる場合は、数の代わりに”FizzBuzz”と出力する。
4. 上記の条件に該当しない場合は、入力された数をそのまま出力する。

## FizzBuzz問題のリファクタリング問題
FizzBuzz問題の要件を満たすFizzBuzzEngineクラスを実装したが、7で割り切れるときは数の代わりに"Foo"と出力する要件が追加されることが決定した。また、今後も任意の素数に応じた文字列を返す要件が複数追加される可能性がある。

Open Closed Principleを適用し、拡張に対しては開かれているが、修正に対しては閉じている設計にFizzBuzzEngineクラスをリファクタリングしなさい。FizzBuzzEngineクラスの振る舞いをインターフェースや抽象クラスを通して柔軟に拡張可能にすることが求められています。
