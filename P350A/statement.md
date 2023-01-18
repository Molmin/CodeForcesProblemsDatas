## Description

<div><p>Valera wanted to prepare a Codesecrof round. He's already got one problem and he wants to set a time limit (TL) on it.</p><p>Valera has written <span class="tex-span"><i>n</i></span> correct solutions. For each correct solution, he knows its running time (in seconds). Valera has also wrote <span class="tex-span"><i>m</i></span> wrong solutions and for each wrong solution he knows its running time (in seconds).</p><p>Let's suppose that Valera will set <span class="tex-span"><i>v</i></span> seconds TL in the problem. Then we can say that a solution passes the system testing if its running time is at most <span class="tex-span"><i>v</i></span> seconds. We can also say that a solution passes the system testing with some "extra" time if for its running time, <span class="tex-span"><i>a</i></span> seconds, an inequality <span class="tex-span">2<i>a</i> ≤ <i>v</i></span> holds.</p><p>As a result, Valera decided to set <span class="tex-span"><i>v</i></span> seconds TL, that the following conditions are met:</p><ol> <li> <span class="tex-span"><i>v</i></span> is a positive integer; </li><li> all correct solutions pass the system testing; </li><li> at least one correct solution passes the system testing with some "extra" time; </li><li> all wrong solutions do not pass the system testing; </li><li> value <span class="tex-span"><i>v</i></span> is minimum among all TLs, for which points <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">3</span>, <span class="tex-span">4</span> hold. </li></ol><p>Help Valera and find the most suitable TL or else state that such TL doesn't exist.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>). The second line contains <span class="tex-span"><i>n</i></span> space-separated positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the running time of each of the <span class="tex-span"><i>n</i></span> correct solutions in seconds. The third line contains <span class="tex-span"><i>m</i></span> space-separated positive integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the running time of each of <span class="tex-span"><i>m</i></span> wrong solutions in seconds. </p></div><div class="output-specification"><p>If there is a valid TL value, print it. Otherwise, print -1.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>). The second line contains <span class="tex-span"><i>n</i></span> space-separated positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the running time of each of the <span class="tex-span"><i>n</i></span> correct solutions in seconds. The third line contains <span class="tex-span"><i>m</i></span> space-separated positive integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the running time of each of <span class="tex-span"><i>m</i></span> wrong solutions in seconds. </p>

## Output

<p>If there is a valid TL value, print it. Otherwise, print -1.</p>





```input1
3 6
4 5 2
8 9 6 10 7 11

```




```input2
3 1
3 4 5
6

```




```output1
5
```




```output2
-1

```


