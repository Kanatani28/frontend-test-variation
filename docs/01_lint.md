# ESLint
基本的にはお好みで良いと思う。  
自分はファイル形式はymlにし、いくつか標準のものに加えて追加している。

各種雛形を作成するコマンドで標準的なものはインストールされるがお好みでカスタマイズするのが良い。  
とはいえ凝りだすと終わらないので公開されているものをベースにちょい足しするような感じにしている。

- extendsとか多用すると設定が重複しているものも多く見かけるのでこの辺の手法でチェックしながら少しずつ追加するのがよいと思う。  
https://zenn.dev/nananaoto/articles/9968d8f3966e90a46229


- Next.jsの場合は割と事前に設定してくれている.   
https://nextjs.org/docs/basic-features/eslint


## 個人的によくちょい足しするもの

- `eslint:recommended` 
  - とりあえず入れている   
    https://www.tam-tam.co.jp/tipsnote/javascript/post11934.html

- `@typescript-eslint` `@typescript-eslint/parser` 
  - TS使うならとりあえず入れておく

- Prettier
  - 必須級。huskyとも相性がいい
  ```
  yarn add --dev prettier eslint-config-prettier
  ```
  参考: https://yoshitaku-jp.hatenablog.com/entry/2019/02/03/220000

- `eslint-plugin-simple-import-sort`
  - import文のソートが気になる人は設定するのがいい
  https://github.com/lydell/eslint-plugin-simple-import-sort

- `eslint-plugin-jest`
  - Jestでテスト書く場合は入れておく

## その他
- env: esXXXX はとりあえず新しいものを設定している
- eslintignoreはいい感じに設定しておく。特に*.config.jsは設定した方がいい

## 参考
https://zenn.dev/januswel/articles/402774d76424e71ac906

各種設定の意味
https://maku.blog/p/j6iu7it/







