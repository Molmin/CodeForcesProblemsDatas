## Description

<div><p>A <span class="tex-font-style-it">wavy number</span> is such positive integer that for any digit of its decimal representation except for the first one and the last one following condition holds: the digit is either strictly larger than both its adjacent digits or strictly less than both its adjacent digits. For example, numbers <span class="tex-span">35270</span>, <span class="tex-span">102</span>, <span class="tex-span">747</span>, <span class="tex-span">20</span> and <span class="tex-span">3</span> are <span class="tex-font-style-it">wavy</span> and numbers <span class="tex-span">123</span>, <span class="tex-span">1000</span> and <span class="tex-span">2212</span> are not.</p><p>The task is to find the <span class="tex-span"><i>k</i></span>-th <span class="tex-font-style-bf">smallest</span> <span class="tex-font-style-it">wavy number</span> <span class="tex-span"><i>r</i></span> that is divisible by <span class="tex-span"><i>n</i></span> for the given integer values <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span>.</p><p>You are to write a program that will find the value of <span class="tex-span"><i>r</i></span> if it doesn't exceed <span class="tex-span">10<sup class="upper-index">14</sup></span>.</p></div><div class="input-specification"><p>The only line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span>, separated by a single space (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 10<sup class="upper-index">14</sup></span>). </p></div><div class="output-specification"><p>Your task is to output the only integer <span class="tex-span"><i>r</i></span> — the answer to the given problem. If such number does not exist or it is larger than <span class="tex-span">10<sup class="upper-index">14</sup></span>, then print "<span class="tex-font-style-tt">-1</span>" (minus one without the quotes) instead.</p></div>

## Input

<p>The only line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span>, separated by a single space (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 10<sup class="upper-index">14</sup></span>). </p>

## Output

<p>Your task is to output the only integer <span class="tex-span"><i>r</i></span> — the answer to the given problem. If such number does not exist or it is larger than <span class="tex-span">10<sup class="upper-index">14</sup></span>, then print "<span class="tex-font-style-tt">-1</span>" (minus one without the quotes) instead.</p>





```input1
123 4

```




```input2
100 1

```




```input3
97461 457

```




```output1
1845

```




```output2
-1

```




```output3
1805270103

```



## Note

<p>The values of the first four <span class="tex-font-style-it">wavy numbers</span> that are divisible by <span class="tex-span"><i>n</i></span> for the first sample are: <span class="tex-span">492</span>, <span class="tex-span">615</span>, <span class="tex-span">738</span> and <span class="tex-span">1845</span>.</p>
