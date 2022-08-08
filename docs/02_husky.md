# husky

コミット時に ESLint が走るようにしておくと各自のエディタや開発環境に依存せずフォーマットがかけられて良い。
単体テストを実行するようなことも可能だが、ボリュームが大きくなるにつれてコミットに時間がかかるようになるので
そこは CI で対応しても良いと個人的には思っている。

## Install

```
yarn add -D husky lint-staged
npx husky-init
yarn prepare
```

参考
https://zenn.dev/seya/articles/c908d88df0a587
https://qiita.com/miruon/items/fc344ea0a489cf9252d5
