## Description

<div><p><span class="tex-font-style-it">This is an interactive problem.</span></p><p>Kira has a hidden positive integer $n$, and Hayato needs to guess it.</p><p>Initially, Kira gives Hayato the value $\mathrm{cnt}$ — the number of unit bits in the binary notation of $n$. To guess $n$, Hayato can only do operations of one kind: choose an integer $x$ and subtract it from $n$. Note that after each operation, the number $n$ <span class="tex-font-style-bf">changes</span>. Kira doesn't like bad requests, so if Hayato tries to subtract a number $x$ greater than $n$, he will lose to Kira. After each operation, Kira gives Hayato the updated value $\mathrm{cnt}$ — the number of unit bits in the binary notation of the updated value of $n$.</p><p>Kira doesn't have much patience, so Hayato must guess the <span class="tex-font-style-bf">original</span> value of $n$ after no more than $30$ operations.</p><p>Since Hayato is in elementary school, he asks for your help. Write a program that guesses the number $n$. Kira is an honest person, so he chooses the initial number $n$ before all operations and <span class="tex-font-style-bf">does not</span> change it afterward.</p></div><div class="input-specification"><p>The input data contains several test cases. The first line contains one integer $t$ ($1 \le t \le 500$) — the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains the number $\mathrm{cnt}$ — the initial number of unit bits in the binary notation $n$.</p><p>The hidden integer $n$ satisfies the following constraint: $1 \le n \le 10^9$.</p></div><div><h2>Interaction</h2><p>To guess $n$, you can perform the operation at most $30$ times. To do that, print a line with the following format: "<span class="tex-font-style-tt">- x</span>" ($1 \le x \le 10^9$).</p><p>After this operation, the number $x$ is subtracted from $n$, and therefore $n$ <span class="tex-font-style-bf">is changed</span>. If the number $x$ is greater than the current value of $n$, then the request is considered invalid.</p><p>After the operation read a line containing a single non-negative integer $\mathrm{cnt}$ — the number of unit bits in the binary notation of the current $n$ after the operation.</p><p>When you know the <span class="tex-font-style-bf">initial</span> value of $n$, print one line in the following format: "<span class="tex-font-style-tt">! n</span>" ($1 \le n \le 10^9$).</p><p>After that, move on to the next test case, or terminate the program if there are none.</p><p>If your program performs more than $30$ operations for one test case, subtracts a number $x$ greater than $n$, or makes an incorrect request, then <span class="tex-font-style-bf">response to the request will be</span> <span class="tex-font-style-tt">-1</span>, after receiving such response, your program must exit immediately to receive the <span class="tex-font-style-tt">Wrong Answer</span> verdict. Otherwise, you can get any other verdict.</p><p>After printing a query or the answer, do not forget to output the end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see documentation for other languages. </li></ul><p><span class="tex-font-style-bf">Hacks</span></p><p>To make a hack, use the following format.</p><p>The first line should contain a single integer $t$ ($1 \leq t \leq 500$).</p><p>Each test case should contain one integer $n$ ($1 \leq n \leq 10^9$) on a separate line.</p></div>

## Input

<p>The input data contains several test cases. The first line contains one integer $t$ ($1 \le t \le 500$) — the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains the number $\mathrm{cnt}$ — the initial number of unit bits in the binary notation $n$.</p><p>The hidden integer $n$ satisfies the following constraint: $1 \le n \le 10^9$.</p>





```input1
3

1

0

1

1

0

2

1

0
```




```output1
- 1

! 1

- 1

- 1

! 2

- 2

- 1

! 3
```



## Note

<p>For example, the number of unit bits in number $6$ is $2$, because binary notation of $6$ is $110$. For $13$ the number of unit bits is $3$, because $13_{10} = 1101_2$.</p><p>In the first test case, $n = 1$, so the input is the number $1$. After subtracting one from $n$, it becomes zero, so the number of unit bits in it is $0$.</p><p>In the third test case, $n = 3$, which in binary representation looks like $3_{10} = 11_2$, so the input is the number of ones, that is $2$. After subtracting $2$, $n = 1$, so the number of unit bits is now $1$. After subtracting one from $n$, it becomes equal to zero.</p><p>Note that the blank lines in the input and output examples are shown for clarity and are not present in the actual interaction.</p>
