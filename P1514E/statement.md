## Description

<div><p><span class="tex-font-style-it">This is an interactive problem.</span></p><p>Baby Ehab loves crawling around his apartment. It has $n$ rooms numbered from $0$ to $n-1$. For every pair of rooms, $a$ and $b$, there's either a direct passage from room $a$ to room $b$, or from room $b$ to room $a$, but never both.</p><p>Baby Ehab wants to go play with Baby Badawy. He wants to know if he could get to him. However, he doesn't know anything about his apartment except the number of rooms. He can ask the baby sitter two types of questions: </p><ul> <li> is the passage between room $a$ and room $b$ directed from $a$ to $b$ or the other way around? </li><li> does room $x$ have a passage towards any of the rooms $s_1$, $s_2$, ..., $s_k$? </li></ul><p>He can ask at most $9n$ queries of the first type and at most $2n$ queries of the second type.</p><p>After asking some questions, he wants to know for every pair of rooms $a$ and $b$ whether there's a path from $a$ to $b$ or not. A path from $a$ to $b$ is a sequence of passages that starts from room $a$ and ends at room $b$.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 30$)&nbsp;— the number of test cases you need to solve.</p><p>Then each test case starts with an integer $n$ ($4 \le n \le 100$)&nbsp;— the number of rooms.</p><p>The sum of $n$ across the test cases doesn't exceed $500$.</p></div><div class="output-specification"><p>To print the answer for a test case, print a line containing "<span class="tex-font-style-tt">3</span>", followed by $n$ lines, each containing a binary string of length $n$. The $j$-th character of the $i$-th string should be $1$ if there's a path from room $i$ to room $j$, and $0$ if there isn't. The $i$-th character of the $i$-th string should be $1$ for each valid $i$.</p><p>After printing the answer, we will respond with a single integer. If it's $1$, you printed a correct answer and should keep solving the test cases (or exit if it is the last one). If it's $-1$, you printed a wrong answer and should terminate to get <span class="tex-font-style-tt">Wrong answer</span> verdict. Otherwise, you can get an arbitrary verdict because your solution will continue to read from a closed stream.</p></div><div><h2>Interaction</h2><p>To ask a question of the first type, use the format: </p><ul> <li> $1$ $a$ $b$ ($0 \le a,b \le n-1$, $a \neq b$). </li><li> we will answer with $1$ if the passage is from $a$ to $b$, and $0$ if it is from $b$ to $a$. </li><li> you can ask at most $9n$ questions of this type in each test case. </li></ul><p>To ask a question of the second type, use the format: </p><ul> <li> $2$ $x$ $k$ $s_1$ $s_2$ ... $s_k$ ($0 \le x,s_i \le n-1$, $0 \le k &lt; n$, $x \neq s_i$, elements of $s$ are pairwise distinct). </li><li> we will answer with $1$ if there's a passage from $x$ to any of the rooms in $s$, and $0$ otherwise. </li><li> you can ask at most $2n$ questions of this type in each test case. </li></ul><p>If we answer with $-1$ instead of a valid answer, that means you exceeded the number of queries or made an invalid query. Exit immediately after receiving $-1$ and you will see <span class="tex-font-style-tt">Wrong answer</span> verdict. Otherwise, you can get an arbitrary verdict because your solution will continue to read from a closed stream.</p><p>After printing a query, do not forget to output end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul><li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++;</li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java;</li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal;</li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python;</li><li> see the documentation for other languages.</li></ul><p><span class="tex-font-style-bf">Hacks:</span></p><p>The first line should contain an integer $t$&nbsp;— the number of test cases.</p><p>The first line of each test case should contain an integer $n$ ($4 \le n \le 100$)&nbsp;— the number of rooms.</p><p>Each of the next $n$ lines should contain a binary string of length $n$. The $j$-th character of the $i$-th string should be $1$ if there's a passage from room $i$ to room $j$, $0$ otherwise. The $i$-th character of the $i$-th string should be $0$.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 30$)&nbsp;— the number of test cases you need to solve.</p><p>Then each test case starts with an integer $n$ ($4 \le n \le 100$)&nbsp;— the number of rooms.</p><p>The sum of $n$ across the test cases doesn't exceed $500$.</p>

## Output

<p>To print the answer for a test case, print a line containing "<span class="tex-font-style-tt">3</span>", followed by $n$ lines, each containing a binary string of length $n$. The $j$-th character of the $i$-th string should be $1$ if there's a path from room $i$ to room $j$, and $0$ if there isn't. The $i$-th character of the $i$-th string should be $1$ for each valid $i$.</p><p>After printing the answer, we will respond with a single integer. If it's $1$, you printed a correct answer and should keep solving the test cases (or exit if it is the last one). If it's $-1$, you printed a wrong answer and should terminate to get <span class="tex-font-style-tt">Wrong answer</span> verdict. Otherwise, you can get an arbitrary verdict because your solution will continue to read from a closed stream.</p>





```input1
1
4

0

0

1

1

1
```




```output1
2 3 3 0 1 2

1 0 1

1 0 2

2 2 1 1

3
1111
1111
1111
0001
```



## Note

<p>In the given example:</p><p><img class="tex-graphics" src="file://NOhRUVX5.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>The first query asks whether there's a passage from room $3$ to any of the other rooms.</p><p>The second query asks about the direction of the passage between rooms $0$ and $1$.</p><p>After a couple other queries, we concluded that you can go from any room to any other room <span class="tex-font-style-bf">except</span> if you start at room $3$, and you can't get out of this room, so we printed the matrix:</p><pre class="verbatim"><br>1111<br>1111<br>1111<br>0001<br></pre><p>The interactor answered with $1$, telling us the answer is correct.</p>
