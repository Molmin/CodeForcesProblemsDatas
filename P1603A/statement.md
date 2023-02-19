## Description

<div><p>YouKn0wWho has an integer sequence $a_1, a_2, \ldots, a_n$. He will perform the following operation until the sequence becomes empty: select an index $i$ such that $1 \le i \le |a|$ and $a_i$ is <span class="tex-font-style-bf">not</span> divisible by $(i + 1)$, and erase this element from the sequence. Here $|a|$ is the length of sequence $a$ at the moment of operation. Note that the sequence $a$ changes and the next operation is performed on this changed sequence.</p><p>For example, if $a=[3,5,4,5]$, then he can select $i = 2$, because $a_2 = 5$ is not divisible by $i+1 = 3$. After this operation the sequence is $[3,4,5]$.</p><p>Help YouKn0wWho determine if it is possible to erase the whole sequence using the aforementioned operation.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10\,000$) &nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print "<span class="tex-font-style-tt">YES</span>" (without quotes) if it is possible to erase the whole sequence using the aforementioned operation, print "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise. You can print each letter in any register (upper or lower).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10\,000$) &nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case, print "<span class="tex-font-style-tt">YES</span>" (without quotes) if it is possible to erase the whole sequence using the aforementioned operation, print "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise. You can print each letter in any register (upper or lower).</p>





```input1
5
3
1 2 3
1
2
2
7 7
10
384836991 191890310 576823355 782177068 404011431 818008580 954291757 160449218 155374934 840594328
8
6 69 696 69696 696969 6969696 69696969 696969696
```




```output1
YES
NO
YES
YES
NO
```



## Note

<p>In the first test case, YouKn0wWho can perform the following operations (the erased elements are underlined): $[1, \underline{2}, 3] \rightarrow [\underline{1}, 3] \rightarrow [\underline{3}] \rightarrow [\,].$</p><p>In the second test case, it is impossible to erase the sequence as $i$ can only be $1$, and when $i=1$, $a_1 = 2$ is divisible by $i + 1 = 2$.</p>
