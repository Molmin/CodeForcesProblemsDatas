## Description

<div><p>You are given two lists of non-zero digits.</p><p>Let's call an integer pretty if its (base <span class="tex-span">10</span>) representation has at least one digit from the first list and at least one digit from the second list. What is the smallest positive pretty integer?</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 9</span>) — the lengths of the first and the second lists, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> distinct digits <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 9</span>) — the elements of the first list.</p><p>The third line contains <span class="tex-span"><i>m</i></span> distinct digits <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 9</span>) — the elements of the second list.</p></div><div class="output-specification"><p>Print the smallest pretty integer.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 9</span>) — the lengths of the first and the second lists, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> distinct digits <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 9</span>) — the elements of the first list.</p><p>The third line contains <span class="tex-span"><i>m</i></span> distinct digits <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 9</span>) — the elements of the second list.</p>

## Output

<p>Print the smallest pretty integer.</p>





```input1
2 3
4 2
5 7 6

```




```input2
8 8
1 2 3 4 5 6 7 8
8 7 6 5 4 3 2 1

```




```output1
25

```




```output2
1

```



## Note

<p>In the first example <span class="tex-span">25</span>, <span class="tex-span">46</span>, <span class="tex-span">24567</span> are pretty, as well as many other integers. The smallest among them is <span class="tex-span">25</span>. <span class="tex-span">42</span> and <span class="tex-span">24</span> are not pretty because they don't have digits from the second list.</p><p>In the second example all integers that have at least one digit different from <span class="tex-span">9</span> are pretty. It's obvious that the smallest among them is <span class="tex-span">1</span>, because it's the smallest positive integer.</p>
