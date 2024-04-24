## Lecture: Whitespace Characters and String Boundaries

Regular experssions (regex) are powerful tools for finding specific patterns in text. Here's a brief explanation about whitespace characters and string boundaries.

### 1. Whitespace Characters

A whitespace character is any empty space in a string. It can be a space ` `, a tab `\t`, a new line `\n`, or a carriage return `r` (used in old typewriters and Windows). In addition to these, there are two more whitespace characters: the vertical tab `\v` and the form feed character `\f`. However, these are not commonly used nowadays.

And there's a special symbol `\s` that can match any of these whitespaces.  


| Whitespace Character | Symbol   |
-----------------------|----------|
| space                |` `       |
| tab                  | **`\t`** |
| new line             | **`\n`** |
| return               | **`\r`** |
| vertical tab         | **`\v`** |
| form feed            | **`\f`** |
| to match'em all      | **`\s`** |



### 2. String Boundaries

They're special characters very useful when there's a need to match a pattern that is located at the beginning `^` or end of a string `$`.  


| To locate pattern at the  | Symbol  |
----------------------------|---------|
| beginning of a string     | **`^`** |
| end of a string           | **`$`** |


<br>

----
#### Summary

There's special symbols to match whitespaces characters as **spaces (` `)**, **tabs (`\t`)**, **new lines (`\n`)** and **returns (`\r`)**. And **one to match'em all**, the special symbol **(`\s`)**.

If needed to match a pattern at the **beginning of a string**, use **(^)** and at the **end of a string ($)**.


#### 🔥 A note about the `^` caret symbol
When the `^` is the first character inside of a character set `[]`, it negates the set. This means it will match any character that is not in the set. For example: in `[^abc]def` only 'd', 'e' and 'f' will be matched.

```regex
/[^abc]def/