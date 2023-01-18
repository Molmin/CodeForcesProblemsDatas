## Description

<div><p>Authors guessed an array $a$ consisting of $n$ integers; each integer is not less than $2$ and not greater than $2 \cdot 10^5$. You don't know the array $a$, but you know the array $b$ which is formed from it with the following sequence of operations:</p><ol> <li> Firstly, let the array $b$ be equal to the array $a$; </li><li> Secondly, for each $i$ from $1$ to $n$: <ul> <li> if $a_i$ is a <span class="tex-font-style-bf">prime</span> number, then one integer $p_{a_i}$ is appended to array $b$, where $p$ is an infinite sequence of prime numbers ($2, 3, 5, \dots$); </li><li> otherwise (if $a_i$ is not a <span class="tex-font-style-bf">prime</span> number), the greatest divisor of $a_i$ which is not equal to $a_i$ is appended to $b$; </li></ul> </li><li> Then the obtained array of length $2n$ is shuffled and given to you in the input. </li></ol><p>Here $p_{a_i}$ means the $a_i$-th prime number. The first prime $p_1 = 2$, the second one is $p_2 = 3$, and so on.</p><p>Your task is to recover <span class="tex-font-style-bf">any</span> suitable array $a$ that forms the given array $b$. It is guaranteed that the answer exists (so the array $b$ is obtained from some suitable array $a$). If there are multiple answers, you can print any.</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of elements in $a$.</p><p>The second line of the input contains $2n$ integers $b_1, b_2, \dots, b_{2n}$ ($2 \le b_i \le 2750131$), where $b_i$ is the $i$-th element of $b$. $2750131$ is the $199999$-th prime number.</p></div><div class="output-specification"><p>In the only line of the output print $n$ integers $a_1, a_2, \dots, a_n$ ($2 \le a_i \le 2 \cdot 10^5$) in <span class="tex-font-style-bf">any</span> order — the array $a$ from which the array $b$ can be obtained using the sequence of moves given in the problem statement. If there are multiple answers, you can print any.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of elements in $a$.</p><p>The second line of the input contains $2n$ integers $b_1, b_2, \dots, b_{2n}$ ($2 \le b_i \le 2750131$), where $b_i$ is the $i$-th element of $b$. $2750131$ is the $199999$-th prime number.</p>

## Output

<p>In the only line of the output print $n$ integers $a_1, a_2, \dots, a_n$ ($2 \le a_i \le 2 \cdot 10^5$) in <span class="tex-font-style-bf">any</span> order — the array $a$ from which the array $b$ can be obtained using the sequence of moves given in the problem statement. If there are multiple answers, you can print any.</p>





```input1
3
3 5 2 3 2 4
```




```input2
1
2750131 199999
```




```input3
1
3 6
```




```output1
3 4 2
```




```output2
199999
```




```output3
6
```


