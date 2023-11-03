#  REGEX MODEL
### model
Matching a URL:
Regex: ^(https?|ftp)://[^\s/$.?#].[^\s]*$

Example:
http://www.example.com 
ftp://files.example.org/path/to/file



## Table of Contents

1. [Introduction](#introduction)
2. [Matching URL Model and Description](#regex)
3. [Character Classes](#char-classes)
4. [Quantifiers](#quantifiers)
5. [Anchors](#anchors)
6. [Author's Section](#authors-section)


## Introduction 
Regular expressions are widely used in programming, text processing, and data extraction tasks. They are supported by many programming languages, text editors, and tools, making them a versatile tool for tasks such as:
Regular expressions consist of a combination of characters and metacharacters that specify the pattern to be matched. They allow you to define complex patterns for text matching in a concise and flexible way. However, they can be quite cryptic and may take some time to master.

## Matching Url Regular Expression Model and Description
The 'Matching Url" regular expression is used to match URLs with the "http", "https", or "ftp" schemes, ensuring that the URL contains only valid characters and no spaces. It validates the basic structure of a URL but doesn't check whether the URL is reachable or functional. It can be used for URL validation in various applications such as form input validation and data extraction. 


### ^(https?|ftp)://[^\s/$.?#].[^\s]*$

^: This symbol ensures that the regex matches from the beginning of the input.

(https?|ftp): This is is used to match the URL scheme, which could be "http", "https", or "ftp".

://: This part of the regex is a common delimiter in URLs, separating the scheme from the rest of the URL.

[^\s/$.?#]: This matches a single character that is not any of the characters listed inside. 

Description of each character:

[^\s]: Matches any character that is not whitespace.
[/]: Matches the forward slash character.
[$]: Matches the dollar sign character.
[.]: Matches the period (dot) character.
[?]: Matches the question mark character.
[#]: Matches the hash (pound) character.

.: A dot (period) outside of square brackets is used here to match the period separating the domain from the top-level domain (TLD) in the URL.

[^\s]*: This matches zero or more characters that are not whitespace. This part of the regex is used to match the domain part of the URL.

$: This symbol ensures that the regex matches to the end of the input.














## Basics

## Quantifiers

## Anchors

## Author's Section
