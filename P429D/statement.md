## Description

<div><p>Iahub and Sorin are the best competitive programmers in their town. However, they can't both qualify to an important contest. The selection will be made with the help of a single problem. Blatnatalag, a friend of Iahub, managed to get hold of the problem before the contest. Because he wants to make sure Iahub will be the one qualified, he tells Iahub the following task.</p><p>You're given an (1-based) array <span class="tex-span"><i>a</i></span> with <span class="tex-span"><i>n</i></span> elements. Let's define function <span class="tex-span"><i>f</i>(<i>i</i>, <i>j</i>)</span> <span class="tex-span">(1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i>)</span> as <span class="tex-span">(<i>i</i> - <i>j</i>)<sup class="upper-index">2</sup> + <i>g</i>(<i>i</i>, <i>j</i>)<sup class="upper-index">2</sup></span>. Function g is calculated by the following pseudo-code:</p><pre class="verbatim"><br>int g(int i, int j) {<br>    int sum = 0;<br>    for (int k = min(i, j) + 1; k &lt;= max(i, j); k = k + 1)<br>        sum = sum + a[k];<br>    return sum;<br>}<br></pre><p>Find a value <span class="tex-span"><i>min</i><sub class="lower-index"><i>i</i> ≠ <i>j</i></sub>&nbsp;&nbsp;<i>f</i>(<i>i</i>, <i>j</i>)</span>.</p><p>Probably by now Iahub already figured out the solution to this problem. Can you?</p></div><div class="input-specification"><p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100000</span>). Next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i>[1]</span>, <span class="tex-span"><i>a</i>[2]</span>, ..., <span class="tex-span"><i>a</i>[<i>n</i>]</span> (<span class="tex-span"> - 10<sup class="upper-index">4</sup> ≤ <i>a</i>[<i>i</i>] ≤ 10<sup class="upper-index">4</sup></span>). </p></div><div class="output-specification"><p>Output a single integer — the value of <span class="tex-span"><i>min</i><sub class="lower-index"><i>i</i> ≠ <i>j</i></sub>&nbsp;&nbsp;<i>f</i>(<i>i</i>, <i>j</i>)</span>.</p></div>

## Input

<p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100000</span>). Next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i>[1]</span>, <span class="tex-span"><i>a</i>[2]</span>, ..., <span class="tex-span"><i>a</i>[<i>n</i>]</span> (<span class="tex-span"> - 10<sup class="upper-index">4</sup> ≤ <i>a</i>[<i>i</i>] ≤ 10<sup class="upper-index">4</sup></span>). </p>

## Output

<p>Output a single integer — the value of <span class="tex-span"><i>min</i><sub class="lower-index"><i>i</i> ≠ <i>j</i></sub>&nbsp;&nbsp;<i>f</i>(<i>i</i>, <i>j</i>)</span>.</p>





```input1
4
1 0 0 -1

```




```input2
2
1 -1

```




```output1
1

```




```output2
2

```


