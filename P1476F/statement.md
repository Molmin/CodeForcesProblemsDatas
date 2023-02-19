## Description

<div><p>There are $n$ lanterns in a row. The lantern $i$ is placed in position $i$ and has power equal to $p_i$.</p><p>Each lantern can be directed to illuminate either some lanterns to the left or some lanterns to the right. If the $i$-th lantern is turned to the left, it illuminates all such lanterns $j$ that $j \in [i - p_i, i - 1]$. Similarly, if it is turned to the right, it illuminates all such lanterns $j$ that $j \in [i + 1, i + p_i]$.</p><p>Your goal is to choose a direction for each lantern so each lantern is illuminated by at least one other lantern, or report that it is impossible.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10000$) — the number of test cases.</p><p>Each test case consists of two lines. The first line contains one integer $n$ ($2 \le n \le 3 \cdot 10^5$) — the number of lanterns.</p><p>The second line contains $n$ integers $p_1, p_2, \dots, p_n$ ($0 \le p_i \le n$) — the power of the $i$-th lantern.</p><p>The sum of $n$ over all test cases does not exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print the answer as follows:</p><p>If it is possible to direct all lanterns so that each lantern is illuminated, print <span class="tex-font-style-tt">YES</span> in the first line and a string of $n$ characters <span class="tex-font-style-tt">L</span> and/or <span class="tex-font-style-tt">R</span> (the $i$-th character is <span class="tex-font-style-tt">L</span> if the $i$-th lantern is turned to the left, otherwise this character is <span class="tex-font-style-tt">R</span>) in the second line. If there are multiple answers, you may print any of them.</p><p>If there is no answer, simply print <span class="tex-font-style-tt">NO</span> for that test case.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10000$) — the number of test cases.</p><p>Each test case consists of two lines. The first line contains one integer $n$ ($2 \le n \le 3 \cdot 10^5$) — the number of lanterns.</p><p>The second line contains $n$ integers $p_1, p_2, \dots, p_n$ ($0 \le p_i \le n$) — the power of the $i$-th lantern.</p><p>The sum of $n$ over all test cases does not exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case, print the answer as follows:</p><p>If it is possible to direct all lanterns so that each lantern is illuminated, print <span class="tex-font-style-tt">YES</span> in the first line and a string of $n$ characters <span class="tex-font-style-tt">L</span> and/or <span class="tex-font-style-tt">R</span> (the $i$-th character is <span class="tex-font-style-tt">L</span> if the $i$-th lantern is turned to the left, otherwise this character is <span class="tex-font-style-tt">R</span>) in the second line. If there are multiple answers, you may print any of them.</p><p>If there is no answer, simply print <span class="tex-font-style-tt">NO</span> for that test case.</p>





```input1
4
8
0 0 3 1 1 1 1 2
2
1 1
2
2 2
2
0 1
```




```output1
YES
RRLLLLRL
YES
RL
YES
RL
NO
```


