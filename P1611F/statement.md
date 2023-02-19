## Description

<div><p>Polycarp started working at a bank. He was assigned to monitor the ATM. The ATM initially contains $s$ rubles.</p><p>A queue of $n$ students lined up to him. Each student wants to either withdraw a certain amount of money or deposit it into an account. If $a_i$ is positive, then the student credits that amount of money via ATM. Otherwise, the student withdraws $|a_i|$ rubles.</p><p>In the beginning, the ATM is turned off and an arbitrary number of students are not served. At some point, Polycarp turns on the ATM, which has an initial amount of $s$ rubles. Then, the remaining students start queueing at the ATM. If at some point in time there is less money in the ATM than the student wants to withdraw, then the student is not served and Polycarp turns off the ATM and does not turn it on anymore.</p><p>More formally, the students that are served are forming a <span class="tex-font-style-bf">contiguous subsequence</span>.</p><p>Polycarp wants the ATM to serve the <span class="tex-font-style-bf">maximum</span> number of students. Help him in this matter. Print the numbers of the first and last student, or determine that he will not be able to serve anyone.</p><p>In other words, find such a longest continuous segment of students that, starting with the sum of $s$ at the ATM, all these students will be served. ATM serves students consistently (i.e. one after another in the order of the queue).</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>Each test case consists of two lines. The first one contains integers $n$ and $s$ ($1 \le n \le 2\cdot10^5$; $0 \le s \le 10^9$) — the length of the $a$ array and the initial amount of rubles in the ATM. The second contains $n$ integers $a_1, a_2, \dots, a_n$ ($-10^9 \le a_i \le 10^9$) — elements of the $a$ array. Note that $a_i$ can be zero.</p><p>It is guaranteed that the sum of the values $n$ over all test cases does not exceed $2\cdot10^5$.</p></div><div class="output-specification"><p>Print $t$ lines, each line must contain the answer to the corresponding set of input data: if the answer exists, print the numbers of the first and last served student. If there is no solution, then print <span class="tex-font-style-tt">-1</span> on the line.</p><p>If there are several possible answers, print any.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>Each test case consists of two lines. The first one contains integers $n$ and $s$ ($1 \le n \le 2\cdot10^5$; $0 \le s \le 10^9$) — the length of the $a$ array and the initial amount of rubles in the ATM. The second contains $n$ integers $a_1, a_2, \dots, a_n$ ($-10^9 \le a_i \le 10^9$) — elements of the $a$ array. Note that $a_i$ can be zero.</p><p>It is guaranteed that the sum of the values $n$ over all test cases does not exceed $2\cdot10^5$.</p>

## Output

<p>Print $t$ lines, each line must contain the answer to the corresponding set of input data: if the answer exists, print the numbers of the first and last served student. If there is no solution, then print <span class="tex-font-style-tt">-1</span> on the line.</p><p>If there are several possible answers, print any.</p>





```input1
3
4 10
-16 2 -6 8
3 1000
-100000 -100000 -100000
6 0
2 6 -164 1 -1 -6543
```




```output1
2 4
-1
1 2
```



## Note

<p>In the first test case, the only correct answer is <span class="tex-font-style-tt">2 4</span>, since when serving students, the number of rubles at the ATM does not become negative, and this is the maximum number of students that can be served.</p><p>In the second test case, the answer is <span class="tex-font-style-tt">-1</span>, as there is not enough money for any student at the ATM.</p><p>In the third test case, the answer can be either <span class="tex-font-style-tt">1 2</span> or <span class="tex-font-style-tt">4 5</span>.</p>
