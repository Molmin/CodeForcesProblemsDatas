## Description

<div><p>The company "Divan's Sofas" is planning to build $n + 1$ different buildings on a coordinate line so that: </p><ul> <li> the coordinate of each building is an integer number; </li><li> no two buildings stand at the same point. </li></ul><p>Let $x_i$ be the coordinate of the $i$-th building. To get from the building $i$ to the building $j$, <span class="tex-font-style-it">Divan</span> spends $|x_i - x_j|$ minutes, where $|y|$ is the absolute value of $y$.</p><p>All buildings that <span class="tex-font-style-it">Divan</span> is going to build can be numbered from $0$ to $n$. The businessman will live in the building $0$, the new headquarters of "Divan's Sofas". In the first ten years after construction <span class="tex-font-style-it">Divan</span> will visit the $i$-th building $a_i$ times, each time spending $2 \cdot |x_0-x_i|$ minutes for walking.</p><p><span class="tex-font-style-it">Divan</span> asks you to choose the coordinates for all $n + 1$ buildings so that over the next ten years the businessman will spend as little time for walking as possible.</p></div><div class="input-specification"><p>Each test contains several test cases. The first line contains one integer number $t$ ($1 \le t \le 10^3$) — the number of test cases.</p><p>The first line of each case contains an integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of buildings that "Divan's Sofas" is going to build, apart from the headquarters.</p><p>The second line contains the sequence $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^6$), where $a_i$ is the number of visits to the $i$-th building.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, on the first line print the number $T$ — the minimum time <span class="tex-font-style-it">Divan</span> will spend walking. </p><p>On the second line print the sequence $x_0, x_1, \ldots, x_n$ of $n + 1$ integers, where $x_i$ ($-10^6 \le x_i \le 10^6$) is the selected coordinate of the $i$-th building. It can be shown that an optimal answer exists with coordinates not exceeding $10^6$.</p><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>Each test contains several test cases. The first line contains one integer number $t$ ($1 \le t \le 10^3$) — the number of test cases.</p><p>The first line of each case contains an integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of buildings that "Divan's Sofas" is going to build, apart from the headquarters.</p><p>The second line contains the sequence $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^6$), where $a_i$ is the number of visits to the $i$-th building.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, on the first line print the number $T$ — the minimum time <span class="tex-font-style-it">Divan</span> will spend walking. </p><p>On the second line print the sequence $x_0, x_1, \ldots, x_n$ of $n + 1$ integers, where $x_i$ ($-10^6 \le x_i \le 10^6$) is the selected coordinate of the $i$-th building. It can be shown that an optimal answer exists with coordinates not exceeding $10^6$.</p><p>If there are multiple answers, print any of them.</p>





```input1
4
3
1 2 3
5
3 8 10 6 1
5
1 1 1 1 1
1
0
```




```output1
14
2 4 1 3
78
1 -1 0 2 3 4
18
3 6 1 5 2 4
0
1 2
```



## Note

<p>Let's look at the first example.</p><p><span class="tex-font-style-it">Divan</span> will visit the first building $a_1 = 1$ times, the second $a_2 = 2$ times and the third $a_3 = 3$ times. Then one of the optimal solution will be as follows: </p><ol> <li> the headquarters is located in $x_0 = 2$; </li><li> $x_1 = 4$: <span class="tex-font-style-it">Divan</span> will spend $2 \cdot |x_0-x_1| \cdot a_1 = 2 \cdot |2-4| \cdot 1 = 4$ minutes walking to the first building; </li><li> $x_2 = 1$: <span class="tex-font-style-it">Divan</span> will spend $2 \cdot |x_0-x_2| \cdot a_2 = 2 \cdot |2-1| \cdot 2 = 4$ minutes walking to the second building; </li><li> $x_3 = 3$: <span class="tex-font-style-it">Divan</span> will spend $2 \cdot |x_0-x_3| \cdot a_3 = 2 \cdot |2-3| \cdot 3 = 6$ minutes walking to the third building. </li></ol><p>In total, <span class="tex-font-style-it">Divan</span> will spend $4 + 4 + 6 = 14$ minutes. It can be shown that it is impossible to arrange buildings so that the businessman spends less time.</p><p>Among others, $x = [1, 3, 2, 0]$, $x = [-5, -3, -6, -4]$ are also correct answers for the first example.</p>
