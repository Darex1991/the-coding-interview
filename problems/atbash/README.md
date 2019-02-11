Atbash is a simple substitution cipher originally for the Hebrew alphabet, but possible with any known alphabet.
```
 Original:   abcdefghijklmnopqrstuvwxyz  
 Substitute: ZYXWVUTSRQPONMLKJIHGFEDCBA
```

So you would substitute "a" in your input text with "Z" in your output text, "b" with "Y", "c" with "X" and so forth.

A few English words also 'Atbash' into other English words: "irk"="rip", "low"="old", "hob"="sly", "hold"="slow", "holy"="slob", "horn"="slim", "glow"="told", "grog"="tilt" and "zoo"="all". Some other English words Atbash into their own reverses, e.g., "wizard" = "draziw."

(https://en.wikipedia.org/wiki/Atbash)


```
var sub = function(text, original = original1, substitute = substitute1) {

const org = original.split('');
const sub = substitute.split('');
	var newText = '';   
	for(var i = 0; i<text.length; i++) {
		const index = org.findIndex((a) => a === text[i]);
		newText += sub[index];
	}
return newText;
}
```

```
var sub = function(text, original = original1, substitute = substitute1) {
	const org = _.split(original, '');
	const sub = _.split(substitute, '');
	let newText = '';   
    _.each(text, (a) => { 
        const index = _.findIndex(org, (b) => b === a);
        newText += sub[index];
	})
	
	return newText;
}
```
