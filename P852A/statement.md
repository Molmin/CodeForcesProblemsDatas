## Description

<div><p>John gave Jack a very hard problem. He wrote a very big positive integer <span class="tex-span"><i>A</i><sub class="lower-index">0</sub></span> on a piece of paper. The number is less than <span class="tex-span">10<sup class="upper-index">200000</sup></span> . In each step, Jack is allowed to put <span class="tex-span">' + '</span> signs in between some of the digits (maybe none) of the current number and calculate the sum of the expression. He can perform the same procedure on that sum and so on. The resulting sums can be labeled respectively by <span class="tex-span"><i>A</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>A</i><sub class="lower-index">2</sub></span> etc. His task is to get to a single digit number.</p><p>The problem is that there is not much blank space on the paper. There are only three lines of space, so he can't perform more than three steps. Since he wants to fill up the paper completely, he will perform exactly three steps.</p><p>Jack must not add leading zeros to intermediate results, but he can put <span class="tex-span">' + '</span> signs in front of digit <span class="tex-span">0</span>. For example, if the current number is <span class="tex-span">1000100</span>, <span class="tex-span">10 + 001 + 00</span> is a valid step, resulting in number <span class="tex-span">11</span>.</p></div><div class="input-specification"><p>First line contains a positive integer <span class="tex-span"><i>N</i> (1 ≤ <i>N</i> ≤ 200000)</span>, representing the number of digits of <span class="tex-span"><i>A</i><sub class="lower-index">0</sub></span>.</p><p>Second line contains a string of length <span class="tex-span"><i>N</i></span> representing positive integer number <span class="tex-span"><i>A</i><sub class="lower-index">0</sub></span>. Each character is digit. There will be no leading zeros.</p></div><div class="output-specification"><p>Output exactly three lines, the steps Jack needs to perform to solve the problem. You can output any sequence of steps which results in a single digit number (and is logically consistent).</p><p>Every step consists of digits and <span class="tex-span">' + '</span> signs. Steps should not contain several <span class="tex-span">' + '</span> signs in a row, whitespaces, or <span class="tex-span">' + '</span> signs as the first or last character. They also need to be arithmetically consistent.</p><p>Solution might not be unique. Output any of them in that case.</p></div>

## Input

<p>First line contains a positive integer <span class="tex-span"><i>N</i> (1 ≤ <i>N</i> ≤ 200000)</span>, representing the number of digits of <span class="tex-span"><i>A</i><sub class="lower-index">0</sub></span>.</p><p>Second line contains a string of length <span class="tex-span"><i>N</i></span> representing positive integer number <span class="tex-span"><i>A</i><sub class="lower-index">0</sub></span>. Each character is digit. There will be no leading zeros.</p>

## Output

<p>Output exactly three lines, the steps Jack needs to perform to solve the problem. You can output any sequence of steps which results in a single digit number (and is logically consistent).</p><p>Every step consists of digits and <span class="tex-span">' + '</span> signs. Steps should not contain several <span class="tex-span">' + '</span> signs in a row, whitespaces, or <span class="tex-span">' + '</span> signs as the first or last character. They also need to be arithmetically consistent.</p><p>Solution might not be unique. Output any of them in that case.</p>





```input1
1
1

```




```input2
4
5806

```




```output1
1
1
1

```




```output2
5+8+0+6
1+9
1+0

```



## Note

<p>In the first sample, Jack can't put <span class="tex-span">' + '</span> signs anywhere, so he just writes <span class="tex-span">1</span> in each line and solves the problem. Here, solution is unique.</p><p>In the second sample, Jack first puts <span class="tex-span">' + '</span> between every two consecutive digits, thus getting the result <span class="tex-span">5 + 8 + 0 + 6 = 19</span>. He does the same on the second step, getting <span class="tex-span">1 + 9 = 10</span>. Once more, he gets <span class="tex-span">1 + 0 = 1</span>, so after three steps, the result is <span class="tex-span">1</span> and his solution is correct.</p>
