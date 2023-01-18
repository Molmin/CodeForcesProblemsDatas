## Description

<div><p>At the children's day, the child came to Picks's house, and messed his house up. Picks was angry at him. A lot of important things were lost, in particular the favorite set of Picks.</p><p>Fortunately, Picks remembers something about his set <span class="tex-span"><i>S</i></span>:</p><ul> <li> its elements were distinct integers from <span class="tex-span">1</span> to <span class="tex-span"><i>limit</i></span>; </li><li> the value of <img align="middle" class="tex-formula" src="file://sFN8kd7p.png" style="max-width: 100.0%;max-height: 100.0%;"> was equal to <span class="tex-span"><i>sum</i></span>; here <span class="tex-span"><i>lowbit</i>(<i>x</i>)</span> equals <span class="tex-span">2<sup class="upper-index"><i>k</i></sup></span> where <span class="tex-span"><i>k</i></span> is the position of the first one in the binary representation of <span class="tex-span"><i>x</i></span>. For example, <span class="tex-span"><i>lowbit</i>(10010<sub class="lower-index">2</sub>) = 10<sub class="lower-index">2</sub>, <i>lowbit</i>(10001<sub class="lower-index">2</sub>) = 1<sub class="lower-index">2</sub>, <i>lowbit</i>(10000<sub class="lower-index">2</sub>) = 10000<sub class="lower-index">2</sub></span> (binary representation). </li></ul><p>Can you help Picks and find any set <span class="tex-span"><i>S</i></span>, that satisfies all the above conditions?</p></div><div class="input-specification"><p>The first line contains two integers: <span class="tex-span"><i>sum</i>, <i>limit</i></span> <span class="tex-span">(1 ≤ <i>sum</i>, <i>limit</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p></div><div class="output-specification"><p>In the first line print an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>, denoting the size of <span class="tex-span"><i>S</i></span>. Then print the elements of set <span class="tex-span"><i>S</i></span> in any order. If there are multiple answers, print any of them.</p><p>If it's impossible to find a suitable set, print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains two integers: <span class="tex-span"><i>sum</i>, <i>limit</i></span> <span class="tex-span">(1 ≤ <i>sum</i>, <i>limit</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p>

## Output

<p>In the first line print an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>, denoting the size of <span class="tex-span"><i>S</i></span>. Then print the elements of set <span class="tex-span"><i>S</i></span> in any order. If there are multiple answers, print any of them.</p><p>If it's impossible to find a suitable set, print <span class="tex-font-style-tt">-1</span>.</p>





```input1
5 5

```




```input2
4 3

```




```input3
5 1

```




```output1
2
4 5

```




```output2
3
2 3 1

```




```output3
-1

```



## Note

<p>In sample test 1: <span class="tex-span"><i>lowbit</i>(4) = 4, <i>lowbit</i>(5) = 1, 4 + 1 = 5</span>.</p><p>In sample test 2: <span class="tex-span"><i>lowbit</i>(1) = 1, <i>lowbit</i>(2) = 2, <i>lowbit</i>(3) = 1, 1 + 2 + 1 = 4</span>.</p>
