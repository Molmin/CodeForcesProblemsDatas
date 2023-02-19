## Description

<div><p>The girl named Masha was walking in the forest and found a complete binary tree of height $n$ and a permutation $p$ of length $m=2^n$.</p><p>A complete binary tree of height $n$ is a rooted tree such that every vertex except the leaves has exactly two sons, and the length of the path from the root to any of the leaves is $n$. The picture below shows the complete binary tree for $n=2$.</p><p>A permutation is an array consisting of $n$ different integers from $1$ to $n$. For example, [$2,3,1,5,4$] is a permutation, but [$1,2,2$] is not ($2$ occurs twice), and [$1,3,4$] is also not a permutation ($n=3$, but there is $4$ in the array).</p><p>Let's enumerate $m$ leaves of this tree from left to right. The leaf with the number $i$ contains the value $p_i$ ($1 \le i \le m$).</p><p>For example, if $n = 2$, $p = [3, 1, 4, 2]$, the tree will look like this:</p><center> <img class="tex-graphics" src="file://W0UbvmDM.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Masha considers a tree <span class="tex-font-style-it">beautiful</span> if the values in its leaves are ordered from left to right in increasing order.</p><p>In one operation, Masha can choose any non-leaf vertex of the tree and swap its left and right sons (along with their subtrees).</p><p>For example, if Masha applies this operation to the root of the tree discussed above, it will take the following form:</p><center> <img class="tex-graphics" src="file://zaqEs7kj.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Help Masha understand if she can make a tree <span class="tex-font-style-it">beautiful</span> in a certain number of operations. If she can, then output the minimum number of operations to make the tree <span class="tex-font-style-it">beautiful</span>.</p></div><div class="input-specification"><p>The first line contains single integer $t$ ($1 \le t \le 10^4$)&nbsp;— number of test cases.</p><p>In each test case, the first line contains an integer $m$ ($1 \le m \le 262144$), which is a power of two &nbsp;— the size of the permutation $p$.</p><p>The second line contains $m$ integers: $p_1, p_2, \dots, p_m$ ($1 \le p_i \le m$)&nbsp;— the permutation $p$.</p><p>It is guaranteed that the sum of $m$ over all test cases does not exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case in a separate line, print the minimum possible number of operations for which Masha will be able to make the tree <span class="tex-font-style-it">beautiful</span> or <span class="tex-font-style-tt">-1</span>, if this is not possible.</p></div>

## Input

<p>The first line contains single integer $t$ ($1 \le t \le 10^4$)&nbsp;— number of test cases.</p><p>In each test case, the first line contains an integer $m$ ($1 \le m \le 262144$), which is a power of two &nbsp;— the size of the permutation $p$.</p><p>The second line contains $m$ integers: $p_1, p_2, \dots, p_m$ ($1 \le p_i \le m$)&nbsp;— the permutation $p$.</p><p>It is guaranteed that the sum of $m$ over all test cases does not exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case in a separate line, print the minimum possible number of operations for which Masha will be able to make the tree <span class="tex-font-style-it">beautiful</span> or <span class="tex-font-style-tt">-1</span>, if this is not possible.</p>





```input1|2,3,6,7
4
8
6 5 7 8 4 3 1 2
4
3 1 4 2
1
1
8
7 8 4 3 1 2 6 5
```




```output1
4
-1
0
-1
```



## Note

<p>Consider the first test.</p><p>In the first test case, you can act like this (the vertex to which the operation is applied at the current step is highlighted in purple): </p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="file://wH1Y2THa.png" style="max-width: 100.0%;max-height: 100.0%;"></td><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="file://MuttEega.png" style="max-width: 100.0%;max-height: 100.0%;"></td></tr><tr><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="file://X696ctWY.png" style="max-width: 100.0%;max-height: 100.0%;"></td><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="file://zQBcWFjj.png" style="max-width: 100.0%;max-height: 100.0%;"></td></tr></tbody></table> </center> It can be shown that it is impossible to make a tree <span class="tex-font-style-it">beautiful</span> in fewer operations.<p>In the second test case, it can be shown that it is impossible to make a tree <span class="tex-font-style-it">beautiful</span>.</p><p>In the third test case, the tree is already <span class="tex-font-style-it">beautiful</span>.</p>
