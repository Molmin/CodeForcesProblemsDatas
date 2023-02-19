## Description

<div><p><span class="tex-font-style-bf">This in an interactive problem</span>.</p><p>There is an unknown tree consisting of $n$ nodes, which has <span class="tex-font-style-bf">exactly one</span> centroid. You only know $n$ at first, and your task is to find the centroid of the tree.</p><p>You can ask the distance between any two vertices for at most $2\cdot10^5$ times. </p><p>Note that the interactor is <span class="tex-font-style-bf">not</span> adaptive. That is, the tree is fixed in each test beforehand and does not depend on your queries.</p><p>A vertex is called a centroid if its removal splits the tree into subtrees with at most $\lfloor\frac{n}{2}\rfloor$ vertices each.</p></div><div class="input-specification"><p>The only line of the input contains an integer $n$ ($3\le n\le 7.5\cdot10^4$)&nbsp;— the number of nodes in the tree.</p></div><div><h2>Interaction</h2><p>Start interaction by reading $n$.</p><p>To ask a query about the distance between two nodes $u, v$ ($1 \le u, v \le n$), output "<span class="tex-font-style-tt">? u v</span>".</p><p>If you determine that the centroid of the tree is $x$, use "<span class="tex-font-style-tt">! x</span>" to report.</p><p>After printing a query, do not forget to output the end of a line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see documentation for other languages. </li></ul><p><span class="tex-font-style-bf">Hacks are disabled in this problem.</span></p><p><span class="tex-font-style-bf">It's guaranteed that there are at most $500$ tests in this problem.</span></p></div>

## Input

<p>The only line of the input contains an integer $n$ ($3\le n\le 7.5\cdot10^4$)&nbsp;— the number of nodes in the tree.</p>





```input1
5

2

1

2

3

1

1

1
```




```output1
? 1 2

? 1 3

? 1 4

? 1 5

? 2 3

? 3 4

? 4 5

! 3
```



## Note

<p>Here is an image of the tree from the sample.</p><center> <img class="tex-graphics" src="file://DnsctPGQ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
