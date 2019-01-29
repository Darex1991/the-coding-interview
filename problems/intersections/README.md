List Intersection
=================

Given two lists of strings, find the intersection of the two lists.

Sample Input:
$a1 = ['dog', 'cat', 'egg']
$a2 = ['cat', 'dog', 'chicken']

Output:
$out = ['dog', 'cat']


$a1 = ['dog', 'cat', 'egg']; $a2 = ['cat', 'dog', 'chicken'];
var c = [];for(var i = 0; i < $a1.length; i++) {var a = $a1[i]; if($a2.includes(a)){c.push(a)}} console.log(c)
