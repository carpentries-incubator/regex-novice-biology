---
title: "Introduction"
teaching: 0
exercises: 0
questions:
- "What is a regular expression?"
- "In what programs can I use regular expessions?"
objectives:
- "Explain that regular expressions are a way of describing patterns in text."
- "Describe circumstances where a regular expression search could be helpful."
- "Access the regular expression search function of a text editor."
keypoints:
- "Regular expressions are a way of describing patterns in text."
- "Most text editors and many other tools include a regular expression engine for performing these kinds of searches."
- "Regular expressions are often offered as a mode of find/replace that can be turned on and off by the user."
---

## What is a regular expression?

A regular expression (regex) is a string of characters
defining a pattern to be found in a block of text.
A regex can be constructed to allow multiple possible matches,
while restricting other possibilities,.
This makes them considerably more powerful and precise
than the simple 'CTRL+F' or 'Find/Replace' operations
that you might be familiar with
from word processing/web browser software.
It is also possible to use regular expressions to
specify parts of the search pattern that will be kept in
the replacement string of a substitution operation.

### Illustrative Example

Imagine that you have a long text document.
The document contains a lot of numbers -
years (2014, 2016, 1998, etc),
digits (9, 4, 58, etc),
and a single phone number (i.e. twelve digits).
You need to find the phone number,
but it is buried in this large body of text, amongst many other numbers.
You cannot remember much about the phone number
(like what digit(s) it starts with),
you can't just randomly search strings of digits with
`CTRL+F`/`Find/Replace`,
because there are far too many possible combinations
(one *trillion* twelve-digit numbers!),
and simply performing ten individual searches
for the digits from `0` to `9` returns many unwanted results.

You *could* run one of these searches for an individual digit,
then manually click through each result,
until you eventually find the phone number.
Or you could simply scroll through the document,
looking for something that resembles a phone number.
But that is likely to take a *long* time, is really boring,
and it would be easy to miss the number while hastily scanning
through so many pages.

With regular expressions, you can define a pattern to find
any combination of twelve digits in succession,
which you can use to find the phone number -
and nothing else -
wherever it is in the document.


## Regular Expression Engines

In order to perform a regex search,
you need to provide the expression to a program that can interpret it.
Such tools are known as regular expression engines.
Unfortunately, there are multiple different 'flavours' of regex engines,
which each work slightly differently.
However, the core rules, which are covered in this lesson and
will probably address 99.9% of your text-searching needs,
are effectively common to all of them.


## How can I use Regular Expressions?

### Text Editors

Most text editors include a regular expression engine
to provide regex search/replace functionality.
See [the Setup page](setup) for suggested text editors to
use on different operating systems when following this lesson.

Usually, you will need to specify that you want to
use regular expression searching instead of
the normal plain text searching that you may already be familiar with.
When you open up the `Find/Replace` interface in your editor,
you should look for an option with a label like
"mode", "grep-like", "regular expression" or "regex",
and use this to control the type of searching that you want to do.

### Command Line

In addition, several Unix command line tools are commonly available
that use regular expressions,
for searching (e.g. `grep`/`egrep`)
and replacement/substitution (e.g. `sed`, `awk`, `perl -e`).

{% include links.md %}
