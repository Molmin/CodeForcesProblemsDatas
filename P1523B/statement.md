## Description

<div><center> <img class="tex-graphics" height="378px" src="file://ZncXghjU.png" style="max-width: 100.0%;max-height: 100.0%;" width="567px"> </center><p>While trading on his favorite exchange trader William realized that he found a vulnerability. Using this vulnerability he could change the values of certain internal variables to his advantage. To play around he decided to change the values of all internal variables from $a_1, a_2, \ldots, a_n$ to $-a_1, -a_2, \ldots, -a_n$. For some unknown reason, the number of service variables is always an even number.</p><p>William understands that with his every action he attracts more and more attention from the exchange's security team, so the number of his actions must not exceed $5\,000$ and after every operation no variable can have an absolute value greater than $10^{18}$. William can perform actions of two types for two chosen variables with indices $i$ and $j$, where $i &lt; j$:</p><ol> <li> Perform assignment $a_i = a_i + a_j$ </li><li> Perform assignment $a_j = a_j - a_i$ </li></ol> William wants you to develop a strategy that will get all the internal variables to the desired values.</div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 20$). Description of the test cases follows.</p><p>The first line of each test case contains a single <span class="tex-font-style-bf">even</span> integer $n$ ($2 \le n \le 10^3$), which is the number of internal variables.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ $(1 \le a_i \le 10^9)$, which are initial values of internal variables.</p></div><div class="output-specification"><p>For each test case print the answer in the following format:</p><p>The first line of output must contain the total number of actions $k$, which the strategy will perform. Note that you do not have to minimize $k$. The inequality $k \le 5\,000$ must be satisfied. </p><p>Each of the next $k$ lines must contain actions formatted as "<span class="tex-font-style-tt">type i j</span>", where "<span class="tex-font-style-tt">type</span>" is equal to "<span class="tex-font-style-tt">1</span>" if the strategy needs to perform an assignment of the first type and "<span class="tex-font-style-tt">2</span>" if the strategy needs to perform an assignment of the second type. Note that $i &lt; j$ should hold.</p><p>We can show that an answer always exists.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 20$). Description of the test cases follows.</p><p>The first line of each test case contains a single <span class="tex-font-style-bf">even</span> integer $n$ ($2 \le n \le 10^3$), which is the number of internal variables.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ $(1 \le a_i \le 10^9)$, which are initial values of internal variables.</p>

## Output

<p>For each test case print the answer in the following format:</p><p>The first line of output must contain the total number of actions $k$, which the strategy will perform. Note that you do not have to minimize $k$. The inequality $k \le 5\,000$ must be satisfied. </p><p>Each of the next $k$ lines must contain actions formatted as "<span class="tex-font-style-tt">type i j</span>", where "<span class="tex-font-style-tt">type</span>" is equal to "<span class="tex-font-style-tt">1</span>" if the strategy needs to perform an assignment of the first type and "<span class="tex-font-style-tt">2</span>" if the strategy needs to perform an assignment of the second type. Note that $i &lt; j$ should hold.</p><p>We can show that an answer always exists.</p>





```input1
2
4
1 1 1 1
4
4 3 1 2
```




```output1
8
2 1 2
2 1 2
2 1 3
2 1 3
2 1 4
2 1 4
1 1 2
1 1 2
8
2 1 4
1 2 4
1 2 4
1 2 4
1 3 4
1 1 2
1 1 2
1 1 4
```



## Note

<p>For the first sample test case one possible sequence of operations is as follows:</p><ol> <li> "<span class="tex-font-style-tt">2 1 2</span>". Values of variables after performing the operation: [1, <span class="tex-font-style-bf">0</span>, 1, 1] </li><li> "<span class="tex-font-style-tt">2 1 2</span>". Values of variables after performing the operation: [1, <span class="tex-font-style-bf">-1</span>, 1, 1] </li><li> "<span class="tex-font-style-tt">2 1 3</span>". Values of variables after performing the operation: [1, -1, <span class="tex-font-style-bf">0</span>, 1] </li><li> "<span class="tex-font-style-tt">2 1 3</span>". Values of variables after performing the operation: [1, -1, <span class="tex-font-style-bf">-1</span>, 1] </li><li> "<span class="tex-font-style-tt">2 1 4</span>". Values of variables after performing the operation: [1, -1, -1, <span class="tex-font-style-bf">0</span>] </li><li> "<span class="tex-font-style-tt">2 1 4</span>". Values of variables after performing the operation: [1, -1, -1, <span class="tex-font-style-bf">-1</span>] </li><li> "<span class="tex-font-style-tt">1 1 2</span>". Values of variables after performing the operation: [<span class="tex-font-style-bf">0</span>, -1, -1, -1] </li><li> "<span class="tex-font-style-tt">1 1 2</span>". Values of variables after performing the operation: [<span class="tex-font-style-bf">-1</span>, -1, -1, -1] </li></ol><p>For the second sample test case one possible sequence of operations is as follows:</p><ol> <li> "<span class="tex-font-style-tt">2 1 4</span>". Values of variables after performing the operation: [4, 3, 1, <span class="tex-font-style-bf">-2</span>] </li><li> "<span class="tex-font-style-tt">1 2 4</span>". Values of variables after performing the operation: [4, <span class="tex-font-style-bf">1</span>, 1, -2] </li><li> "<span class="tex-font-style-tt">1 2 4</span>". Values of variables after performing the operation: [4, <span class="tex-font-style-bf">-1</span>, 1, -2] </li><li> "<span class="tex-font-style-tt">1 2 4</span>". Values of variables after performing the operation: [4, <span class="tex-font-style-bf">-3</span>, 1, -2] </li><li> "<span class="tex-font-style-tt">1 3 4</span>". Values of variables after performing the operation: [4, -3, <span class="tex-font-style-bf">-1</span>, -2] </li><li> "<span class="tex-font-style-tt">1 1 2</span>". Values of variables after performing the operation: [<span class="tex-font-style-bf">1</span>, -3, -1, -2] </li><li> "<span class="tex-font-style-tt">1 1 2</span>". Values of variables after performing the operation: [<span class="tex-font-style-bf">-2</span>, -3, -1, -2] </li><li> "<span class="tex-font-style-tt">1 1 4</span>". Values of variables after performing the operation: [<span class="tex-font-style-bf">-4</span>, -3, -1, -2] </li></ol>
