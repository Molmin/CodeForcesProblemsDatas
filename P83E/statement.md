## Description

<div><p>On an IT lesson Valera studied data compression. The teacher told about a new method, which we shall now describe to you.</p><p>Let <span class="tex-span">{<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>}</span> be the given sequence of lines needed to be compressed. Here and below we shall assume that all lines are <span class="tex-font-style-bf">of the same length</span> and consist only of the digits <span class="tex-span">0</span> and <span class="tex-span">1</span>. Let's define the compression function:</p><ul> <li> <span class="tex-span"><i>f</i>(</span>empty sequence<span class="tex-span">) = </span>empty string </li><li> <span class="tex-span"><i>f</i>(<i>s</i>) = <i>s</i></span>. </li><li> <span class="tex-span"><i>f</i>(<i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>) = </span> the smallest in length string, which has one of the prefixes equal to <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and one of the suffixes equal to <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span>. For example, <span class="tex-span"><i>f</i>(001, 011) = 0011</span>, <span class="tex-span"><i>f</i>(111, 011) = 111011</span>. </li><li> <span class="tex-span"><i>f</i>(<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>) = <i>f</i>(<i>f</i>(<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index"><i>n</i> - 1</sub>), <i>a</i><sub class="lower-index"><i>n</i></sub>)</span>. For example, <span class="tex-span"><i>f</i>(000, 000, 111) = <i>f</i>(<i>f</i>(000, 000), 111) = <i>f</i>(000, 111) = 000111</span>. </li></ul><p>Valera faces a real challenge: he should divide the given sequence <span class="tex-span">{<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>}</span> into two subsequences <span class="tex-span">{<i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>k</i></sub>}</span> and <span class="tex-span">{<i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>m</i></sub>}</span>, <span class="tex-span"><i>m</i> + <i>k</i> = <i>n</i></span>, so that the value of <span class="tex-span"><i>S</i> = |<i>f</i>(<i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>k</i></sub>)| + |<i>f</i>(<i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>m</i></sub>)|</span> took the minimum possible value. Here <span class="tex-span">|<i>p</i>|</span> denotes the length of the string <span class="tex-span"><i>p</i></span>.</p><p>Note that it is not allowed to change the relative order of lines in the subsequences. It is allowed to make one of the subsequences empty. Each string from the initial sequence should belong to exactly one subsequence. Elements of subsequences <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> don't have to be consecutive in the original sequence <span class="tex-span"><i>a</i></span>, i. e. elements of <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> can alternate in <span class="tex-span"><i>a</i></span> (see samples 2 and 3).</p><p>Help Valera to find the minimum possible value of <span class="tex-span"><i>S</i></span>.</p></div><div class="input-specification"><p>The first line of input data contains an integer <span class="tex-span"><i>n</i></span> — the number of strings (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>). Then on <span class="tex-span"><i>n</i></span> lines follow elements of the sequence — strings whose lengths are from <span class="tex-span">1</span> to <span class="tex-span">20</span> characters, consisting only of digits <span class="tex-span">0</span> and <span class="tex-span">1</span>. The <span class="tex-span"><i>i</i> + 1</span>-th input line contains the <span class="tex-span"><i>i</i></span>-th element of the sequence. Elements of the sequence are separated only by a newline. It is guaranteed that all lines have the same length.</p></div><div class="output-specification"><p>Print a single number — the minimum possible value of <span class="tex-span"><i>S</i></span>.</p></div>

## Input

<p>The first line of input data contains an integer <span class="tex-span"><i>n</i></span> — the number of strings (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>). Then on <span class="tex-span"><i>n</i></span> lines follow elements of the sequence — strings whose lengths are from <span class="tex-span">1</span> to <span class="tex-span">20</span> characters, consisting only of digits <span class="tex-span">0</span> and <span class="tex-span">1</span>. The <span class="tex-span"><i>i</i> + 1</span>-th input line contains the <span class="tex-span"><i>i</i></span>-th element of the sequence. Elements of the sequence are separated only by a newline. It is guaranteed that all lines have the same length.</p>

## Output

<p>Print a single number — the minimum possible value of <span class="tex-span"><i>S</i></span>.</p>





```input1
3
01
10
01

```




```input2
4
000
111
110
001

```




```input3
5
10101
01010
11111
01000
10010

```




```output1
4

```




```output2
8

```




```output3
17

```



## Note

<p>Detailed answers to the tests:</p><ul> <li> The best option is to make one of the subsequences empty, and the second one equal to the whole given sequence. <span class="tex-span">|<i>f</i>(01, 10, 01)| = |<i>f</i>(<i>f</i>(01, 10), 01)| = |<i>f</i>(010, 01)| = |0101| = 4</span>. </li><li> The best option is: <span class="tex-span"><i>b</i> = {000, 001}, <i>c</i> = {111, 110}.</span> <span class="tex-span"><i>S</i> = |<i>f</i>(000, 001)| + |<i>f</i>(111, 110)| = |0001| + |1110| = 8</span>. </li><li> The best option is: <span class="tex-span"><i>b</i> = {10101, 01010, 01000}, <i>c</i> = {11111, 10010}.</span> <span class="tex-span"><i>S</i> = |10101000| + |111110010| = 17</span>. </li></ul>
