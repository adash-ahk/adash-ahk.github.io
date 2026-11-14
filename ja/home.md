# adash.ahk

AutoHotkey v2 向けのモダンなユーティリティライブラリ。[Lodash](https://lodash.com/) にインスパイアされ、依存関係はゼロです。

[ドキュメント](/ja/docs) · [はじめに](/ja/getting-started) · [ダウンロード](/ja/download) · [GitHub](https://github.com/adash-ahk/adash.ahk)

## なぜ adash?

日々のスクリプト作成には、配列のループ、オブジェクトの整形、文字列の整理といった細かなデータ処理がつきものです。adash.ahk は、そうした定型コードを短く予測しやすいメソッドに置き換え、本来の課題に集中できるようにします。

```autohotkey
#Include <adash.ahk>
_ := adash

_.chunk(["a", "b", "c", "d"], 2)
; => [["a", "b"], ["c", "d"]]

users := [{name: "tank", age: 40}, {name: "cypher", age: 34}]
_.sortBy(users, "age")
; => [{name: "cypher", age: 34}, {name: "tank", age: 40}]

_.kebabCase("fooBar")
; => "foo-bar"
```

## 特長

- **300 以上のメソッド**: 配列、コレクション、オブジェクト、文字列、数値、関数などに対応。すべて例付きでドキュメント化され、テストで検証されています。
- **既定でイミュータブル**: メソッドは新しい値を返し、入力は変更しません。`.fill` や `.pull` など一部の例外は、ドキュメントに明記されています。
- **依存関係ゼロ**: 1 つのファイルを読み込むだけです。
- **必要なときは高速**: `_.throwExceptions := false` を設定すると、型チェックを完全にスキップします。
- **わかりやすいエラー**: `_.throwExceptions := true` (既定) では、引数の型が違うと、期待された型と実際の型が示されます。
- **必要なものだけ使える**: 各メソッドは独立しているため、スクリプトは小さく読みやすいままです。

## 次のステップ

- **初めての方**: [はじめに](/ja/getting-started)をご覧ください。
- **メソッドを探す**: [ドキュメント](/ja/docs)を検索してください。
- **最新情報**: [ニュースとリリースノート](/ja/news)をご覧ください。
- **協力したい方**: [GitHub](https://github.com/adash-ahk/adash.ahk) で issue や pull request を送るか、[寄付](/ja/donate)で開発を支援してください。

<br>

[MIT ライセンス](https://opensource.org/licenses/MIT)のもとで公開されています。
