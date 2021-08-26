---
layout: lesson
root: .  # Is the only page that doesn't follow the pattern /:path/index.html
permalink: index.html  # Is the only page that doesn't follow the pattern /:path/index.html
---

Do you often work with lots of data files on the computer?
Are you often trying to spot particular files or lines of text in them that are important for you?

If so, then using regular expressions could save you a lot of time and frustration!

Regular expressions (regex/REs) are a method for describing patterns of characters
that you want to match in a body of text.
A knowledge of regular expressions can be extremely helpful in computational biology
and when combined with text editors and common tools (`grep`, `sed`, `awk`, etc)
used in command line computing.

These course materials are designed to give an introduction to using regular regular expressions.
Working through the materials, you will learn how to quickly find and replace text in large files,
controlling the types and numbers of characters matched,
handling repeats,
keeping certain parts of a matched pattern during replacement,
and constructing sets of different options to be matched.

The course does not provide a comprehensive overview of the regex syntax or engine.
Instead, they reflect the vast majority of use cases that the authors encounter.
The background of the authors is represented in many of the examples chosen,
which often focus on biological contexts and file formats.

For a comprehensive overview of regular expressions, we highly recommend the excellent
[regular-expressions.info](http://www.regular-expressions.info/).

> ## Prerequisites
>
> To follow this lesson, learners should know how to open a text file on their computer,
> and some familiarity with the _Find/Replace_ functionality
> available in most text editing tools will be beneficial.
> The examples used will feel most relevant to those who are familiar with common file formats
> used to represent biological data, and some knowledge of sequence biology
> (DNA/RNA and protein sequences) is assumed.
{: .prereq}

{% include links.md %}
