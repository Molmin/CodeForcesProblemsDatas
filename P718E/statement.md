## Description

<div><p>Today is Matvey's birthday. He never knows what to ask as a present so friends gave him a string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span>. This string consists of only first eight English letters: '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>', <span class="tex-span">...</span>, '<span class="tex-font-style-tt">h</span>'.</p><p>First question that comes to mind is: who might ever need some string? Matvey is a special boy so he instantly found what to do with this string. He used it to build an undirected graph where vertices correspond to position in the string and there is an edge between distinct positions <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>) if <span class="tex-font-style-bf">at least one</span> of the following conditions hold: </p><ol> <li> <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are neighbouring, i.e. <span class="tex-span">|<i>a</i> - <i>b</i>| = 1</span>. </li><li> Positions <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> contain equal characters, i.e. <span class="tex-span"><i>s</i><sub class="lower-index"><i>a</i></sub> = <i>s</i><sub class="lower-index"><i>b</i></sub></span>. </li></ol><p>Then Matvey decided to find the diameter of this graph. Diameter is a maximum distance (length of the shortest path) among all pairs of vertices. Also, Matvey wants to find the number of pairs of vertices such that the distance between them is equal to the diameter of the graph. As he is very cool and experienced programmer he managed to solve this problem very fast. Will you do the same?</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the length of the string.</p><p>The second line contains the string <span class="tex-span"><i>s</i></span> itself. It's guaranteed that <span class="tex-span"><i>s</i></span> consists of only first eight letters of English alphabet.</p></div><div class="output-specification"><p>Print two integers&nbsp;— the diameter of the graph and the number of pairs of positions with the distance equal to the diameter.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the length of the string.</p><p>The second line contains the string <span class="tex-span"><i>s</i></span> itself. It's guaranteed that <span class="tex-span"><i>s</i></span> consists of only first eight letters of English alphabet.</p>

## Output

<p>Print two integers&nbsp;— the diameter of the graph and the number of pairs of positions with the distance equal to the diameter.</p>





```input1
3
abc

```




```input2
7
aaabaaa

```




```output1
2 1

```




```output2
2 4

```



## Note

<p>Consider the second sample. </p><p>The maximum distance is <span class="tex-span">2</span>. It's obtained for pairs <span class="tex-span">(1, 4)</span>, <span class="tex-span">(2, 4)</span>, <span class="tex-span">(4, 6)</span> and <span class="tex-span">(4, 7)</span>.</p>
