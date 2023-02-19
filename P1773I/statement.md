## Description

<div><p>Oh no, this wicked jury hides something from you again, and you need to guess it interactively. </p><p>This time, you need to find an integer $n$. To do that, you can make at most 10 queries of the form "What&nbsp;is the $k$-th decimal digit of the product of all integers from 1 to $n$ (also known as factorial and denoted as&nbsp;$n!$)?". </p></div><div><h2>Interaction</h2><p>In the first line, there is an integer $t$ ($1 \le t \le 100$)&nbsp;— the number of tests you shall process. </p><p>For each test, the integer $n$ is chosen in advance. The length of $n!$ is at most $20\,000$, so $1 \le n \le 5982$.</p><p>You can make <span class="tex-font-style-bf">at most 10 queries</span> of the form "<span class="tex-font-style-tt">? </span>$k$" ($0 \le k &lt; 20\,000$). In response to the query, you will get a single digit&nbsp;— the $k$-th decimal digit of $n!$ (the response is between 0 and 9 inclusive). Digits are numbered from 0, starting with the least significant digit. If $n!$ is too short, and there is no $k$-th digit, then 0 is returned. </p><p>After your program finds the value of $n$ it shall answer with "<span class="tex-font-style-tt">! </span>$n$". If the answer is correct, then you will receive "<span class="tex-font-style-tt">YES</span>" and should proceed to the next test or terminate if it was the last one. If the answer is not correct, or you are trying to guess, and there are several possible answers consistent with the information you have received, you will get "<span class="tex-font-style-tt">NO</span>". In that case, your submission will receive "<span class="tex-font-style-tt">Wrong answer</span>" verdict and your code shall terminate immediately. </p></div>





```input1
2

1

YES

0

2

YES
```




```output1
? 0

! 1

? 0

? 19997

! 5982
```


