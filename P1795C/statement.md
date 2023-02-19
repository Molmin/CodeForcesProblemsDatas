## Description

<div><p>A tea manufacturer decided to conduct a massive tea tasting. $n$ sorts of tea will be tasted by $n$ tasters. Both the sorts of tea and the tasters are numbered from $1$ to $n$. The manufacturer prepared $a_i$ milliliters of the $i$-th sort of tea. The $j$-th taster can drink $b_j$ milliliters of tea at once.</p><p>The tasting will be conducted in steps. During the first step, the $i$-th taster tastes the $i$-th sort of tea. The $i$-th taster drinks $\min(a_i, b_i)$ tea (how much is available of the $i$-th sort and how much the $i$-th taster can drink). $a_i$ also decreases by this amount.</p><p>Then all tasters move to the previous sort of tea. Thus, during the second step, the $i$-th taster tastes the $(i-1)$-st sort of tea. The $i$-th taster drinks $\min(a_{i-1}, b_i)$ tea. The $1$-st person ends the tasting.</p><p>During the third step, the $i$-th taster tastes the $(i-2)$-nd sort of tea. The $2$-nd taster ends the tasting. This goes on until everyone ends the tasting.</p><p>Take a look at the tasting process for $n = 3$, $a = [10, 20, 15]$, $b = [9, 8, 6]$. In the left row, there are the current amounts of each sort of tea. In the right column, there are current amounts of tea each taster has drunk in total. The arrow tells which taster each tea goes to on the current step. The number on the arrow is the amount&nbsp;— minimum of how much is available of the sort of tea and how much the taster can drink.</p><center> <img class="tex-graphics" src="file://SoPve5zQ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>For each taster, print how many milliliters of tea he/she will drink in total.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the number of sorts of tea and the number of tasters.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the amount of each sort of tea.</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_i \le 10^9$)&nbsp;— the amount of tea each taster can drink at once.</p><p>The sum of $n$ over all testcases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each testcase, print $n$ integers&nbsp;— the $i$-th value should be equal to the total amount of tea the $i$-th taster will drink.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the number of sorts of tea and the number of tasters.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the amount of each sort of tea.</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_i \le 10^9$)&nbsp;— the amount of tea each taster can drink at once.</p><p>The sum of $n$ over all testcases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each testcase, print $n$ integers&nbsp;— the $i$-th value should be equal to the total amount of tea the $i$-th taster will drink.</p>





```input1|2,3,4,8,9,10
4
3
10 20 15
9 8 6
1
5
7
4
13 8 5 4
3 4 2 1
3
1000000000 1000000000 1000000000
1 1 1000000000
```




```output1
9 9 12 
5 
3 8 6 4 
1 2 2999999997
```



## Note

<p>The first testcase is described in the statement. Here are the remaining amounts of each sort of tea <span class="tex-font-style-it">after</span> each step and the total amount of tea each taster has drunk: </p><ul> <li> $a = [1, 12, 9]$, $\mathit{ans} = [9, 8, 6]$ </li><li> $a = [0, 6, 9]$, $\mathit{ans} = [9, 9, 12]$ </li><li> $a = [0, 6, 9]$, $\mathit{ans} = [9, 9, 12]$ </li></ul><p>In the second testcase, the only taster drinks $\min(5, 7)$ milliliters of tea of the only sort.</p><p>Here are the remaining amounts of each sort of tea <span class="tex-font-style-it">after</span> each step and the total amount of tea each taster has drunk for the third testcase: </p><ul> <li> $a = [10, 4, 3, 3]$, $\mathit{ans} = [3, 4, 2, 1]$; </li><li> $a = [6, 2, 2, 3]$, $\mathit{ans} = [3, 8, 4, 2]$; </li><li> $a = [4, 1, 2, 3]$, $\mathit{ans} = [3, 8, 6, 3]$; </li><li> $a = [3, 1, 2, 3]$, $\mathit{ans} = [3, 8, 6, 4]$. </li></ul><p>Here are the remaining amounts of each sort of tea <span class="tex-font-style-it">after</span> each step and the total amount of tea each taster has drunk for the fourth testcase: </p><ul> <li> $a = [999999999, 999999999, 0]$, $\mathit{ans} = [1, 1, 1000000000]$; </li><li> $a = [999999998, 0, 0]$, $\mathit{ans} = [1, 2, 1999999999]$; </li><li> $a = [0, 0, 0]$, $\mathit{ans} = [1, 2, 2999999997]$. </li></ul>
