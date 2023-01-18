## Description

<div><p>Let's assume that we have a sequence of doubles <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index">|<i>a</i>|</sub></span> and a double variable <span class="tex-span"><i>x</i></span>. You are allowed to perform the following two-staged operation:</p><ol> <li> choose an index of the sequence element <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ |<i>a</i>|)</span>; </li><li> consecutively perform assignments: <img align="middle" class="tex-formula" src="file://zUxFpjf6.png" style="max-width: 100.0%;max-height: 100.0%;">. </li></ol><p>Let's use function <span class="tex-span"><i>g</i>(<i>a</i>, <i>x</i>)</span> to represent the largest value that can be obtained from variable <span class="tex-span"><i>x</i></span>, using the described operation any number of times and sequence <span class="tex-span"><i>a</i></span>.</p><p>Sereja has sequence <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index">|<i>b</i>|</sub></span>. Help Sereja calculate sum: <img align="middle" class="tex-formula" src="file://ao7tkgOD.png" style="max-width: 100.0%;max-height: 100.0%;">. Record <span class="tex-span">[<i>b</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i> + 1</sub>, ..., <i>b</i><sub class="lower-index"><i>j</i></sub>]</span> represents a sequence containing the elements in brackets in the given order. To avoid problems with precision, please, print the required sum divided by <span class="tex-span">|<i>b</i>|<sup class="upper-index">2</sup></span>.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span">|<i>b</i>|</span> <span class="tex-span">(1 ≤ |<i>b</i>| ≤ 3·10<sup class="upper-index">5</sup>)</span> — the length of sequence <span class="tex-span"><i>b</i></span>. The second line contains <span class="tex-span">|<i>b</i>|</span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>b</i><sub class="lower-index">|<i>b</i>|</sub></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>.</p></div><div class="output-specification"><p>In a single line print a real number — the required sum divided by <span class="tex-span">|<i>b</i>|<sup class="upper-index">2</sup></span>. Your answer will be considered correct if its absolute or relative error won't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span">|<i>b</i>|</span> <span class="tex-span">(1 ≤ |<i>b</i>| ≤ 3·10<sup class="upper-index">5</sup>)</span> — the length of sequence <span class="tex-span"><i>b</i></span>. The second line contains <span class="tex-span">|<i>b</i>|</span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>b</i><sub class="lower-index">|<i>b</i>|</sub></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>.</p>

## Output

<p>In a single line print a real number — the required sum divided by <span class="tex-span">|<i>b</i>|<sup class="upper-index">2</sup></span>. Your answer will be considered correct if its absolute or relative error won't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
5
1 2 3 4 1

```




```output1
1.238750000000000

```


