## Description

<div><p>You are given a sequence $a=[a_1,a_2,\dots,a_n]$ consisting of $n$ <span class="tex-font-style-bf">positive</span> integers.</p><p>Let's call a group of consecutive elements a <span class="tex-font-style-it">segment</span>. Each <span class="tex-font-style-it">segment</span> is characterized by two indices: the index of its left end and the index of its right end. Denote by $a[l,r]$ a <span class="tex-font-style-it">segment</span> of the sequence $a$ with the left end in $l$ and the right end in $r$, i.e. $a[l,r]=[a_l, a_{l+1}, \dots, a_r]$.</p><p>For example, if $a=[31,4,15,92,6,5]$, then $a[2,5]=[4,15,92,6]$, $a[5,5]=[6]$, $a[1,6]=[31,4,15,92,6,5]$ are <span class="tex-font-style-it">segments</span>.</p><p>We split the given sequence $a$ into <span class="tex-font-style-it">segments</span> so that: </p><ul> <li> each element is in <span class="tex-font-style-bf">exactly</span> one <span class="tex-font-style-it">segment</span>; </li><li> the sums of elements for all <span class="tex-font-style-it">segments</span> are <span class="tex-font-style-bf">equal</span>. </li></ul><p>For example, if $a$ = [$55,45,30,30,40,100$], then such a sequence can be split into three <span class="tex-font-style-it">segments</span>: $a[1,2]=[55,45]$, $a[3,5]=[30, 30, 40]$, $a[6,6]=[100]$. Each element belongs to exactly <span class="tex-font-style-it">segment</span>, the sum of the elements of each <span class="tex-font-style-it">segment</span> is $100$.</p><p>Let's define <span class="tex-font-style-it">thickness</span> of split as the length of the longest <span class="tex-font-style-it">segment</span>. For example, the thickness of the split from the example above is $3$.</p><p>Find the minimum thickness among all possible splits of the given sequence of $a$ into <span class="tex-font-style-it">segments</span> in the required way.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 100$) — the number of test cases.</p><p>Each test case is described by two lines.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2000$) — the length of the sequence $a$.</p><p>The second line of each test case contains exactly $n$ integers: $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^6$) — elements of the sequence $a$.</p><p>It is guaranteed that the sum of $n$ for all test cases does not exceed $2000$.</p></div><div class="output-specification"><p>For each test case, output one integer — the minimum possible thickness of a split of the sequence $a$ into <span class="tex-font-style-it">segments</span>.</p><p>Note that there always exist a split, you can always consider whole sequence as one segment.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 100$) — the number of test cases.</p><p>Each test case is described by two lines.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2000$) — the length of the sequence $a$.</p><p>The second line of each test case contains exactly $n$ integers: $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^6$) — elements of the sequence $a$.</p><p>It is guaranteed that the sum of $n$ for all test cases does not exceed $2000$.</p>

## Output

<p>For each test case, output one integer — the minimum possible thickness of a split of the sequence $a$ into <span class="tex-font-style-it">segments</span>.</p><p>Note that there always exist a split, you can always consider whole sequence as one segment.</p>





```input1|2,3,6,7
4
6
55 45 30 30 40 100
4
10 23 7 13
5
10 55 35 30 65
6
4 1 1 1 1 4
```




```output1
3
4
2
3
```



## Note

<p>The split in the first test case is explained in the statement, it can be shown that it is optimal.</p><p>In the second test case, it is possible to split into <span class="tex-font-style-it">segments</span> only by leaving a single <span class="tex-font-style-it">segment</span>. Then the thickness of this split is equal to the length of the entire sequence, that is, $4$.</p><p>In the third test case, the optimal split will be $[10, 55], [35, 30], [65]$. The thickness of the split equals to $2$.</p><p>In the fourth test case possible splits are:</p><ul> <li> $[4] + [1, 1, 1, 1] + [4]$; </li><li> $[4, 1, 1] + [1, 1, 4]$. </li></ul>
