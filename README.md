#  REGEX: MATCHING URL 

## Introduction 
### What is Regex?
Regular expressions are widely used in programming, text processing, and data extraction tasks. They are supported by many programming languages, text editors, and tools.
Regex consists of a combination of characters and metacharacters that specify the pattern to be matched. They allow you to define complex patterns for text matching in a concise and flexible way.

## Table of Contents
1. [Introduction](#Introduction)
2. [Matching URL Model](#model)
3. [Anchors](#anchors)
4. [Operator](#operator)
5. [Character Classes](#character-classes)
6. [Flags](#flags)
7. [Grouping and Capturing](#grouping-and-capturing)
8. [Bracket Expressions](#bracket-expressions)
9. [Summary](#summary)
10. [Look-ahead and Look-behind](#look-aheadLook-behind)
11. [Author's Section](#authors-section)


## Model 

### Matching Url RegEx
The 'Matching Url" regular expression is used to match URLs with the "http", "https", or "ftp" schemes, ensuring that the URL contains only valid characters and no spaces. It validates the basic structure of a URL but doesn't check whether the URL is reachable or functional. It can be used for URL validation in various applications such as form input validation and data extraction. 

Matching URL Model:

`^(https?|ftp)://[^\s/$.?#].[^\s]*$`

### Anchors:
`^` (caret) - Matches the start of a line or string.
In this pattern, it indicates that the URL should start with the specified protocols (http, https, or ftp).

### Operator:
`|` (pipe) - Specifies alternatives.
In this pattern, it allows matching URLs that start with either "http," "https," or "ftp."


### Character Classes:
`[^\s/$.?#]` - A character class that matches a single character that is not a space, "/", "$," ".", "?," or "#."


### Grouping and Capturing:
Parentheses `()` are used to group subpatterns. In this pattern, they are used to group the protocols for the OR operator.

### Bracket Expressions:
`[...]` - Defines a set of characters to match. In this pattern, it is used in the character class to specify characters that are not allowed in the URL path.

## Summary 
In summary, this regex pattern is used to match URLs that start with either "http," "https," or "ftp," followed by "://," and then any characters except whitespace, "/", "$," ".", "?," or "#." It ensures that the URL adheres to a basic structure commonly found in web addresses. This regex does not capture specific URL components; it checks if the URL matches this structure.


## Author's Section

### Authors Name: Ramen Dosanjh
### Github Repo: https://github.com/ramendosanjh
### Contact: ramendosanjh@outlook.com
