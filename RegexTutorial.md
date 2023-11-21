# 17-Regex-Tutorial-on-Matching-an-Email

Regular expressions (Regex) is sometimes also referred to as rational expression, and is a sequence of characters that specifies and matches patterns within text. Regex are used often in the coding workspace to validate specific inputs. In this assignment I will be using Regex to match character information for validating email addresses.

# Summary

The code we will be summarizing today is: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

# Table of Contents

1. [Anchors](#Anchors)
2. [Quantifiers](#Quantifiers)
3. [Classes](#Classes)
4. [Grouping](#Grouping)
5. [Expressions](#Expressions)
6. [Greedy and Lazy Match](#greedy-and-lazy-match)
7. [Sources](#Sources)
8. [Author](#Author)

## Anchors

Anchors are complicated in the world of Regex, as they dont match any real characters. What anchors do however is ensure that regex matches a string to a specific place, usually the beginning or end of a coding line. The anchors used to contain this email Regex are: `^` to start, and `$` to finish.

## Quantifiers

In regular expressions the quantifiers specifies how many instances of a character group or class have to be present in the input for that code match to be found correctly. In this regex, we used `+` to communicate that there is another sequence to be matched as a greedy quantifier. We then also used `{2,6}` as another greedy quantifer to specify the input must be a minimum of 2 characters up to a maximum of 6 characters.

## Classes

In regex a character class is defined as a set of characters enclosed within square brackets. These classes then specify the characters that will be matched to a single character from given inputs. In this regex, the character class `/d` is used, which in JS classifies the use of any digit from 0 to 9.

## Grouping

Grouping is a feature of regular expressions that when used properly can simplify complex patterns within a string. In regex any subpattern that has been enclosed within parenthesis is considered a group. Capturing groups is a way of treating multiple characters as a single unit. For example the expressions (CAT) would create a single group containing the letters "C" "A" and "T".
This email matching example captures three groups. Group #1 is the username of the e-mail account `[a-z0-9_\.-]`. The second group captures the domain name or the e-mail service being used `[\da-z\.-]`. And finally, the third group captures the domain extention (i.e .com or .net) `[a-z\.]{2,6}`

## Expressions

expressions

## Greedy and Lazy Match

Greedy/Lazy Match

## Sources

Sources

# Author

me

- Github: (https://github.com/Anthonykahly)
- Email: akahly@gmail.com
