## Lecture: Collection Operations

Regular expressions (regex) are powerful tools for finding specific patterns in text. Here's a brief explanation of the collection operations:

### 1. Character Sets

Character sets match any one character enclosed in the square brackets `[]`.

For example, the regex `[abc]` will match any single character that is either 'a', 'b', or 'c'.

```regex
/[abc]/
```

### 2. Ranges
Ranges allow you to specify a range of characters within a character set.

For example, the regex `[a-z]` will match any single lowercase letter, and `[0-9]` will match any single digit.

```regex
/[a-z]/
/[0-9]/
```

### 3. Negated Character Sets
Negated character sets match any other character not enclosed in the square brackets `[^]`.

For example, the regex `[^abc]` will match any single character that is **<ins>not</ins>** ‘a’, ‘b’, or ‘c’. But any other characters beside will be matched (example: 'd', 'e', 'f', ..., will be matched).

```regex
/[^abc]/
````

<br>

----
#### Summary
`[ ]`: The **square brackets** indicates a character set, or collection.  

`[a-z]`: The **hyphen** within the brackets indicates a range in a character set. In this case, **any** **lowercase** letter from **a** through **z**.  

`[^]`: The **caret symbol** at the start of a set **negates** the set, or collection.


#### 🔥 A note about the `^` caret symbol
When used outside of a character set, the `^` matches the start of the input. For example: `^H` will any string that start with 'H', just like in 'How i met your mother'.

```regex
/^H/