## Description

<div><p>In this problem you are given a string <span class="tex-span"><i>s</i></span> consisting of uppercase and lowercase Latin letters, spaces, dots and commas. Your task is to correct the formatting of this string by removing and inserting spaces, as well as changing the case of the letters.</p><p>After formatting, the resulting string must meet the following requirements:</p><ul> <li> the string must not start with a space; </li><li> there should be exactly one space between any two consecutive words; </li><li> there should be a Latin letter immediately before a dot or a comma, and there should be a space immediately after a dot or a comma in the case that there is a word after that dot or comma, otherwise that dot or comma must be the last character in the string; </li><li> all letters must be lowercase, except all first letters in the first words of the sentences, they must be capitalized. The first word of a sentence is a word that is either the first word of the string or a word after a dot. </li></ul><p>It is guaranteed that there is at least one letter in the given string between any two punctuation marks (commas and dots are punctuation marks). There is at least one letter before the leftmost punctuation mark.</p></div><div class="input-specification"><p>The first line contains a non-empty string <span class="tex-span"><i>s</i></span>, consisting of uppercase and lowercase Latin letters, spaces, dots and commas. The length of the given string does not exceed 255. The string is guaranteed to have at least one character other than the space.</p></div><div class="output-specification"><p>Output the corrected string which meets all the requirements described in the statement.</p></div>

## Input

<p>The first line contains a non-empty string <span class="tex-span"><i>s</i></span>, consisting of uppercase and lowercase Latin letters, spaces, dots and commas. The length of the given string does not exceed 255. The string is guaranteed to have at least one character other than the space.</p>

## Output

<p>Output the corrected string which meets all the requirements described in the statement.</p>





```input1
hello ,i AM veRy GooD.Boris

```




```input2
a. b,   C  .   

```




```output1
Hello, i am very good. Boris

```




```output2
A. B, c.

```


