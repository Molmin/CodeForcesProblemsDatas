## Description

<div><p><span class="tex-font-style-it">One day Prof. Slim decided to leave the kingdom of the GUC to join the kingdom of the GIU. He was given an easy online assessment to solve before joining the GIU. Citizens of the GUC were <span class="tex-font-style-striked">happy</span> sad to see the prof leaving, so they decided to hack into the system and change the online assessment into a harder one so that he stays at the GUC. After a long argument, they decided to change it into the following problem.</span></p><p>Given an array of $n$ integers $a_1,a_2,\ldots,a_n$, <span class="tex-font-style-bf">where $a_{i} \neq 0$</span>, check if you can make this array sorted by using the following operation any number of times (possibly zero). An array is sorted if its elements are arranged in a non-decreasing order.</p><ol> <li> select two indices $i$ and $j$ ($1 \le i,j \le n$) such that $a_i$ and $a_j$ have <span class="tex-font-style-bf">different signs</span>. In other words, one must be positive and one must be negative. </li><li> swap the <span class="tex-font-style-bf">signs</span> of $a_{i}$ and $a_{j}$. For example if you select $a_i=3$ and $a_j=-2$, then they will change to $a_i=-3$ and $a_j=2$. </li></ol><p>Prof. Slim saw that the problem is still too easy and isn't worth his time, so he decided to give it to you to solve.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^{5}$) — the length of the array $a$.</p><p>The next line contain $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^9 \le a_{i} \le 10^9$, $a_{i} \neq 0$) separated by spaces describing elements of the array $a$. </p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print "<span class="tex-font-style-tt">YES</span>" if the array can be sorted in the non-decreasing order, otherwise print "<span class="tex-font-style-tt">NO</span>". You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^{5}$) — the length of the array $a$.</p><p>The next line contain $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^9 \le a_{i} \le 10^9$, $a_{i} \neq 0$) separated by spaces describing elements of the array $a$. </p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $10^5$.</p>

## Output

<p>For each test case, print "<span class="tex-font-style-tt">YES</span>" if the array can be sorted in the non-decreasing order, otherwise print "<span class="tex-font-style-tt">NO</span>". You can print each letter in any case (upper or lower).</p>





```input1
4
7
7 3 2 -11 -13 -17 -23
6
4 10 25 47 71 96
6
71 -35 7 -4 -11 -25
6
-45 9 -48 -67 -55 7
```




```output1
NO
YES
YES
NO
```



## Note

<p>In the first test case, there is no way to make the array sorted using the operation any number of times.</p><p>In the second test case, the array is already sorted.</p><p>In the third test case, we can swap the sign of the $1$-st element with the sign of the $5$-th element, and the sign of the $3$-rd element with the sign of the $6$-th element, this way the array will be sorted.</p><p>In the fourth test case, there is no way to make the array sorted using the operation any number of times.</p>
