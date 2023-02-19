## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem. Remember to flush your output while communicating with the testing program.</span> You may use <span class="tex-font-style-tt">fflush(stdout)</span> in C++, <span class="tex-font-style-tt">system.out.flush()</span> in Java, <span class="tex-font-style-tt">stdout.flush()</span> in Python or <span class="tex-font-style-tt">flush(output)</span> in Pascal to flush the output. If you use some other programming language, consult its documentation. You may also refer to the guide on interactive problems: <a href="https://codeforces.com/blog/entry/45307">https://codeforces.com/blog/entry/45307</a>.</p><p>The jury has chosen a string $s$ consisting of $n$ characters; each character of $s$ is a lowercase Latin letter. Your task is to guess this string; initially, you know only its length.</p><p>You may ask queries of two types:</p><ul> <li> $1$ $i$ — the query of the first type, where $i$ is an integer from $1$ to $n$. In response to this query, the jury will tell you the character $s_i$; </li><li> $2$ $l$ $r$ — the query of the second type, where $l$ and $r$ are integers such that $1 \le l \le r \le n$. In response to this query, the jury will tell you the number of different characters among $s_l, s_{l+1}, \dots, s_r$. </li></ul><p>You are allowed to ask no more than $26$ queries of the first type, and no more than $6000$ queries of the second type. Your task is to restore the string $s$.</p><p>For each test in this problem, the string $s$ is fixed beforehand, and will be the same for every submission.</p></div><div class="input-specification"><p>Initially, the jury program sends one integer $n$ on a separate line — the size of $s$ ($1 \le n \le 1000$).</p></div><div class="output-specification"><p>To give the answer, print one line <span class="tex-font-style-tt">! s</span> <span class="tex-font-style-it">with a line break in the end</span>, where $s$ should be the string picked by the jury. After that, your program should flush the output and terminate gracefully.</p></div><div><h2>Interaction</h2><p>To ask a query, you should send one line containing the query, in one of the following formats:</p><ul> <li> <span class="tex-font-style-tt">? 1 i</span> — for a query of the first type ($1 \le i \le n$); </li><li> <span class="tex-font-style-tt">? 2 l r</span> — for a query of the second type ($1 \le l \le r \le n$). </li></ul><p>Don't forget to flush the output after sending the query line.</p><p>The answer to your query will be given on a separate line. For a query of the first type, the answer will be the character $s_i$. For a query of the second type, the answer will be an integer equal to the number of different characters among $s_l, s_{l+1}, \dots, s_r$.</p><p>You are allowed to ask no more than $26$ queries of the first type, and no more than $6000$ queries of the second type.</p><p>In case you ask too many queries, or the jury program fails to recognize your query format, the answer to your query will be one integer $0$. After receiving $0$ as the answer, your program should terminate immediately — otherwise you may receive verdict "Runtime error", "Time limit exceeded" or some other verdict instead of "Wrong answer".</p></div>

## Input

<p>Initially, the jury program sends one integer $n$ on a separate line — the size of $s$ ($1 \le n \le 1000$).</p>

## Output

<p>To give the answer, print one line <span class="tex-font-style-tt">! s</span> <span class="tex-font-style-it">with a line break in the end</span>, where $s$ should be the string picked by the jury. After that, your program should flush the output and terminate gracefully.</p>





```input1
5
4
u
2
g
e
s
1
```




```output1
? 2 1 5
? 1 2
? 2 1 2
? 1 1
? 1 3
? 1 4
? 2 4 5
! guess
```



## Note

<p>Let's analyze the example of interaction.</p><p>The string chosen by the jury is <span class="tex-font-style-tt">guess</span>, so initially the jury sends one integer $5$.</p><ol> <li> the first query is <span class="tex-font-style-tt">? 2 1 5</span>, which means "count the number of different characters among $s_1, s_2, \dots, s_5$". The answer to it is $4$. </li><li> the second query is <span class="tex-font-style-tt">? 1 2</span>, which means "tell which character is $s_2$". The answer to it is <span class="tex-font-style-tt">u</span>. </li><li> the third query is <span class="tex-font-style-tt">? 2 1 2</span>, which means "count the number of different characters among $s_1$ and $s_2$". The answer to it is $2$. </li><li> the fourth query is <span class="tex-font-style-tt">? 1 1</span>, which means "tell which character is $s_1$". The answer to it is <span class="tex-font-style-tt">g</span>. </li><li> the fifth query is <span class="tex-font-style-tt">? 1 3</span>, which means "tell which character is $s_3$". The answer to it is <span class="tex-font-style-tt">e</span>. </li><li> the sixth query is <span class="tex-font-style-tt">? 1 4</span>, which means "tell which character is $s_4$". The answer to it is <span class="tex-font-style-tt">s</span>. </li><li> the seventh query is <span class="tex-font-style-tt">? 2 4 5</span>, which means "count the number of different characters among $s_4$ and $s_5$". The answer to it is $1$, so it's possible to deduce that $s_4$ is the same as $s_5$.</li></ol><p>In the end, the answer is submitted as <span class="tex-font-style-tt">! guess</span>, and it is deduced correctly.</p>
