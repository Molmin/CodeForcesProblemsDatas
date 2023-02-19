## Description

<div><p>Masha meets a new friend and learns his phone number&nbsp;— $s$. She wants to remember it as soon as possible. The phone number&nbsp;— is a string of length $m$ that consists of digits from $0$ to $9$. The phone number may start with <span class="tex-font-style-tt">0</span>.</p><p>Masha already knows $n$ phone numbers (all numbers have the same length $m$). It will be easier for her to remember a new number if the $s$ is represented as segments of numbers she already knows. Each such segment must be of length <span class="tex-font-style-bf">at least $2$</span>, otherwise there will be too many segments and Masha will get confused.</p><p>For example, Masha needs to remember the number: $s = $ '<span class="tex-font-style-tt">12345678</span>' and she already knows $n = 4$ numbers: '<span class="tex-font-style-tt">12340219</span>', '<span class="tex-font-style-tt">20215601</span>', '<span class="tex-font-style-tt">56782022</span>', '<span class="tex-font-style-tt">12300678</span>'. You can represent $s$ as a $3$ segment: '<span class="tex-font-style-tt">1234</span>' of number one, '<span class="tex-font-style-tt">56</span>' of number two, and '<span class="tex-font-style-tt">78</span>' of number three. There are other ways to represent $s$.</p><p>Masha asks you for help, she asks you to break the string $s$ into segments of length $2$ or more of the numbers she already knows. If there are several possible answers, print <span class="tex-font-style-bf">any</span> of them.</p></div><div class="input-specification"><p>The first line of input data contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;—the number of test cases.</p><p>Before each test case there is a blank line. Then there is a line containing integers $n$ and $m$ ($1 \le n, m \le 10^3$)&nbsp;—the number of phone numbers that Masha knows and the number of digits in each phone number. Then follow $n$ line, $i$-th of which describes the $i$-th number that Masha knows. The next line contains the phone number of her new friend $s$.</p><p>Among the given $n+1$ phones, there may be duplicates (identical phones).</p><p>It is guaranteed that the sum of $n \cdot m$ ($n$ multiplied by $m$) values over all input test cases does not exceed $10^6$.</p></div><div class="output-specification"><p>You need to print the answers to $t$ test cases. The first line of the answer should contain one number $k$, corresponding to the number of segments into which you split the phone number $s$. Print <span class="tex-font-style-tt">-1</span> if you cannot get such a split.</p><p>If the answer is yes, then follow $k$ lines containing triples of numbers $l, r, i$. Such triplets mean that the next $r-l+1$ digits of number $s$ are equal to a segment (substring) with boundaries $[l, r]$ of the phone under number $i$. Both the phones and the digits in them are numbered from $1$. Note that $r-l+1 \ge 2$ for all $k$ lines.</p></div>

## Input

<p>The first line of input data contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;—the number of test cases.</p><p>Before each test case there is a blank line. Then there is a line containing integers $n$ and $m$ ($1 \le n, m \le 10^3$)&nbsp;—the number of phone numbers that Masha knows and the number of digits in each phone number. Then follow $n$ line, $i$-th of which describes the $i$-th number that Masha knows. The next line contains the phone number of her new friend $s$.</p><p>Among the given $n+1$ phones, there may be duplicates (identical phones).</p><p>It is guaranteed that the sum of $n \cdot m$ ($n$ multiplied by $m$) values over all input test cases does not exceed $10^6$.</p>

## Output

<p>You need to print the answers to $t$ test cases. The first line of the answer should contain one number $k$, corresponding to the number of segments into which you split the phone number $s$. Print <span class="tex-font-style-tt">-1</span> if you cannot get such a split.</p><p>If the answer is yes, then follow $k$ lines containing triples of numbers $l, r, i$. Such triplets mean that the next $r-l+1$ digits of number $s$ are equal to a segment (substring) with boundaries $[l, r]$ of the phone under number $i$. Both the phones and the digits in them are numbered from $1$. Note that $r-l+1 \ge 2$ for all $k$ lines.</p>





```input1|2,3,4,5,6,7,8,14,15,16,17,25,26,27,28,29,30,31
5
<br>
4 8
12340219
20215601
56782022
12300678
12345678
<br>
2 3
134
126
123
<br>
1 4
1210
1221
<br>
4 3
251
064
859
957
054
<br>
4 7
7968636
9486033
4614224
5454197
9482268
```




```output1
3
1 4 1
5 6 2
3 4 3
-1
2
1 2 1
2 3 1
-1
3
1 3 2
5 6 3
3 4 1
```



## Note

<p>The example from the statement.</p><p>In the second case, it is impossible to represent by segments of known numbers of length 2 or more.</p><p>In the third case, you can get the segments '<span class="tex-font-style-tt">12</span>' and '<span class="tex-font-style-tt">21</span>' from the first phone number.</p>
