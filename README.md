# A Beginner's Guide to Regular Expressions (Regex)

Regular Expressions, also known as regex, is a powerful tool for searching and manipulating text. In this guide, we will provide a comprehensive overview of the most essential regex components and explain how they work. We will cover anchors, quantifiers, grouping constructs, bracket expressions, character classes, the OR operator, flags, and character escapes. By the end of this guide, you should have a solid understanding of regex and be able to apply it to your own projects.

## Summary

In this guide, we will provide a comprehensive overview of the most essential regex components and explain how they work. We will cover anchors, quantifiers, grouping constructs, bracket expressions, character classes, the OR operator, flags, and character escapes. Here is an example of a regex that we will be describing:

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

This regex is used to validate email addresses.

1. `/^` - This denotes the start of the regular expression and ensures that the match starts at the beginning of the string.
2. `([a-z0-9_.-]+)` - This matches the username part of the email address, which consists of one or more lowercase letters, numbers, underscores, dots, or hyphens. The parentheses around this part capture the username as a group.
3. `@` - This matches the @ symbol that separates the username from the domain name.
4. `([\da-z.-]+)` - This matches the domain name, which consists of one or more lowercase letters, numbers, dots, or hyphens. The `[\da-z.-]` part is a character set that matches digits, lowercase letters, dots, and hyphens. The parentheses around this part capture the domain name as a group.
5. `.` - This matches the period that separates the domain name from the top-level domain (TLD).
6. `([a-z.]{2,6})$/` - This matches the TLD, which consists of two to six lowercase letters or dots. The parentheses around this part capture the TLD as a group. The `$` at the end of the regex ensures that the match ends at the end of the string.

So, overall, this regex matches an email address that consists of a username, followed by an `@` symbol, a domain name, a period, and a TLD.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)
- [Credits](#credits)
- [Questions](#questions)

## Regex Components

### Anchors

Anchors are used to match a position rather than a character. They are used to specify the start or end of a line or a word. Examples of anchors are `^` which matches the start of a line, `$` which matches the end of a line, and `\b` which matches a word boundary.

### Quantifiers

Quantifiers are used to specify the number of times a character or a group of characters should be repeated. Examples of quantifiers are `*` which matches zero or more times, `+` which matches one or more times, `?` which matches zero or one time, and `{n}` which matches exactly n times.

### Grouping Constructs

Grouping constructs are used to group patterns together and apply quantifiers to them. They are enclosed in parentheses `()` and can be nested. Examples of grouping constructs are `(abc)+` which matches the pattern abc one or more times, and `(ab|cd)` which matches either `ab` or `cd`.

### Bracket Expressions

Bracket expressions, also known as character sets, are used to match a single character from a set of characters. They are enclosed in square brackets `[]`. Examples of bracket expressions are `[abc]` which matches either `a`, `b`, or `c`, and `[0-9]` which matches any digit.

### Character Classes

Character classes are shorthand representations of commonly used bracket expressions. Examples of character classes are `\d` which matches any digit, `\s` which matches any whitespace character, and `\w` which matches any word character.

### The OR Operator

The OR operator, denoted by the `|` character, matches either the pattern on the left or the pattern on the right. Examples of the OR operator are `(abc|def)` which matches either `abc` or `def`, and `[a-z]|[A-Z]` which matches any lowercase or uppercase letter.

### Flags

Flags modify how the regex engine treats the input string. Some commonly used flags include:

`g`: global flag to match all occurrences of the pattern<br>
`i`: case-insensitive matching<br>
`m`: multi-line matching<br>
`u`: enables full Unicode support<br>
`y`: sticky matching that starts at the last matched position in the input string<br>

You can add flags to the end of the regex expression, such as `/pattern/gi`.

### Character Escapes

Character escapes allow you to match special characters like newlines or tabs. They are denoted by a backslash followed by a special character. Some commonly used character escapes include:

`\n`: matches a newline character<br>
`\t`: matches a tab character<br>
`\d`: matches any digit character (0-9)<br>
`\w`: matches any word character (a-z, A-Z, 0-9, or \_)<br>
`\s`: matches any whitespace character (space, tab, newline, etc.)<br>

For example, to match a string containing a newline character, you could use the regex /hello\nworld/.

## Credits

:bust_in_silhouette: [David Michael Mackey](https://www.notion.so/davidmichaelmackey/David-Mackey-a59ce61a996840d6a933e3b135673467?pvs=4)<br>
:email: [Email](mailto:davidmackey@hey.com)<br>
:octocat: [GitHub](https://github.com/davidmichaelmackey/)<br>
:briefcase: [Linkedin](https://linkedin.com/in/davidmichaelmackey/)<br>

## Questions

Have Questions? Feel free send me an [email](mailto:davidmackey@hey.com) or reach out to me on [Linkedin](https://linkedin.com/in/davidmichaelmackey/).
