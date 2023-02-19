## Description

<div><p>Mark is administering an online exam consisting of $n$ true-false questions. However, he has lost all answer keys. He needs a way to retrieve the answers before his client gets infuriated.</p><p>Fortunately, he has access to the grading system. Thus, for each query, you can input the answers to all $n$ questions, and the grading system will output how many of them are correct.</p><p>He doesn't have much time, so he can use the grading system at most $675$ times. Help Mark determine the answer keys.</p><p>Note that answer keys are fixed in advance and will not change depending on your queries.</p></div><div class="input-specification"><p>The first line of the input consists of an integer $n$ ($1\leq n\leq 1000$) — the number of questions.</p></div><div><h2>Interaction</h2><p>After reading $n$, you can start making queries to the grading system. For each query, print a line containing a string $s$ of length $n$ consisting of only letters '<span class="tex-font-style-tt">T</span>' and '<span class="tex-font-style-tt">F</span>'. </p><ul> <li> $s_i = $'<span class="tex-font-style-tt">T</span>' means that you answer the $i$-question <span class="tex-font-style-tt">true</span>. </li><li> $s_i = $'<span class="tex-font-style-tt">F</span>' means that you answer the $i$-question <span class="tex-font-style-tt">false</span>. </li></ul><p>After a successful query, you should read an integer $k$ ($0\leq k\leq n$) — the number of correct answers. <span class="tex-font-style-bf">If you read $n$, then you found the answers, and your program should not make any more queries.</span></p><p>If your program reads $k = -1$ instead of the number of correct answers, it means that you either made an invalid query or exceeded the query limits. Exit immediately after receiving $-1$, and you will see <span class="tex-font-style-tt">Wrong answer</span> verdict. Otherwise, you can get an arbitrary verdict because your solution will continue to read from a closed stream.</p><p>After printing a query do not forget to output end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use: </p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see documentation for other languages. </li></ul><p><span class="tex-font-style-bf">Hacks</span></p><p>To hack, use the following format:</p><p>The first line contains an integer $n$ ($1\leq n\leq 1000$) — the number of questions.</p><p>The second line contains a string $s$ of length $n$ consisting of only '<span class="tex-font-style-tt">T</span>' and '<span class="tex-font-style-tt">F</span>' — the answer key.</p></div>

## Input

<p>The first line of the input consists of an integer $n$ ($1\leq n\leq 1000$) — the number of questions.</p>





```input1
3

1

3
```




```input2
4

0

3

4
```




```output1
FTT

TTF
```




```output2
FTFF

TTTT

TFTT
```



## Note

<p>The empty lines in the example are just for you to better understand the interaction process. <span class="tex-font-style-bf">You're not required to print them.</span></p><p>In the first example, there are $3$ questions, and the answer to each question is '<span class="tex-font-style-tt">true</span>', '<span class="tex-font-style-tt">true</span>', and '<span class="tex-font-style-tt">false</span>', respectively. </p><ul> <li> The first query, guessing the answers to be '<span class="tex-font-style-tt">false</span>', '<span class="tex-font-style-tt">true</span>', and '<span class="tex-font-style-tt">true</span>', respectively, guesses only one question — the $2$-nd question — correctly. </li><li> Then, in the second query, the program correctly guesses the answer key. The interaction ends here. </li></ul><p>In the second example, there are $4$ questions, and the answer to each question is '<span class="tex-font-style-tt">true</span>', '<span class="tex-font-style-tt">false</span>', '<span class="tex-font-style-tt">true</span>', and '<span class="tex-font-style-tt">true</span>', respectively. </p><ul> <li> The first query guessed none of the questions correctly, resulting in the answer $0$. </li><li> The second query guessed the $1$-st, $3$-rd, and $4$-th question correctly, resulting in the answer $3$. </li><li> In the third query, the program correctly guesses the answer key. Then, the interaction ends. </li></ul>
