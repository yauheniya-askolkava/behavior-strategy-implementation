# [Remove duplicates from the list](https://www.codewars.com/kata/57a5b0dfcf1fa526bb000118/train/javascript)

Function removes the duplicates from an array of numbers and returns it as a result. The order of the sequence stays the same.

## Syntax

> distinct(`array`) -> `array`

### Parameters

**a**: `array`

- an array of numbers with some of them duplicate

### Return Value: `array`

The same return with no duplicates.

## Examples

The function is supposed to return an orderly array with no duplicates, perhaps parsing the data from one or another document.

```js
const a = [1, 2, 2, 2, 3];
const result = distinct(a);
console.log(result); // [1, 2, 3]
```

```js
const a = ["a", "a", "a", "a", "c"];
const result = distinct(a);
console.log(result); // ["a", "c"]
```


## [wichu](https://www.codewars.com/kata/reviews/580a1bd1b56dcf80b2000031/groups/580a6b5de4912cf0cc000128)

```js
function distinct(a) {
  return Array.from(new Set(a));
}
```

### Strategy

The strategy is based on a method in combination with an object, which provide a removal of repetition as a result.

### Implementation


**Array.from(Set)**: that is a method with a newly created Set object make a distinction on repetitve values.

### Possible Refactors

- could have been done: 
const distinct = a => [...new Set(a)];


## [Elsir](https://www.codewars.com/kata/reviews/580a1bd1b56dcf80b2000031/groups/5aec4d426d46ad5654000045)

```js
const distinct = a => a.filter((item, index) => a.indexOf(item) === index);
```

### Strategy

The person parses the elements in the array based on their position in the array.

### Implementation

**method of indexOf**: returns the position of the first occurrence of the item in combination with **strict equality** to the index.

**filter method**: creates a new array which is passed under the mentioned condition of indexOf method.

### Possible Refactors

reduce and include methods might have played the same functionality I guess here.


---

## Notes


- I learnt the methods of filter and indexOf a bit.
- I would like to learn the methods more in depth or have a handy cheatsheet, maybe?
