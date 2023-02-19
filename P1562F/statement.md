## Description

<div><p>Do you know what tubular bells are? They are a musical instrument made up of cylindrical metal tubes. In an orchestra, tubular bells are used to mimic the ringing of bells.</p><p>Mike has tubular bells, too! They consist of $n$ tubes, and each of the tubes has a length that can be expressed by a integer from $l$ to $r$ inclusive. It is clear that the lengths of all the tubes are different (it makes no sense to make the same tubes). It is also known that $r-l+1 = n$.</p><p>Formally, we can say that Mike's tubular bells are described by a permutation $a$ of length $n$ that contains all numbers from $l$ to $r$ inclusive, with $a_i$ denoting the length of the $i$-th tube.</p><p>You are offered an interesting task: to guess what Mike's instrument looks like. Simply, you must guess the permutation.</p><p>Mike won't tell you $l$ or $r$. He will only tell you $n$, and will allow you to ask no more than $n + 5000$ queries.</p><p>In each query, you name two positive integers $x$, $y$ such that $1 \le x, y \le n, x \neq y$. In response to this query, the program written by Mike will give you $\mathrm{lcm}(a_x, a_y)$, where $\mathrm{lcm}(c,d)$ denotes the least common multiple of $c$ and $d$.</p><p>Solve Mike's problem!</p></div><div class="input-specification"><p>Each test contains multiple test cases.</p><p>The first line contains one positive integer $t$ ($1 \le t \le 20$), denoting the number of test cases. Description of the test cases follows.</p><p>The single line of each test case contains one positive integer $n$ ($3 \le n \le 10^5$)&nbsp;— number of tubes in Mike's tubular bells. Also $1 \le l \le r \le 2 \cdot 10^5$, i.e. the lengths of the tubes do not exceed $2 \cdot 10^5$.</p><p>It is guaranteed that the sum of <span class="tex-font-style-bf">maximal number of queries</span> (i.e. $n + 5000$) over all test cases does not exceed $10^5 + 5000$. It means that sum of $n$ does not exceed $10^5 + 5000 - t \cdot 5000$.</p></div><div><h2>Interaction</h2><p>For each set of input data, read one integer $n$. You are allowed to make no more than $n + 5000$ queries.</p><p>If you want to make a query, output it in the format "? $x$ $y$", where $x$ and $y$&nbsp;— the numbers of tubes for which you learn the lcm (least common multiple) of their lengths. Note that $1 \le x, y \le n, x \neq y$ must be satisfied. The interactor will return a single integer&nbsp;—the answer to your query.</p><p>If you are ready to print the answer, print it in the format "! $a_1$ $a_2$ ... $a_n$". <span class="tex-font-style-bf">The output of the answer is not considered a query and is not included in the number of queries.</span></p><p>After each query and answer output, don't forget to output the line translation and reset the output buffer. Otherwise you will get the verdict "Idleness limit exceeded". To reset the buffer use:</p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or cout.flush() in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see documentation for other languages. </li></ul><p><span class="tex-font-style-bf">Note that the interactor is not adaptive.</span> That is, the original permutation is fixed in the beginning and don't depend on your queries.</p><p><span class="tex-font-style-bf">Hacks:</span></p><p>Use the following format for hacks:</p><p>The first line contains a single positive integer $t$ ($1 \le t \le 20$)&nbsp;— the number of input datasets. A description of the input data sets is given below.</p><p>The first line of each test case contains one positive integer $n$ ($3 \le n \le 10^5$)&nbsp;—the number of tubes. It is known that $1 \le l \le r \le 2 \cdot 10^5$, i.e. the lengths of the tubes do not exceed $2 \cdot 10^5$.</p><p>The second line of each test case contains an array $a$ of $n$ positive integers&nbsp;— the lengths of the tubes in each input dataset. Remember that $l \le a_i \le r$ and $r-l+1 = n$, and that all $a_i$ are different.</p></div>

## Input

<p>Each test contains multiple test cases.</p><p>The first line contains one positive integer $t$ ($1 \le t \le 20$), denoting the number of test cases. Description of the test cases follows.</p><p>The single line of each test case contains one positive integer $n$ ($3 \le n \le 10^5$)&nbsp;— number of tubes in Mike's tubular bells. Also $1 \le l \le r \le 2 \cdot 10^5$, i.e. the lengths of the tubes do not exceed $2 \cdot 10^5$.</p><p>It is guaranteed that the sum of <span class="tex-font-style-bf">maximal number of queries</span> (i.e. $n + 5000$) over all test cases does not exceed $10^5 + 5000$. It means that sum of $n$ does not exceed $10^5 + 5000 - t \cdot 5000$.</p>





```input1
3
5
8 10 7 6 9
5
24 25 28 27 26
7
1 2 3 4 5 6 7
```




```output1
? 1 2
40
? 2 5
90
? 3 1
56
? 4 5
18
! 8 10 7 6 9
? 1 5
312
? 2 4
675
! 24 25 28 27 26
? 1 4
4
? 2 5
10
? 3 7
21
? 6 2
6
? 2 5
10
? 1 2
2
? 1 2
2
? 1 2
2
? 1 2
2
? 1 2
2
! 1 2 3 4 5 6 7
```


