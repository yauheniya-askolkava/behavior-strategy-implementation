# [Convert boolean values to strings 'Yes' or 'No'.](https://www.codewars.com/kata/53369039d7ab3ac506000467/train/javascript)

The fucntion is to convert values to strings 'Yes' or No'

## Syntax

> boolToWord( bool ) -> string

### Parameters

**bool**: `boolean`

- an answer in a form of string as Yes or No

### Return Value: `string`

Returns Yes or No in terms of string, an abstraction with no precision.

## Examples

No complicated edge-cases, the function converts any boolean to a string.

```js
const bool = true
const result = boolToWord('bool')
console.log(result) // string

---

const bool = false
const result = boolToWord('bool')
console.log(result) // string

```

## [weavermeadia](https://www.codewars.com/kata/reviews/54a59ef00c96357db90000e9/groups/54a6a5cb478d8e25c700099b)

```js
function boolToWord( bool ){
  if (bool) {
    return 'Yes';
  } else {
    return 'No';
  }
}
```

### Strategy

The strategy is to turn the parameter to a string in any case, whether one condition or another.

### Implementation

if/else statement, what provides no exit, but to return a necessary string of Yes or No.

### Possible Refactors

- ternary operator might have been a solution


## [weavermedia](https://www.codewars.com/kata/reviews/54a59ef00c96357db90000e9/groups/54a81d47d56c6d36f1000b42)

```js
function boolToWord( bool ){
  if( bool ){
    return "Yes";
  }
  
  return "No";
  
}
```

### Strategy

A simple function, which forcefully returns Yes or No reply with a single condition.

### Implementation


**if conditional**: with no else-satement as previous, the exit from the function defines an alternative result as No.

### Possible Refactors

There is a range of refactors, mentioned in the solutions, ones define the truthiness using the strict operator === - yet still with a conditional statement if or if else. 

Arrays are possibilities too, but more complex.


---

## Notes


- It took me sometime to realise how it could be used in some practice, what I discovered, that it is in fact necessery for UX design, where true or false sounds intimidating, the string might be a solution.
- I wish I could understand better how to implement it with array.
