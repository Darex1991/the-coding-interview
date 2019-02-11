Calculate the sum of an array which contains integers and other arrays with integers.
For example:

```
array_sum([1,2,[3,4,[5]]])
```

would return 15. 

```
_.sum(_.flattenDeep([1,2,[3,4,[5]]]))
```
```
function flat(arr) {
  return arr.reduce(function (before, current) {
    return before + (Array.isArray(current) ? flatten2(current) : current);
  }, 0);
}
```
