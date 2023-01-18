## Description

<div><p>You have multiset of <span class="tex-span"><i>n</i></span> strings of the same length, consisting of lowercase English letters. We will say that those strings are easy to remember if for each string there is some position <span class="tex-span"><i>i</i></span> and some letter <span class="tex-span"><i>c</i></span> of the English alphabet, such that this string is the only string in the multiset that has letter <span class="tex-span"><i>c</i></span> in position <span class="tex-span"><i>i</i></span>.</p><p>For example, a multiset of strings {"abc", "aba", "adc", "ada"} are not easy to remember. And multiset {"abc", "ada", "ssa"} is easy to remember because: </p><ul> <li> the first string is the only string that has character <span class="tex-span"><i>c</i></span> in position <span class="tex-span">3</span>; </li><li> the second string is the only string that has character <span class="tex-span"><i>d</i></span> in position <span class="tex-span">2</span>; </li><li> the third string is the only string that has character <span class="tex-span"><i>s</i></span> in position <span class="tex-span">2</span>. </li></ul><p>You want to change your multiset a little so that it is easy to remember. For <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> coins, you can change character in the <span class="tex-span"><i>j</i></span>-th position of the <span class="tex-span"><i>i</i></span>-th string into any other lowercase letter of the English alphabet. Find what is the minimum sum you should pay in order to make the multiset of strings easy to remember.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 20</span>)&nbsp;— the number of strings in the multiset and the length of the strings respectively. Next <span class="tex-span"><i>n</i></span> lines contain the strings of the multiset, consisting only of lowercase English letters, each string's length is <span class="tex-span"><i>m</i></span>.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> integers each, the <span class="tex-span"><i>i</i></span>-th of them contains integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>1</sub>, <i>a</i><sub class="lower-index"><i>i</i>2</sub>, ..., <i>a</i><sub class="lower-index"><i>im</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 10<sup class="upper-index">6</sup></span>).</p></div><div class="output-specification"><p>Print a single number — the answer to the problem.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 20</span>)&nbsp;— the number of strings in the multiset and the length of the strings respectively. Next <span class="tex-span"><i>n</i></span> lines contain the strings of the multiset, consisting only of lowercase English letters, each string's length is <span class="tex-span"><i>m</i></span>.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> integers each, the <span class="tex-span"><i>i</i></span>-th of them contains integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>1</sub>, <i>a</i><sub class="lower-index"><i>i</i>2</sub>, ..., <i>a</i><sub class="lower-index"><i>im</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 10<sup class="upper-index">6</sup></span>).</p>

## Output

<p>Print a single number — the answer to the problem.</p>





```input1
4 5
abcde
abcde
abcde
abcde
1 1 1 1 1
1 1 1 1 1
1 1 1 1 1
1 1 1 1 1

```




```input2
4 3
abc
aba
adc
ada
10 10 10
10 1 10
10 10 10
10 1 10

```




```input3
3 3
abc
ada
ssa
1 1 1
1 1 1
1 1 1

```




```output1
3

```




```output2
2

```




```output3
0

```


