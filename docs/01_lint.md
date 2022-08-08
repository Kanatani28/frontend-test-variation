# ESLint
基本的にはお好みで良いと思う。
自分はyml形式でいくつか標準のものに加えて追加する。

各種雛形を作成するコマンドで標準的なものはインストールされるがお好みでカスタマイズするのが良い。
とはいえ凝りだすと終わらないので公開されているものをベースにするのが良い。

extendsとか多用すると設定が重複しているものも多く見かけるのでこの辺の手法でチェックしながら少しずつ追加するとよい
https://zenn.dev/nananaoto/articles/9968d8f3966e90a46229

参考
https://zenn.dev/januswel/articles/402774d76424e71ac906

Next.jsの場合は割と事前に設定してくれている
https://nextjs.org/docs/basic-features/eslint

各種設定の意味
https://maku.blog/p/j6iu7it/

これ以外で有効にしても良さそうなもの

- eslint:recommended
https://www.tam-tam.co.jp/tipsnote/javascript/post11934.html

@typescript-eslint/parser
デフォルトはJavaScriptベースなので入れておくのが良さそう

Prettier

必須級

```
yarn add --dev eslint-config-prettier
```

eslint-plugin-simple-import-sort
https://github.com/lydell/eslint-plugin-simple-import-sort



eslint-plugin-jest


esXXXX とりあえず新しいものを