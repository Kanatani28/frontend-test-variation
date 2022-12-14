# ESLint

基本的にはお好みで良いと思う。  
自分はファイル形式は yml にし、いくつか標準のものに加えて追加している。

各種雛形を作成するコマンドで標準的なものはインストールされるがお好みでカスタマイズするのが良い。  
とはいえ凝りだすと終わらないので公開されているものをベースにちょい足しするような感じにしている。

- extends とか多用すると設定が重複しているものも多く見かけるのでこの辺の手法でチェックしながら少しずつ追加するのがよいと思う。  
  https://zenn.dev/nananaoto/articles/9968d8f3966e90a46229

- Next.js の場合は割と事前に設定してくれている.  
  https://nextjs.org/docs/basic-features/eslint

## 個人的によくちょい足しするもの

- `eslint:recommended`

  - とりあえず入れている  
    https://www.tam-tam.co.jp/tipsnote/javascript/post11934.html

- `@typescript-eslint` `@typescript-eslint/parser`

  - TS 使うならとりあえず入れておく

- Prettier

  - 必須級。husky とも相性がいい

  ```
  yarn add --dev prettier eslint-config-prettier
  ```

  参考: https://yoshitaku-jp.hatenablog.com/entry/2019/02/03/220000

- `eslint-plugin-simple-import-sort`

  - import 文のソートが気になる人は設定するのがいい
    https://github.com/lydell/eslint-plugin-simple-import-sort

- `eslint-plugin-jest`
  - Jest でテスト書く場合は入れておく

## その他

- env: esXXXX はとりあえず新しいものを設定している
- eslintignore はいい感じに設定しておく。特に\*.config.js は設定した方がいい
- lintとはちょっと違うけどtsconfigもお好みで設定しておく。
  - [この辺の設定](https://github.com/Kanatani28/frontend-test-variation/commit/aa992e5361d1f522a5eba8918f2e28aa3104584e#diff-b55cdbef4907b7045f32cc5360d48d262cca5f94062e353089f189f4460039e0R21-R24)あたりはしておくと`import`する際に`../../../`みたいなの書かなくて済む。

## 参考

https://zenn.dev/januswel/articles/402774d76424e71ac906

各種設定の意味
https://maku.blog/p/j6iu7it/
