# adash.ahk

A modern utility library for AutoHotkey v2. Inspired by [Lodash](https://lodash.com/), with zero dependencies.

[Browse the docs](/) · [Getting started](/en/getting-started) · [Download](/en/download) · [GitHub](https://github.com/adash-ahk/adash.ahk)

## Why adash?

Everyday scripting is full of small data chores: looping over arrays, reshaping objects, cleaning up strings. adash.ahk replaces that boilerplate with short, predictable methods so you can spend your time on the actual problem.

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

## What you get

- **300+ methods** for arrays, collections, objects, strings, math, numbers, functions, and more, documented with examples and covered by tests.
- **Immutable by default.** Methods return new values and leave your input untouched. The few exceptions, such as `.fill` and `.pull`, say so in their docs.
- **Zero dependencies.** Include one file and you're done.
- **Fast when you need it.** Set `_.throwExceptions := false` to skip type checking entirely.
- **Clear errors.** With `_.throwExceptions := true` (the default), a wrong argument type tells you what was expected and what was received.
- **Use only what you need.** Every method stands alone, so your scripts stay small and readable.

## Where to next

- **New here?** Start with [Getting Started](/en/getting-started).
- **Looking for a method?** Search the [documentation](/).
- **What's new?** Read the [news and release notes](/en/news).
- **Want to help?** Report issues or send pull requests on [GitHub](https://github.com/adash-ahk/adash.ahk), or [donate](/en/donate) to support development.

<br>

Released under the [MIT license](https://opensource.org/licenses/MIT).
