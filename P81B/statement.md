## Description

<div><p>Polycarp is very careful. He even types numeric sequences carefully, unlike his classmates. If he sees a sequence without a space after the comma, with two spaces in a row, or when something else does not look neat, he rushes to correct it. For example, number sequence written like "<span class="tex-font-style-tt">1,2&nbsp;,3,...,&nbsp;&nbsp;&nbsp;10</span>" will be corrected to "<span class="tex-font-style-tt">1,&nbsp;2,&nbsp;3,&nbsp;...,&nbsp;10</span>".</p><p>In this task you are given a string <span class="tex-span"><i>s</i></span>, which is composed by a concatination of terms, each of which may be: </p><ul> <li> a positive integer of an arbitrary length (leading zeroes are not allowed), </li><li> a "comma" symbol ("<span class="tex-font-style-tt">,</span>"), </li><li> a "space" symbol ("<span class="tex-font-style-tt"> </span>"), </li><li> "three dots" ("<span class="tex-font-style-tt">...</span>", that is, exactly three points written one after another, also known as suspension points). </li></ul><p>Polycarp wants to add and remove spaces in the string <span class="tex-span"><i>s</i></span> to ensure the following: </p><ul> <li> each comma is followed by exactly one space (if the comma is the last character in the string, this rule does not apply to it), </li><li> each "three dots" term is preceded by exactly one space (if the dots are at the beginning of the string, this rule does not apply to the term), </li><li> if two consecutive numbers were separated by spaces only (one or more), then exactly one of them should be left, </li><li> there should not be other spaces. </li></ul><p>Automate Polycarp's work and write a program that will process the given string <span class="tex-span"><i>s</i></span>.</p></div><div class="input-specification"><p>The input data contains a single string <span class="tex-span"><i>s</i></span>. Its length is from 1 to 255 characters. The string <span class="tex-span"><i>s</i></span> does not begin and end with a space. Its content matches the description given above.</p></div><div class="output-specification"><p>Print the string <span class="tex-span"><i>s</i></span> after it is processed. Your program's output should be <span class="tex-font-style-it">exactly</span> the same as the expected answer. It is permissible to end output line with a line-break character, and without it.</p></div>

## Input

<p>The input data contains a single string <span class="tex-span"><i>s</i></span>. Its length is from 1 to 255 characters. The string <span class="tex-span"><i>s</i></span> does not begin and end with a space. Its content matches the description given above.</p>

## Output

<p>Print the string <span class="tex-span"><i>s</i></span> after it is processed. Your program's output should be <span class="tex-font-style-it">exactly</span> the same as the expected answer. It is permissible to end output line with a line-break character, and without it.</p>





```input1
1,2 ,3,...,     10

```




```input2
1,,,4...5......6

```




```input3
...,1,2,3,...

```




```output1
1, 2, 3, ..., 10

```




```output2
1, , , 4 ...5 ... ...6

```




```output3
..., 1, 2, 3, ...

```


