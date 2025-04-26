# Completed javascript Tutorial with Regular Ex[ressions
Today, I dove deep into one of the most powerful tools in programming — Regular Expressions (RegEx). If you've ever wanted to match patterns in strings easily, RegEx is your best friend. Let’s explore everything I learned today.

## What are Regular Expressions?
Regular Expressions are patterns used to match character combinations in strings. JavaScript provides a powerful RegExp object to define and work with these patterns.

## Patterns and Flags
A pattern defines what you want to search for.

Flags change how the search behaves.

Common flags:

g — global search (find all matches)

i — case-insensitive search

m — multiline search

u — Unicode mode

y — sticky search (starts at specific position)

## Character Classes
Character classes help match specific types of characters:

\d	Digit (0–9)

\D	Non-digit

\w	Word character (a-z, A-Z, 0-9, _)

\W	Non-word character

\s	Whitespace (spaces, tabs, etc.)

\S	Non-whitespace

## Unicode Support: Flag u and Class \p{...}
The u flag enables full Unicode support. With it, we can use \p{...} to match characters by Unicode property.

## Anchors: Start ^ and End $
^ asserts position at the start of the string.

$ asserts position at the end.

## Multiline Mode (m Flag)
Normally, ^ and $ work with the start and end of the whole string.
With m flag, they work with the start/end of each line.

## Word Boundaries: \b
\b matches a word boundary — the position between a word character and a non-word character.

## Escaping Special Characters
Special characters (like ., *, ?, etc.) must be escaped with a backslash \ if you want to match them literally.

## Sets and Ranges [ ... ]
Square brackets create a set of characters to match.

## Quantifiers: +, *, ?, {n}
Quantifiers specify how many times a pattern should repeat:

+	One or more times

*	Zero or more times

?	Zero or one time

{n}	Exactly n times

{n,}	n or more times

{n,m}	Between n and m times

## Greedy and Lazy Quantifiers
Greedy: matches as much as possible (default).

Lazy: matches as little as possible by adding ?.

## Capturing Groups ( ... )
Parentheses are used to group patterns and capture matched substrings.

## Backreferences: \N and \k<name>
Backreferences let you reuse captured groups.

\1, \2, etc., refer to capturing groups by number.

\k<name> refers to named groups.

## Alternation (OR) |
Alternation lets you match one thing OR another.

## Lookahead and Lookbehind
Lookahead: match only if followed by something.

Lookbehind: match only if preceded by something.

