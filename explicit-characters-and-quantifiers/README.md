## Lecture: Quantifiers

Regular expressions (regex) are powerful tools for finding specific patterns in text. Here's a brief explanation of the `*`, `+`, `?`, and `{}` operations:

### 1. Asterisk (*)
The `*` character is a quantifier that matches the preceding element 0 or an unlimited times.  

For example the regex `a*bc` will match 'bc', 'abc', 'aaabc', and so on.

```regex
/a*bc/
```  

### 1. Plus (+) 

The `+` character is a quantifier that matches the preceding element 1 or more times. 

For example, the regex `a+bc` will match 'abc', 'aabc', 'aaabc', and so on. **<ins>But won't match 'bc'</ins>**.

```regex
/a+bc/
```

### 2. Question Mark (?)
The ? character is a quantifier that matches the preceding element 0 or 1 times, making it optional.

For example, the regex `a?bc` will match ‘bc’, ‘abc’. **<ins>But won't match 'aabc'</ins>**.

```regex
/a?bc/
```

### 3. Curly Braces ({})
The {} characters are quantifiers that match the preceding element a specific number of times.

{n} matches exactly n times.
{n,} matches n or more times.
{n,m} matches at least n times but no more than m times.
For example, the regex a{2,4} will match ‘aa’, ‘aaa’, and ‘aaaa’. **<ins>But won't match 'a' or 'aaaaa', and so on</ins>**.

```regex
/a{2,4}/
```

<br>

---
#### Summary

`*`: The **asterisk** indicates that the preceding character or group will be matched **zero** or **unlimited**, *id est*, somewhat like a combination of the `+` and `?` quantifiers (it's optional, but if it exists, can be one or more of it). 

`+`: The **plus sign** indicates that the preceding character or group will be matched **one** or **more times**, *id est*, **at least once**.  

`?`: The **question mark** makes the preceding character or group **optional**.  

`{n}` / `{n, m}`: These **curly braces** are used to specify the **exact number** <ins>**or**</ins> **range of times** a preceding character or group should be matched. `{n}` matches exactly **n times** and `{n, m}` matches **between n and m times**.
