# Character Positioning Notes

Instead of having your function countLetters return just the count of each letter, the requirement has changed to return all the indices (zero-based positions) in the string where each character is found. So for each letter, we're no longer returning just one number to represent its number of occurrences, but rather (potentially) multiple numbers to represent all the places in the string that it shows up.


1. First, ask yourself: What would the resulting object (key-value mapping) look like with the same example string ("lighthouse in the house")?

```
{
  l: [0],
  i: [1, 10],
  g: [2],
  h: [3, 5, 13, 15],
  t: [4, 12],
  o: [6, 16],
  u: [7, 17],
  s: [8, 18],
  e: [9, 14, 19],
  n: [11]
}
```

"lighthouse in the house"