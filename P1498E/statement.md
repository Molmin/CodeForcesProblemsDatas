## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem. Remember to flush your output while communicating with the testing program.</span> You may use <span class="tex-font-style-tt">fflush(stdout)</span> in C++, <span class="tex-font-style-tt">system.out.flush()</span> in Java, <span class="tex-font-style-tt">stdout.flush()</span> in Python or <span class="tex-font-style-tt">flush(output)</span> in Pascal to flush the output. If you use some other programming language, consult its documentation. You may also refer to the guide on interactive problems: <a href="https://codeforces.com/blog/entry/45307">https://codeforces.com/blog/entry/45307</a>.</p><p>There is a city in which Dixit lives. In the city, there are $n$ houses. There is <span class="tex-font-style-bf"> exactly one directed road between every pair of houses.</span> For example, consider two houses A and B, then there is a directed road either from A to B or from B to A but not both. The number of roads leading to the $i$-th house is $k_i$.</p><p>Two houses A and B are <span class="tex-font-style-it">bi-reachable</span> if A is reachable from B <span class="tex-font-style-bf">and</span> B is reachable from A. We say that house B is reachable from house A when there is a path from house A to house B.</p><p>Dixit wants to buy two houses in the city, that is, one for living and one for studying. Of course, he would like to travel from one house to another. So, he wants to find a pair of bi-reachable houses A and B. Among all such pairs, he wants to choose one with the maximum value of $|k_A - k_B|$, where $k_i$ is the number of roads leading to the house $i$. If more than one optimal pair exists, any of them is suitable.</p><p>Since Dixit is busy preparing CodeCraft, can you help him find the desired pair of houses, or tell him that no such houses exist?</p><p>In the problem input, you are <span class="tex-font-style-bf">not</span> given the direction of each road. You are given — for each house — only the number of incoming roads to that house ($k_i$).</p><p>You are allowed to ask only one type of query from the judge: give two houses A and B, and the judge answers whether B is reachable from A. There is <span class="tex-font-style-bf">no upper limit on the number of queries</span>. But, <span class="tex-font-style-bf">you cannot ask more queries after the judge answers "<span class="tex-font-style-tt">Yes</span>" to any of your queries.</span> Also, you cannot ask the same query twice.</p><p>Once you have exhausted all your queries (or the judge responds "<span class="tex-font-style-tt">Yes</span>" to any of your queries), your program must output its guess for the two houses and quit.</p><p>See the Interaction section below for more details.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($3 \le n \le 500$) denoting the number of houses in the city. The next line contains $n$ space-separated integers $k_1, k_2, \dots, k_n$ ($0 \le k_i \le n - 1$), the $i$-th of them represents the number of incoming roads to the $i$-th house.</p></div><div><h2>Interaction</h2><p>To ask a query, print "<span class="tex-font-style-tt">? A B</span>" $(1 \leq A,B \leq N, A\neq B)$. The judge will respond "<span class="tex-font-style-tt">Yes</span>" if house B is reachable from house A, or "<span class="tex-font-style-tt">No</span>" otherwise.</p><p>To output the final answer, print "<span class="tex-font-style-tt">! A B</span>", where A and B are bi-reachable with the maximum possible value of $|k_A - k_B|$. If there does not exist such pair of houses A and B, output "<span class="tex-font-style-tt">! 0 0</span>".</p><p>After outputting the final answer, your program must terminate immediately, otherwise you will receive Wrong Answer verdict.</p><p>You cannot ask the same query twice. <span class="tex-font-style-bf">There is no upper limit to the number of queries you ask, but, you cannot ask more queries after the judge answers "<span class="tex-font-style-tt">Yes</span>" to any of your queries.</span> Your program must now output the final answer ("<span class="tex-font-style-tt">! A B</span>" or "<span class="tex-font-style-tt">! 0 0</span>") and terminate.</p><p>If you ask a query in incorrect format or repeat a previous query, you will get Wrong Answer verdict.</p><p>After printing a query do not forget to output the end of the line and flush the output. Otherwise, you will get the Idleness limit exceeded error. To do this, use:</p><ul><li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see documentation for other languages.</li></ul></div>

## Input

<p>The first line contains a single integer $n$ ($3 \le n \le 500$) denoting the number of houses in the city. The next line contains $n$ space-separated integers $k_1, k_2, \dots, k_n$ ($0 \le k_i \le n - 1$), the $i$-th of them represents the number of incoming roads to the $i$-th house.</p>





```input1
3
1 1 1
Yes
```




```input2
4
1 2 0 3
No
No
No
No
No
No
```




```output1
? 1 2
! 1 2
```




```output2
? 2 1
? 1 3
? 4 1
? 2 3
? 4 2
? 4 3
! 0 0
```



## Note

<p>In the first sample input, we are given a city of three houses with one incoming road each. The user program asks one query: "<span class="tex-font-style-tt">? 1 2</span>": asking whether we can reach from house $1$ to house $2$. The judge responds with "<span class="tex-font-style-tt">Yes</span>". The user program now concludes that this is sufficient information to determine the correct answer. So, it outputs "<span class="tex-font-style-tt">! 1 2</span>" and quits.</p><p>In the second sample input, the user program queries for six different pairs of houses, and finally answers "<span class="tex-font-style-tt">! 0 0</span>" as it is convinced that no two houses as desired in the question exist in this city.</p>
