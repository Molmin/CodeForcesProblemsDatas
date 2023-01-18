## Description

<div><p>Little Artem is given a graph, constructed as follows: start with some <span class="tex-span"><i>k</i></span>-clique, then add new vertices one by one, connecting them to <span class="tex-span"><i>k</i></span> already existing vertices that form a <span class="tex-span"><i>k</i></span>-clique.</p><p>Artem wants to count the number of spanning trees in this graph modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>First line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>min</i>(<i>n</i>, 5)</span>)&nbsp;— the total size of the graph and the size of the initial clique, respectively.</p><p>Next <span class="tex-span"><i>n</i> - <i>k</i></span> lines describe <span class="tex-span"><i>k</i> + 1</span>-th, <span class="tex-span"><i>k</i> + 2</span>-th, ..., <span class="tex-span"><i>i</i></span>-th, ..., <span class="tex-span"><i>n</i></span>-th vertices by listing <span class="tex-span"><i>k</i></span> distinct vertex indices <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> &lt; <i>i</i></span> it is connected to. It is guaranteed that those vertices form a k-clique.</p></div><div class="output-specification"><p>Output a single integer&nbsp;— the number of spanning trees in the given graph modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>First line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>min</i>(<i>n</i>, 5)</span>)&nbsp;— the total size of the graph and the size of the initial clique, respectively.</p><p>Next <span class="tex-span"><i>n</i> - <i>k</i></span> lines describe <span class="tex-span"><i>k</i> + 1</span>-th, <span class="tex-span"><i>k</i> + 2</span>-th, ..., <span class="tex-span"><i>i</i></span>-th, ..., <span class="tex-span"><i>n</i></span>-th vertices by listing <span class="tex-span"><i>k</i></span> distinct vertex indices <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> &lt; <i>i</i></span> it is connected to. It is guaranteed that those vertices form a k-clique.</p>

## Output

<p>Output a single integer&nbsp;— the number of spanning trees in the given graph modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
3 2
1 2

```




```input2
4 3
1 2 3

```




```output1
3

```




```output2
16

```


