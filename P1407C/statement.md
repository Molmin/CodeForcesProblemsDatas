## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem.</span></p><p>We hid from you a permutation $p$ of length $n$, consisting of the elements from $1$ to $n$. You want to guess it. To do that, you can give us 2 different indices $i$ and $j$, and we will reply with $p_{i} \bmod p_{j}$ (remainder of division $p_{i}$ by $p_{j}$).</p><p>We have enough patience to answer at most $2 \cdot n$ queries, so you should fit in this constraint. Can you do it?</p><p>As a reminder, a permutation of length $n$ is an array consisting of $n$ distinct integers from $1$ to $n$ in arbitrary order. For example, $[2,3,1,5,4]$ is a permutation, but $[1,2,2]$ is not a permutation ($2$ appears twice in the array) and $[1,3,4]$ is also not a permutation ($n=3$ but there is $4$ in the array).</p></div><div class="input-specification"><p>The only line of the input contains a single integer $n$ ($1 \le n \le 10^4$) — length of the permutation.</p></div><div><h2>Interaction</h2><p>The interaction starts with reading $n$. </p><p>Then you are allowed to make at most $2 \cdot n$ queries in the following way: </p><ul> <li> "<span class="tex-font-style-tt">? x y</span>" ($1 \le x, y \le n, x \ne y$). </li></ul><p>After each one, you should read an integer $k$, that equals $p_x \bmod p_y$. </p><p>When you have guessed the permutation, print a single line "<span class="tex-font-style-tt">! </span>" (without quotes), followed by array $p$ and quit.</p><p>After printing a query do not forget to output end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul><li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++;</li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java;</li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal;</li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python;</li><li> see documentation for other languages.</li></ul><p>Exit immediately after receiving "<span class="tex-font-style-tt">-1</span>" and you will see <span class="tex-font-style-tt">Wrong answer</span> verdict. Otherwise you can get an arbitrary verdict because your solution will continue to read from a closed stream.</p><p><span class="tex-font-style-bf">Hack format</span></p><p>In the first line output $n$ ($1 \le n \le 10^4$). In the second line print the permutation of $n$ integers $p_1, p_2, \ldots, p_n$.</p></div>

## Input

<p>The only line of the input contains a single integer $n$ ($1 \le n \le 10^4$) — length of the permutation.</p>





```input1
3

1

2

1

0
```




```output1
? 1 2

? 3 2

? 1 3

? 2 1

! 1 3 2
```


