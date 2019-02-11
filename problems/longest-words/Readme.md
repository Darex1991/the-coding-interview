# Longest Words

Write a function that returns the longest word(s) from a sentence. The function should not return any duplicate words (case-insensitive).

## Example

```js
longestWords("You are just an old antidisestablishmentarian") // ["antidisestablishmentarian"]
longestWords("I gave a present to my parents") // ["present", "parents"]
longestWords("Buffalo buffalo Buffalo buffalo buffalo buffalo Buffalo buffalo") // ["buffalo"] or ["Buffalo"]
```

```
var long = function(text) {
var b = text.split(' ');
var sorted = b.sort((c, d) => d.length - c.length);
var result = [];
for(var i = 0; i < sorted.length; i++) {
 if(sorted[0].length <= sorted[i].length && !result.includes(sorted[i].toLowerCase())) {
	result.push(sorted[i].toLowerCase());
 }
}
return result;
}
```
