## Description

<div><p>Monocarp and Polycarp are playing a computer game. This game features $n$ bosses for the playing to kill, numbered from $1$ to $n$.</p><p>They will fight <span class="tex-font-style-bf">each</span> boss the following way: </p><ul> <li> Monocarp makes $k$ attempts to kill the boss; </li><li> Polycarp makes $k$ attempts to kill the boss; </li><li> Monocarp makes $k$ attempts to kill the boss; </li><li> Polycarp makes $k$ attempts to kill the boss; </li><li> ... </li></ul><p>Monocarp kills the $i$-th boss on <span class="tex-font-style-bf">his</span> $a_i$-th attempt. Polycarp kills the $i$-th boss on <span class="tex-font-style-bf">his</span> $b_i$-th attempt. After one of them kills the $i$-th boss, they move on to the $(i+1)$-st boss. The attempt counters reset for both of them. Once one of them kills the $n$-th boss, the game ends.</p><p>Find all values of $k$ from $1$ to $n$ such that Monocarp kills <span class="tex-font-style-bf">all bosses</span>.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the number of bosses.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$)&nbsp;— the index of attempt Monocarp kills each boss on.</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_i \le n$)&nbsp;— the index of attempt Polycarp kills each boss on.</p><p>The sum of $n$ over all testcases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each testcase, print two lines. The first line should contain a single integer $\mathit{cnt}$&nbsp;— the number of values of $k$ from $1$ to $n$ such that Monocarp kills <span class="tex-font-style-bf">all bosses</span>. The second line should contain $\mathit{cnt}$ distinct integers&nbsp;— the values of $k$ themselves.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the number of bosses.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$)&nbsp;— the index of attempt Monocarp kills each boss on.</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_i \le n$)&nbsp;— the index of attempt Polycarp kills each boss on.</p><p>The sum of $n$ over all testcases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each testcase, print two lines. The first line should contain a single integer $\mathit{cnt}$&nbsp;— the number of values of $k$ from $1$ to $n$ such that Monocarp kills <span class="tex-font-style-bf">all bosses</span>. The second line should contain $\mathit{cnt}$ distinct integers&nbsp;— the values of $k$ themselves.</p>





```input1|2,3,4,8,9,10
3
3
1 1 1
2 3 1
1
1
1
4
1 4 3 2
3 3 4 1
```




```output1
3
1 2 3 
1
1 
2
2 4
```



## Note

<p>Consider the last testcase of the example.</p><p>Let $k = 1$. First, Monocarp makes one attempt to kill the first boss. It's successful, since $a_1 = 1$. Then, Monocarp makes one attempt to kill the second boss. It's unsuccessful, since $a_2 &gt; 1$. So, Polycarp makes an attempt then. It's also unsuccessful, since $b_2 &gt; 1$. Then, Monocarp makes another attempt. It's still unsuccessful, since $a_2 &gt; 2$. This goes on until Polycarp finally kills the boss on his third attempt. Monocarp didn't kill this boss, thus, $k = 1$ isn't the answer.</p><p>Let $k = 2$. Monocarp still kills the first boss on his first attempt. Then, he makes two unsuccessful attempts for the second boss. Then, Polycarp makes two unsuccessful attempts. Then, Monocarp makes two more attempts and kills the boss on his fourth attempt. The third boss is similar. First, two unsuccessful attempts by Monocarp. Then, two unsuccessful attempts by Polycarp. Then, Monocarp has two more attempts, but even his first one is successful, since $a_3 = 3$. The fourth boss is also killed by Monocarp. Thus, $k = 2$ is the answer.</p>
