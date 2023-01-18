## Description

<div><p><span class="tex-font-style-bf">This problem is interactive</span>.</p><p>We have hidden an array $a$ of $n$ <span class="tex-font-style-bf">pairwise different</span> numbers (this means that no two numbers are equal). You can get some information about this array using a new device you just ordered on Amazon. </p><p>This device can answer queries of the following form: in response to the positions of $k$ different elements of the array, it will return the position and value of the $m$-th among them in the ascending order.</p><p>Unfortunately, the instruction for the device was lost during delivery. However, you remember $k$, but don't remember $m$. Your task is to find $m$ using queries to this device. </p><p>You can ask <span class="tex-font-style-bf">not more than $n$ queries</span>.</p><p>Note that the array $a$ and number $m$ are fixed before the start of the interaction and don't depend on your queries. In other words, <span class="tex-font-style-bf">interactor is not adaptive</span>.</p><p>Note that you don't have to minimize the number of queries, and you don't need to guess array $a$. You just have to guess $m$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1\le k &lt; n \le 500$)&nbsp;— the length of the array and the number of the elements in the query.</p><p>It is guaranteed that number $m$ satisfies $1\le m \le k$, elements $a_1, a_2, \dots, a_n$ of the array satisfy $0\le a_i \le 10^9$, and all of them are different.</p></div><div><h2>Interaction</h2><p>You begin the interaction by reading $n$ and $k$.</p><p>To ask a question about elements on positions $x_1, x_2, \dots, x_k$, in a separate line output</p><p>$?$ $x_1$ $x_2$ $x_3$ ... $x_k$</p><p>Numbers in the query have to satisfy $1 \le x_i \le n$, and all $x_i$ have to be different. Don't forget to 'flush', to get the answer.</p><p>In response, you will receive two integers $pos$ and $a_{pos}$&nbsp;— the position in the array $a$ of the $m$-th in ascending order element among $a_{x_1}, a_{x_2}, \dots, a_{x_k}$, and the element on this position.</p><p>In case your query is invalid or you asked more than $n$ queries, the program will print $-1$ and will finish interaction. You will receive a <span class="tex-font-style-bf">Wrong answer</span> verdict. Make sure to exit immediately to avoid getting other verdicts.</p><p>When you determine $m$, output </p><p>$!$ $m$</p><p>After printing a query do not forget to output end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul><li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++;</li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java;</li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal;</li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python;</li><li> see documentation for other languages.</li></ul><p><span class="tex-font-style-bf">Hack format</span></p><p>For the hacks use the following format:</p><p>The first line has to contain three integers $n, k, m$ ($1 \le m \le k &lt; n \le 500$)&nbsp;— the length of the array, number of elements in the query, and which in the ascending order number the device returns.</p><p>In the next line output $n$ integers $a_1, a_2, \dots, a_n$ ($0\le a_i \le 10^9$)&nbsp;— the elements of the array. They have to be pairwise different.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1\le k &lt; n \le 500$)&nbsp;— the length of the array and the number of the elements in the query.</p><p>It is guaranteed that number $m$ satisfies $1\le m \le k$, elements $a_1, a_2, \dots, a_n$ of the array satisfy $0\le a_i \le 10^9$, and all of them are different.</p>





```input1
4 3
4 9
4 9
4 9
1 2
```




```output1
? 2 3 4
? 1 3 4
? 1 2 4
? 1 2 3
! 3
```



## Note

<p>In the example, $n = 4$, $k = 3$, $m = 3$, $a = [2, 0, 1, 9]$.</p>
