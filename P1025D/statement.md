## Description

<div><p>Dima the hamster enjoys nibbling different things: cages, sticks, bad problemsetters and even trees!</p><p>Recently he found a binary search tree and instinctively nibbled all of its edges, hence messing up the vertices. Dima knows that if Andrew, who has been thoroughly assembling the tree for a long time, comes home and sees his creation demolished, he'll get extremely upset. </p><p>To not let that happen, Dima has to recover the binary search tree. Luckily, he noticed that any two vertices connected by a direct edge had their greatest common divisor value exceed $1$.</p><p>Help Dima construct such a <span class="tex-font-style-bf">binary search tree</span> or determine that it's impossible. The definition and properties of a binary search tree can be found <a href="https://en.wikipedia.org/wiki/Binary_search_tree">here.</a></p></div><div class="input-specification"><p>The first line contains the number of vertices $n$ ($2 \le n \le 700$).</p><p>The second line features $n$ distinct integers $a_i$ ($2 \le a_i \le 10^9$)&nbsp;— the values of vertices <span class="tex-font-style-bf">in ascending order</span>.</p></div><div class="output-specification"><p>If it is possible to reassemble the binary search tree, such that the greatest common divisor of any two vertices connected by the edge is greater than $1$, print "<span class="tex-font-style-tt">Yes</span>" (quotes for clarity).</p><p>Otherwise, print "<span class="tex-font-style-tt">No</span>" (quotes for clarity).</p></div>

## Input

<p>The first line contains the number of vertices $n$ ($2 \le n \le 700$).</p><p>The second line features $n$ distinct integers $a_i$ ($2 \le a_i \le 10^9$)&nbsp;— the values of vertices <span class="tex-font-style-bf">in ascending order</span>.</p>

## Output

<p>If it is possible to reassemble the binary search tree, such that the greatest common divisor of any two vertices connected by the edge is greater than $1$, print "<span class="tex-font-style-tt">Yes</span>" (quotes for clarity).</p><p>Otherwise, print "<span class="tex-font-style-tt">No</span>" (quotes for clarity).</p>





```input1
6
3 6 9 18 36 108

```




```input2
2
7 17

```




```input3
9
4 8 10 12 15 18 33 44 81

```




```output1
Yes

```




```output2
No

```




```output3
Yes

```



## Note

<p>The picture below illustrates one of the possible trees for the first example.</p><center> <img class="tex-graphics" src="file://tYIJJqgA.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The picture below illustrates one of the possible trees for the third example.</p><center> <img class="tex-graphics" src="file://HjaM2fYk.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
