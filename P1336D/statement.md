## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem.</span></p><p>Yui is a girl who enjoys playing Mahjong.</p><center><img class="tex-graphics" src="file://OT5TSl8x.png" style="max-width: 100.0%;max-height: 100.0%;"></center>&nbsp;<p>She has a mysterious set which consists of tiles (this set can be empty). Each tile has an integer value between $1$ and $n$, and <span class="tex-font-style-bf">at most $n$ tiles</span> in the set have the same value. So the set can contain at most $n^2$ tiles.</p><p>You want to figure out which values are on the tiles. But Yui is shy, she prefers to play a guessing game with you.</p><p>Let's call a set consisting of <span class="tex-font-style-bf">three</span> tiles <span class="tex-font-style-it">triplet</span> if their values are the same. For example, $\{2,\,2,\,2\}$ is a triplet, but $\{2,\,3,\,3\}$ is not.</p><p>Let's call a set consisting of <span class="tex-font-style-bf">three</span> tiles <span class="tex-font-style-it">straight</span> if their values are consecutive integers. For example, $\{2,\,3,\,4\}$ is a straight, but $\{1,\,3,\,5\}$ is not.</p><p>At first, Yui gives you the number of triplet subsets and straight subsets of the initial set respectively. After that, you can insert a tile with an integer value between $1$ and $n$ into the set <span class="tex-font-style-bf">at most $n$ times</span>. Every time you insert a tile, you will get the number of triplet subsets and straight subsets of the current set as well.</p><p>Note that two tiles with the same value are treated different. In other words, in the set $\{1,\,1,\,2,\,2,\,3\}$ you can find $4$ subsets $\{1,\,2,\,3\}$.</p><p>Try to guess the number of tiles in the initial set with value $i$ for all integers $i$ from $1$ to $n$.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($4 \le n \le 100$).</p><p>The second line contains two integers which represent the number of triplet subsets and straight subsets of the initial set respectively.</p></div><div class="output-specification"><p>When you are ready to answer, print a single line of form "<span class="tex-font-style-tt">! $a_1$ $a_2$ $\ldots$ $a_n$</span>" ($0 \le a_i \le n$), where $a_i$ is equal to the number of tiles in the initial set with value $i$.</p></div><div><h2>Interaction</h2><p>To insert a tile, print a single line of form "<span class="tex-font-style-tt">+ $x$</span>" ($1 \le x \le n$), where $x$ is the value of the tile you insert. Then you should read two integers which represent the number of triplet subsets and straight subsets of the current set respectively.</p><p>After printing a line, do not forget to flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see documentation for other languages. </li></ul><p>You will get <span class="tex-font-style-tt">Wrong answer</span> if you insert more than $n$ tiles.</p><p><span class="tex-font-style-bf">Hacks</span></p><p>To make a hack you should provide a test in such format:</p><p>The first line contains a single integer $n$ ($4 \le n \le 100$).</p><p>The second line contains $n$ integers $a_1,a_2,\ldots,a_n$ ($0 \le a_i \le n$) &nbsp;— $a_i$ is equal to the number of tiles with value $i$ in the set.</p></div>

## Input

<p>The first line contains a single integer $n$ ($4 \le n \le 100$).</p><p>The second line contains two integers which represent the number of triplet subsets and straight subsets of the initial set respectively.</p>

## Output

<p>When you are ready to answer, print a single line of form "<span class="tex-font-style-tt">! $a_1$ $a_2$ $\ldots$ $a_n$</span>" ($0 \le a_i \le n$), where $a_i$ is equal to the number of tiles in the initial set with value $i$.</p>





```input1
5
1 6
2 9
5 12
5 24
6 24
```




```output1
+ 1
+ 1
+ 2
+ 5
! 2 1 3 0 2
```



## Note

<p>In the first test, the initial set of tiles is $\{1, 1, 2, 3, 3, 3, 5, 5\}$. It has only one triplet subset $\{3, 3, 3\}$ and six straight subsets, all equal to $\{1, 2, 3\}$. After inserting a tile with value $1$ the set of tiles will be $\{1, 1, 1, 2, 3, 3, 3, 5, 5\}$ and will have two triplet subsets $\{1, 1, 1\}$, $\{3, 3, 3\}$ and nine straight subsets, all equal to $\{1, 2, 3\}$.</p>
