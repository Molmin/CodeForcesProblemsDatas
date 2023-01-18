## Description

<div><p>A non-empty string <span class="tex-span"><i>s</i></span> is called <span class="tex-font-style-it">binary</span>, if it consists only of characters "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1</span>". Let's number the characters of binary string <span class="tex-span"><i>s</i></span> from 1 to the string's length and let's denote the <span class="tex-span"><i>i</i></span>-th character in string <span class="tex-span"><i>s</i></span> as <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Binary string <span class="tex-span"><i>s</i></span> with length <span class="tex-span"><i>n</i></span> is <span class="tex-font-style-it">periodical</span>, if there is an integer <span class="tex-span">1 ≤ <i>k</i> &lt; <i>n</i></span> such that: </p><ul> <li> <span class="tex-span"><i>k</i></span> is a divisor of number <span class="tex-span"><i>n</i></span> </li><li> for all <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i> - <i>k</i></span>, the following condition fulfills: <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> = <i>s</i><sub class="lower-index"><i>i</i> + <i>k</i></sub></span> </li></ul><p>For example, binary strings "101010" and "11" are periodical and "10" and "10010" are not.</p><p>A positive integer <span class="tex-span"><i>x</i></span> is <span class="tex-font-style-it">periodical</span>, if its binary representation (without leading zeroes) is a periodic string.</p><p>Your task is to calculate, how many periodic numbers are in the interval from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> (both ends are included).</p></div><div class="input-specification"><p>The single input line contains two integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">18</sup></span>). The numbers are separated by a space.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the cin, cout streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div><div class="output-specification"><p>Print a single integer, showing how many periodic numbers are in the interval from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> (both ends are included).</p></div>

## Input

<p>The single input line contains two integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">18</sup></span>). The numbers are separated by a space.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the cin, cout streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>

## Output

<p>Print a single integer, showing how many periodic numbers are in the interval from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> (both ends are included).</p>





```input1
1 10

```




```input2
25 38

```




```output1
3

```




```output2
2

```



## Note

<p>In the first sample periodic numbers are <span class="tex-span">3</span>, <span class="tex-span">7</span> and <span class="tex-span">10</span>.</p><p>In the second sample periodic numbers are <span class="tex-span">31</span> and <span class="tex-span">36</span>.</p>
