## Description

<div><p>The hero is addicted to glory, and is fighting against a monster. </p><p>The hero has $n$ skills. The $i$-th skill is of type $a_i$ (either <span class="tex-font-style-bf">fire</span> or <span class="tex-font-style-bf">frost</span>) and has initial damage $b_i$. </p><p>The hero can perform all of the $n$ skills in any order (with each skill performed exactly <span class="tex-font-style-bf">once</span>). When performing each skill, the hero can play a magic as follows: </p><ul> <li> If the current skill immediately follows another skill of a different type, then its damage is <span class="tex-font-style-bf">doubled</span>. </li></ul> In other words, <ol> <li> If a skill of type fire and with initial damage $c$ is performed immediately after a skill of type fire, then it will deal $c$ damage; </li><li> If a skill of type fire and with initial damage $c$ is performed immediately after a skill of type frost, then it will deal $2c$ damage; </li><li> If a skill of type frost and with initial damage $c$ is performed immediately after a skill of type fire, then it will deal $2c$ damage; </li><li> If a skill of type frost and with initial damage $c$ is performed immediately after a skill of type frost , then it will deal $c$ damage. </li></ol><p>Your task is to find the <span class="tex-font-style-bf">maximum</span> damage the hero can deal. </p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 10^5$) — the number of test cases. The following lines contain the description of each test case.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 10^5$), indicating the number of skills. </p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \leq a_i \leq 1$), where $a_i$ indicates the type of the $i$-th skill. Specifically, the $i$-th skill is of type fire if $a_i = 0$, and of type frost if $a_i = 1$. </p><p>The third line of each test case contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \leq b_i \leq 10^9$), where $b_i$ indicates the initial damage of the $i$-th skill. </p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, output the maximum damage the hero can deal.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 10^5$) — the number of test cases. The following lines contain the description of each test case.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 10^5$), indicating the number of skills. </p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \leq a_i \leq 1$), where $a_i$ indicates the type of the $i$-th skill. Specifically, the $i$-th skill is of type fire if $a_i = 0$, and of type frost if $a_i = 1$. </p><p>The third line of each test case contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \leq b_i \leq 10^9$), where $b_i$ indicates the initial damage of the $i$-th skill. </p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, output the maximum damage the hero can deal.</p>





```input1|2,3,4,8,9,10
4
4
0 1 1 1
1 10 100 1000
6
0 0 0 1 1 1
3 4 5 6 7 8
3
1 1 1
1000000000 1000000000 1000000000
1
1
1
```




```output1
2112
63
3000000000
1
```



## Note

<p>In the first test case, we can order the skills by $[3, 1, 4, 2]$, and the total damage is $100 + 2 \times 1 + 2 \times 1000 + 10 = 2112$.</p><p>In the second test case, we can order the skills by $[1, 4, 2, 5, 3, 6]$, and the total damage is $3 + 2 \times 6 + 2 \times 4 + 2 \times 7 + 2 \times 5 + 2 \times 8 = 63$.</p><p>In the third test case, we can order the skills by $[1, 2, 3]$, and the total damage is $1000000000 + 1000000000 + 1000000000 = 3000000000$.</p><p>In the fourth test case, there is only one skill with initial damage $1$, so the total damage is $1$. </p>
