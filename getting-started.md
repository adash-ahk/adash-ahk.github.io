## Installation

In your code only the file adash.ahk needs to be included:

```autohotkey
#Include <adash.ahk>

_ := adash
msgbox(_.join(["a", "b", "c"], " "))
; => "a b c"
```

### Properties

By default the following properties are as follows:

`_.throwExceptions := true`
Wherever typeif errors can be detected, adash.ahk will throw an exception pointing out the location the error occurred. Set this to `false` if you would like your script to continue without being stopped by exceptions.

`_.stringCaseSense := false`
String comparisons are case-insensitive by default. Set this to `true` for case-sensitive matching. This also applies to object and map key matching.
<br><br>
