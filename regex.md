# Regular expression

* `a*`: 0 or more characters
  `a*` = {`\epsilon`, a, aa, aaa, ...}
* `aaaaa`: a string
  `aaaaa` = {aaaaa}
* `a+`: one or more characters
  `a+` = {a, aa, aaa, ...}
* `[]`: match any character within the brackets
  `[A-Z]` = {A,B,...,Z}
* `()`: in order of chars in the brackets
  `(a*b)` = {ab, aab, b, aaab, aaaaaaaab, ...}
* `[^]`: things not in the brackets
  `[^A-Z]` = {a,b,c,...,z}
* `|` = or
  `(a|b)` = {a,b}
* `.`: only one char
  `.` = {a,b,...z,A,B,...Z}
* `^`: start of a string
  `^a` = {a, aa, aab, abcdefghijklmnopqrstuvwxyz, ...}
* `\`: indicates escaped characters
* `$`: end of string
* `?!`: does not contain
  `^((?![A-Z]).)*$` = any words not contain with a capital letter e.g. apple
