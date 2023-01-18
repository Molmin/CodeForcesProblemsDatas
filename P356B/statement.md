## Description

<div><p>Xenia is an amateur programmer. Today on the IT lesson she learned about the Hamming distance.</p><p>The Hamming distance between two strings <span class="tex-span"><i>s</i> = <i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index"><i>n</i></sub></span> and <span class="tex-span"><i>t</i> = <i>t</i><sub class="lower-index">1</sub><i>t</i><sub class="lower-index">2</sub>... <i>t</i><sub class="lower-index"><i>n</i></sub></span> of equal length <span class="tex-span"><i>n</i></span> is value <img align="middle" class="tex-formula" src="file://S6QR1SwO.png" style="max-width: 100.0%;max-height: 100.0%;">. Record <span class="tex-span">[<i>s</i><sub class="lower-index"><i>i</i></sub> ≠ <i>t</i><sub class="lower-index"><i>i</i></sub>]</span> is the Iverson notation and represents the following: if <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> ≠ <i>t</i><sub class="lower-index"><i>i</i></sub></span>, it is one, otherwise — zero.</p><p>Now Xenia wants to calculate the Hamming distance between two long strings <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. The first string <span class="tex-span"><i>a</i></span> is the concatenation of <span class="tex-span"><i>n</i></span> copies of string <span class="tex-span"><i>x</i></span>, that is, <img align="middle" class="tex-formula" src="file://9TUI0JrP.png" style="max-width: 100.0%;max-height: 100.0%;">. The second string <span class="tex-span"><i>b</i></span> is the concatenation of <span class="tex-span"><i>m</i></span> copies of string <span class="tex-span"><i>y</i></span>. </p><p>Help Xenia, calculate the required Hamming distance, given <span class="tex-span"><i>n</i>, <i>x</i>, <i>m</i>, <i>y</i></span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">12</sup>)</span>. The second line contains a non-empty string <span class="tex-span"><i>x</i></span>. The third line contains a non-empty string <span class="tex-span"><i>y</i></span>. Both strings consist of at most <span class="tex-span">10<sup class="upper-index">6</sup></span> lowercase English letters.</p><p>It is guaranteed that strings <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> that you obtain from the input have the same length.</p></div><div class="output-specification"><p>Print a single integer — the required Hamming distance.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">12</sup>)</span>. The second line contains a non-empty string <span class="tex-span"><i>x</i></span>. The third line contains a non-empty string <span class="tex-span"><i>y</i></span>. Both strings consist of at most <span class="tex-span">10<sup class="upper-index">6</sup></span> lowercase English letters.</p><p>It is guaranteed that strings <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> that you obtain from the input have the same length.</p>

## Output

<p>Print a single integer — the required Hamming distance.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
100 10
a
aaaaaaaaaa

```




```input2
1 1
abacaba
abzczzz

```




```input3
2 3
rzr
az

```




```output1
0

```




```output2
4

```




```output3
5

```



## Note

<p>In the first test case string <span class="tex-span"><i>a</i></span> is the same as string <span class="tex-span"><i>b</i></span> and equals 100 letters <span class="tex-font-style-tt">a</span>. As both strings are equal, the Hamming distance between them is zero.</p><p>In the second test case strings <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> differ in their 3-rd, 5-th, 6-th and 7-th characters. Thus, the Hamming distance equals 4.</p><p>In the third test case string <span class="tex-span"><i>a</i></span> is <span class="tex-font-style-tt">rzrrzr</span> and string <span class="tex-span"><i>b</i></span> is <span class="tex-font-style-tt">azazaz</span>. The strings differ in all characters apart for the second one, the Hamming distance between them equals 5.</p>
