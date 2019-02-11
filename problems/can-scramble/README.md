# CanScramble

Write a function that returns true if one string can be formed out of another by
reordering ("scrambling") the characters.

For example:

```
can_scramble("abc", "cba") -> true
can_scramble("aab", "bba") -> false
```

```
var can_scramble = function(a,b) {
	return a.split('').sort().toString() ===  b.split('').sort().toString()
}
```

```
_.isEqual(_.sortBy('abc'), _.sortBy('acb'))
```
