## Description

<div><p>One of the most important products of the R1 company is a popular @r1.com mail service. The R1 mailboxes receive and send millions of emails every day.</p><p>Today, the online news thundered with terrible information. The R1 database crashed and almost no data could be saved except for one big string. The developers assume that the string contains the letters of some users of the R1 mail. Recovering letters is a tedious mostly manual work. So before you start this process, it was decided to estimate the difficulty of recovering. Namely, we need to calculate the number of different substrings of the saved string that form correct e-mail addresses.</p><p>We assume that valid addresses are only the e-mail addresses which meet the following criteria:</p><ul> <li> the address should begin with a non-empty sequence of letters, numbers, characters '<span class="tex-font-style-tt">_</span>', starting with a letter; </li><li> then must go character '<span class="tex-font-style-tt">@</span>'; </li><li> then must go a non-empty sequence of letters or numbers; </li><li> then must go character '<span class="tex-font-style-tt">.</span>'; </li><li> the address must end with a non-empty sequence of letters. </li></ul><p>You got lucky again and the job was entrusted to you! Please note that the substring is several consecutive characters in a string. Two substrings, one consisting of the characters of the string with numbers <span class="tex-span"><i>l</i><sub class="lower-index">1</sub>, <i>l</i><sub class="lower-index">1</sub> + 1, <i>l</i><sub class="lower-index">1</sub> + 2, ..., <i>r</i><sub class="lower-index">1</sub></span> and the other one consisting of the characters of the string with numbers <span class="tex-span"><i>l</i><sub class="lower-index">2</sub>, <i>l</i><sub class="lower-index">2</sub> + 1, <i>l</i><sub class="lower-index">2</sub> + 2, ..., <i>r</i><sub class="lower-index">2</sub></span>, are considered distinct if <span class="tex-span"><i>l</i><sub class="lower-index">1</sub> ≠ <i>l</i><sub class="lower-index">2</sub></span> or <span class="tex-span"><i>r</i><sub class="lower-index">1</sub> ≠ <i>r</i><sub class="lower-index">2</sub></span>.</p></div><div class="input-specification"><p>The first and the only line contains the sequence of characters <span class="tex-span"><i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span> — the saved string. It is guaranteed that the given string contains only small English letters, digits and characters '<span class="tex-font-style-tt">.</span>', '<span class="tex-font-style-tt">_</span>', '<span class="tex-font-style-tt">@</span>'.</p></div><div class="output-specification"><p>Print in a single line the number of substrings that are valid e-mail addresses.</p></div>

## Input

<p>The first and the only line contains the sequence of characters <span class="tex-span"><i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span> — the saved string. It is guaranteed that the given string contains only small English letters, digits and characters '<span class="tex-font-style-tt">.</span>', '<span class="tex-font-style-tt">_</span>', '<span class="tex-font-style-tt">@</span>'.</p>

## Output

<p>Print in a single line the number of substrings that are valid e-mail addresses.</p>





```input1
gerald.agapov1991@gmail.com

```




```input2
x@x.x@x.x_e_@r1.com

```




```input3
a___@1.r

```




```input4
.asd123__..@

```




```output1
18

```




```output2
8

```




```output3
1

```




```output4
0

```



## Note

<p>In the first test case all the substrings that are correct e-mail addresses begin from one of the letters of the word agapov and end in one of the letters of the word com.</p><p>In the second test case note that the e-mail x@x.x is considered twice in the answer. Note that in this example the e-mail entries overlap inside the string.</p>
