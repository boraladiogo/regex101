## Regular Expressions: Quantifiers

Regular expressions (regex) are powerful tools for finding specific patterns in text. Here's a brief explanation of the `+`, `?`, and `{}` operations:

### 1. Plus (+) 

The `+` character is a quantifier that matches the preceding element 1 or more times. 

For example, the regex `a+` will match 'a', 'aa', 'aaa', and so on.

```regex
/a+/
```

### 2. Question Mark (?) / Optional
The ? character is a quantifier that matches the preceding element 0 or 1 times, making it optional.

For example, the regex a? will match ‘ ’, ‘a’.

```regex
/a?/
```

### 3. Braces ({}) / How many
The {} characters are quantifiers that match the preceding element a specific number of times.

{n} matches exactly n times.
{n,} matches n or more times.
{n,m} matches at least n times but no more than m times.
For example, the regex a{2,4} will match ‘aa’, ‘aaa’, and ‘aaaa’.

```regex
/a{2,4}/
```

<br>

---
#### Summary

`+` at least one of the character  
`?` may have or may not have *(optional)*  
`{n}` / `{n, m}` how many characters *(exactly **N** or a range between **N~M**)*  