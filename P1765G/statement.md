## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem. You have to use <span class="tex-font-style-tt">flush</span> operation right after printing each line. For example, in C++ you should use the function <span class="tex-font-style-tt">fflush(stdout)</span>, in Java or Kotlin — <span class="tex-font-style-tt">System.out.flush()</span>, and in Python — <span class="tex-font-style-tt">sys.stdout.flush()</span>.</span></p><p>The jury has a string $s$ consisting of characters <span class="tex-font-style-tt">0</span> and/or <span class="tex-font-style-tt">1</span>. The first character of this string is <span class="tex-font-style-tt">0</span>. The length of this string is $n$. You have to guess this string. Let's denote $s[l..r]$ as the substring of $s$ from $l$ to $r$ (i. e. $s[l..r]$ is the string $s_ls_{l+1} \dots s_r$).</p><p>Let the <span class="tex-font-style-it">prefix function</span> of the string $s$ be an array $[p_1, p_2, \dots, p_n]$, where $p_i$ is the greatest integer $j \in [0, i-1]$ such that $s[1..j] = s[i-j+1..i]$. Also, let the <span class="tex-font-style-it">antiprefix function</span> of the string $s$ be an array $[q_1, q_2, \dots, q_n]$, where $q_i$ is the greatest integer $j \in [0, i-1]$ such that $s[1..j]$ differs from $s[i-j+1..i]$ in <span class="tex-font-style-bf">every</span> position.</p><p>For example, for the string <span class="tex-font-style-tt">011001</span>, its <span class="tex-font-style-it">prefix function</span> is $[0, 0, 0, 1, 1, 2]$, and its <span class="tex-font-style-it">antiprefix function</span> is $[0, 1, 1, 2, 3, 4]$.</p><p>You can ask queries of two types to guess the string $s$:</p><ul> <li> $1$ $i$ — "what is the value of $p_i$?"; </li><li> $2$ $i$ — "what is the value of $q_i$?". </li></ul><p>You have to guess the string by asking no more than $789$ queries. Note that giving the answer does not count as a query.</p><p><span class="tex-font-style-bf">In every test and in every test case, the string $s$ is fixed beforehand</span>.</p></div><div><h2>Interaction</h2><p>Initially, the jury program sends one integer $t$ ($1 \le t \le 100$) — the number of test cases.</p><p>At the start of each test case, the jury program sends one integer $n$ ($2 \le n \le 1000$) — the length of the string.</p><p>After that, your program can submit queries to the jury program by printing one of the following lines <span class="tex-font-style-bf">(do not forget to flush the output after printing a line!)</span>:</p><ul> <li> $1$ $i$ — the query "what is the value of $p_i$?"; </li><li> $2$ $i$ — the query "what is the value of $q_i$?". </li></ul><p>For every query, the jury prints one integer on a separate line. It is either:</p><ul> <li> the answer for your query, if the query is correct and you haven't exceeded the query limit; </li><li> or the integer $-1$, if your query is incorrect (for example, the constraint $1 \le i \le n$ is not met) or if you have asked too many queries while processing the current test case. </li></ul><p>To submit the answer, your program should send a line in the following format <span class="tex-font-style-bf">(do not forget to flush the output after printing a line!)</span>:</p><ul> <li> $0$ $s$, where $s$ is a sequence of $n$ characters <span class="tex-font-style-tt">0</span> and/or <span class="tex-font-style-tt">1</span>. </li></ul><p>If your guess is correct, the jury program will print one integer $1$ on a separate line, indicating that you may proceed to the next test case (or terminate the program, if it was the last test case) and that the number of queries you have asked is reset. If it is not correct, the jury program will print one integer $-1$ on a separate line.</p><p>After your program receives $-1$ as the answer, it should immediately terminate. This will lead to your submission receiving the verdict "Wrong Answer". If your program does not terminate, the verdict of your submission is undefined.</p></div>





```input1
2 // 2 test cases
6 // n = 6

0 // p[3] = 0

1 // q[2] = 1

4 // q[6] = 4

1 // p[4] = 1

1 // answer is correct
5 // n = 5

1 // p[2] = 1

2 // q[4] = 2

2 // q[5] = 2

1 // answer is correct
```




```output1
1 3      // what is p[3]?

2 2      // what is q[2]?

2 6      // what is q[6]?

1 4      // what is p[4]?

0 011001 // the guess is 011001


1 2      // what is p[2]?

2 4      // what is q[4]?

2 5      // what is q[5]?

0 00111  // the guess is 00111
```



## Note

<p>The example contains one possible way of interaction in a test where $t = 2$, and the strings guessed by the jury are <span class="tex-font-style-tt">011001</span> and <span class="tex-font-style-tt">00111</span>. Note that everything after the <span class="tex-font-style-tt">//</span> sign is a comment that explains which line means what in the interaction. <span class="tex-font-style-bf">The jury program won't print these comments in the actual problem, and you shouldn't print them</span>. The empty lines are also added for your convenience, <span class="tex-font-style-bf">the jury program won't print them, and your solution should not print any empty lines</span>.</p>
