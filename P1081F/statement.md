## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem.</span></p><p>Chouti was tired of studying, so he opened the computer and started playing a puzzle game.</p><p>Long long ago, the boy found a sequence $s_1, s_2, \ldots, s_n$ of length $n$, kept by a tricky interactor. It consisted of $0$s and $1$s only and the number of $1$s is $t$. The boy knows nothing about this sequence except $n$ and $t$, but he can try to find it out with some queries with the interactor.</p><p>We define an operation called flipping. Flipping $[l,r]$ ($1 \leq l \leq r \leq n$) means for each $x \in [l,r]$, changing $s_x$ to $1-s_x$.</p><p>In each query, the boy can give the interactor two integers $l,r$ satisfying $1 \leq l \leq r \leq n$ and the interactor will either flip $[1,r]$ or $[l,n]$ (both outcomes have the same probability and all decisions made by interactor are independent from each other, see <span class="tex-font-style-tt">Notes</span> section for more details). The interactor will tell the current number of $1$s after each operation. Note, that the sequence <span class="tex-font-style-bf">won't be restored</span> after each operation.</p><p>Help the boy to find the <span class="tex-font-style-bf">original</span> sequence in no more than $10000$ interactions.</p><p>"Weird legend, dumb game." he thought. However, after several tries, he is still stuck with it. Can you help him beat this game?</p></div><div><h2>Interaction</h2><p>The interaction starts with a line containing two integers $n$ and $t$ ($1 \leq n \leq 300$, $0 \leq t \leq n$)&nbsp;— the length of the sequence and the number of $1$s in it.</p><p>After that, you can make queries.</p><p>To make a query, print a line "<span class="tex-font-style-tt">? l r</span>" ($1 \leq l \leq r \leq n$), then <span class="tex-font-style-tt">flush</span> the output.</p><p>After each query, read a single integer $t$ ($-1 \leq t \leq n$).</p><ul><li> If $t=-1$, it means that you're out of queries, you should terminate your program immediately, then you will get <span class="tex-font-style-tt">Wrong Answer</span>, otherwise the judging result would be undefined because you will interact with a closed stream.</li><li> If $t \geq 0$, it represents the current number of $1$s in the sequence.</li></ul><p>When you found the original sequence, print a line "<span class="tex-font-style-tt">! s</span>", <span class="tex-font-style-tt">flush</span> the output and terminate. Print $s_1, s_2, \ldots, s_n$ as a binary string and do not print spaces in between.</p><p>Your solution will get <span class="tex-font-style-tt">Idleness Limit Exceeded</span> if you don't print anything or forget to flush the output.</p><p>To <span class="tex-font-style-tt">flush</span> you need to do the following right after printing a query and a line end: </p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see documentation for other languages. </li></ul><p><span class="tex-font-style-bf">Hacks</span></p><p>For hacks, use the following format:</p><p>In the first and only line, print a non-empty binary string. Its length will be $n$ and it will be treated as $s_1, s_2, \ldots, s_n$.</p><p>For example, the the test corresponding to the example contains a line "<span class="tex-font-style-tt">0011</span>".</p></div>





```input1
4 2
2
2
0
```




```output1
? 1 1
? 1 1
? 3 4
! 0011
```



## Note

<p>For first query $1,1$, the interactor should flip $[1,1]$ or $[1,4]$. It chose to flip $[1,4]$, so the sequence became <span class="tex-font-style-tt">1100</span>.</p><p>For second query $1,1$, the interactor should flip $[1,1]$ or $[1,4]$. It again chose to flip $[1,4]$, so the sequence became <span class="tex-font-style-tt">0011</span>.</p><p>For third query $3,4$, the interactor should flip $[1,4]$ or $[3,4]$. It chose to flip $[3,4]$, so the sequence became <span class="tex-font-style-tt">0000</span>.</p><p>Q: How does interactor choose between $[1,r]$ and $[l,n]$? Is it really random?</p><p>A: The interactor will use a <span class="tex-font-style-bf">secret</span> <a href="https://en.wikipedia.org/wiki/Pseudorandom_number_generator">pseudorandom number generator</a>. Only $s$ and your queries will be hashed and used as the seed. So if you give the same sequence of queries twice for the same secret string, you will get the same results. Except this, you can consider the choices fully random, like flipping a fair coin. <span class="tex-font-style-bf">You needn't (and shouldn't) exploit the exact generator to pass this problem.</span></p>
