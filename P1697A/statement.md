## Description

<div><p>You are walking through a parkway near your house. The parkway has $n+1$ benches in a row numbered from $1$ to $n+1$ from left to right. The distance between the bench $i$ and $i+1$ is $a_i$ meters.</p><p>Initially, you have $m$ units of energy. To walk $1$ meter of distance, you spend $1$ unit of your energy. You can't walk if you have no energy. Also, you can restore your energy by <span class="tex-font-style-bf">sitting on benches</span> (and this is the only way to restore the energy). When you are sitting, you can restore any integer amount of energy you want (if you sit longer, you restore more energy). Note that the amount of your energy <span class="tex-font-style-bf">can exceed</span> $m$.</p><p>Your task is to find the <span class="tex-font-style-bf">minimum</span> amount of energy you have to <span class="tex-font-style-bf">restore</span> (by sitting on benches) to reach the bench $n+1$ from the bench $1$ (and end your walk).</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 100$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains two integers $n$ and $m$ ($1 \le n \le 100$; $1 \le m \le 10^4$).</p><p>The second line of the test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 100$), where $a_i$ is the distance between benches $i$ and $i+1$.</p></div><div class="output-specification"><p>For each test case, print one integer — the <span class="tex-font-style-bf">minimum</span> amount of energy you have to <span class="tex-font-style-bf">restore</span> (by sitting on benches) to reach the bench $n+1$ from the bench $1$ (and end your walk) in the corresponding test case.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 100$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains two integers $n$ and $m$ ($1 \le n \le 100$; $1 \le m \le 10^4$).</p><p>The second line of the test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 100$), where $a_i$ is the distance between benches $i$ and $i+1$.</p>

## Output

<p>For each test case, print one integer — the <span class="tex-font-style-bf">minimum</span> amount of energy you have to <span class="tex-font-style-bf">restore</span> (by sitting on benches) to reach the bench $n+1$ from the bench $1$ (and end your walk) in the corresponding test case.</p>





```input1
3
3 1
1 2 1
4 5
3 3 5 2
5 16
1 2 3 4 5
```




```output1
3
8
0
```



## Note

<p>In the first test case of the example, you can walk to the bench $2$, spending $1$ unit of energy, then restore $2$ units of energy on the second bench, walk to the bench $3$, spending $2$ units of energy, restore $1$ unit of energy and go to the bench $4$.</p><p>In the third test case of the example, you have enough energy to just go to the bench $6$ without sitting at all.</p>
