## Description

<div><p>You are given four <span class="tex-font-style-bf">distinct</span> integers $a$, $b$, $c$, $d$. </p><p>Timur and three other people are running a marathon. The value $a$ is the distance that Timur has run and $b$, $c$, $d$ correspond to the distances the other three participants ran. </p><p>Output the number of participants in front of Timur.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>The description of each test case consists of four <span class="tex-font-style-bf">distinct</span> integers $a$, $b$, $c$, $d$ ($0 \leq a, b, c, d \leq 10^4$).</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;— the number of participants in front of Timur.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>The description of each test case consists of four <span class="tex-font-style-bf">distinct</span> integers $a$, $b$, $c$, $d$ ($0 \leq a, b, c, d \leq 10^4$).</p>

## Output

<p>For each test case, output a single integer&nbsp;— the number of participants in front of Timur.</p>





```input1
4
2 3 4 1
10000 0 1 2
500 600 400 300
0 9999 10000 9998
```




```output1
2
0
1
3
```



## Note

<p>For the first test case, there are $2$ people in front of Timur, specifically the participants who ran distances of $3$ and $4$. The other participant is not in front of Timur because he ran a shorter distance than Timur.</p><p>For the second test case, no one is in front of Timur, since he ran a distance of $10000$ while all others ran a distance of $0$, $1$, and $2$ respectively.</p><p>For the third test case, only the second person is in front of Timur, who ran a total distance of $600$ while Timur ran a distance of $500$.</p>
