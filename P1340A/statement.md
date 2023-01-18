## Description

<div><p><span class="tex-font-style-it"> Denis was very sad after Nastya rejected him. So he decided to walk through the gateways to have some fun. And luck smiled at him! When he entered the first courtyard, he met a strange man who was selling something. </span></p><p>Denis bought a mysterious item and it was... Random permutation generator! Denis could not believed his luck.</p><p>When he arrived home, he began to study how his generator works and learned the algorithm. The process of generating a permutation consists of $n$ steps. At the $i$-th step, a place is chosen for the number $i$ $(1 \leq i \leq n)$. The position for the number $i$ is defined as follows:</p><ul> <li> For all $j$ from $1$ to $n$, we calculate $r_j$ &nbsp;— the minimum index such that $j \leq r_j \leq n$, and the position $r_j$ is not yet occupied in the permutation. If there are no such positions, then we assume that the value of $r_j$ is not defined. </li><li> For all $t$ from $1$ to $n$, we calculate $count_t$ &nbsp;— the number of positions $1 \leq j \leq n$ such that $r_j$ is defined and $r_j = t$. </li><li> Consider the positions that are still not occupied by permutation and among those we consider the positions for which the value in the $count$ array is maximum. </li><li> The generator selects one of these positions for the number $i$. The generator can choose <span class="tex-font-style-bf">any</span> position. </li></ul><p>Let's have a look at the operation of the algorithm in the following example:</p><center> <img class="tex-graphics" src="file://whbwkZ4Q.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Let $n = 5$ and the algorithm has already arranged the numbers $1, 2, 3$ in the permutation. Consider how the generator will choose a position for the number $4$:</p><ul> <li> The values of $r$ will be $r = [3, 3, 3, 4, \times]$, where $\times$ means an indefinite value. </li><li> Then the $count$ values will be $count = [0, 0, 3, 1, 0]$. </li><li> There are only two unoccupied positions in the permutation: $3$ and $4$. The value in the $count$ array for position $3$ is $3$, for position $4$ it is $1$. </li><li> The maximum value is reached only for position $3$, so the algorithm will uniquely select this position for number $4$. </li></ul><p>Satisfied with his purchase, Denis went home. For several days without a break, he generated permutations. He believes that he can come up with random permutations no worse than a generator. After that, he wrote out the first permutation that came to mind $p_1, p_2, \ldots, p_n$ and decided to find out if it could be obtained as a result of the generator.</p><p>Unfortunately, this task was too difficult for him, and he asked you for help. It is necessary to define whether the written permutation could be obtained using the described algorithm if the generator always selects the position Denis needs.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ $(1 \leq t \leq 10^5)$ &nbsp;— the number of test cases. Then the descriptions of the test cases follow.</p><p>The first line of the test case contains a single integer $n$ $(1 \leq n \leq 10^5)$ &nbsp;— the size of the permutation.</p><p>The second line of the test case contains $n$ different integers $p_1, p_2, \ldots, p_n$ ($1 \leq p_i \leq n$) &nbsp;— the permutation written by Denis.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $10^5$.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">Yes</span>" if this permutation could be obtained as a result of the generator. Otherwise, print "<span class="tex-font-style-tt">No</span>".</p><p>All letters can be displayed in any case.</p></div>

## Input

<p>The first line contains a single integer $t$ $(1 \leq t \leq 10^5)$ &nbsp;— the number of test cases. Then the descriptions of the test cases follow.</p><p>The first line of the test case contains a single integer $n$ $(1 \leq n \leq 10^5)$ &nbsp;— the size of the permutation.</p><p>The second line of the test case contains $n$ different integers $p_1, p_2, \ldots, p_n$ ($1 \leq p_i \leq n$) &nbsp;— the permutation written by Denis.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $10^5$.</p>

## Output

<p>Print "<span class="tex-font-style-tt">Yes</span>" if this permutation could be obtained as a result of the generator. Otherwise, print "<span class="tex-font-style-tt">No</span>".</p><p>All letters can be displayed in any case.</p>





```input1
5
5
2 3 4 5 1
1
1
3
1 3 2
4
4 2 3 1
5
1 5 2 4 3
```




```output1
Yes
Yes
No
Yes
No
```



## Note

<p>Let's simulate the operation of the generator in the first test.</p><p>At the $1$ step, $r = [1, 2, 3, 4, 5], count = [1, 1, 1, 1, 1]$. The maximum value is reached in any free position, so the generator can choose a random position from $1$ to $5$. In our example, it chose $5$.</p><p>At the $2$ step, $r = [1, 2, 3, 4, \times], count = [1, 1, 1, 1, 0]$. The maximum value is reached in positions from $1$ to $4$, so the generator can choose a random position among them. In our example, it chose $1$.</p><p>At the $3$ step, $r = [2, 2, 3, 4, \times], count = [0, 2, 1, 1, 0]$. The maximum value is $2$ and is reached only at the $2$ position, so the generator will choose this position.</p><p>At the $4$ step, $r = [3, 3, 3, 4, \times], count = [0, 0, 3, 1, 0]$. The maximum value is $3$ and is reached only at the $3$ position, so the generator will choose this position.</p><p>At the $5$ step, $r = [4, 4, 4, 4, \times], count = [0, 0, 0, 4, 0]$. The maximum value is $4$ and is reached only at the $4$ position, so the generator will choose this position.</p><p>In total, we got a permutation of $2, 3, 4, 5, 1$, that is, a generator could generate it.</p>
