## Description

<div><p>The gardener Kazimir Kazimirovich has an array of $n$ integers $c_1, c_2, \dots, c_n$.</p><p>He wants to check if there are two different subsequences $a$ and $b$ of the original array, for which $f(a) = f(b)$, where $f(x)$ is the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#OR">bitwise OR</a> of all of the numbers in the sequence $x$.</p><p>A sequence $q$ is a subsequence of $p$ if $q$ can be obtained from $p$ by deleting several (possibly none or all) elements.</p><p>Two subsequences are considered different if the sets of indexes of their elements in the original sequence are different, that is, the values of the elements are not considered when comparing the subsequences.</p><center> <img class="tex-graphics" src="file://hzpFLnIE.png" style="max-width: 100.0%;max-height: 100.0%;"> </center></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^5$). The description of the test cases follows.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 10^5$)&nbsp;— the size of the array $c$.</p><p>The description of the array $c$ in this problem is given implicitly to speed up input.</p><p>The $(i + 1)$-st of the following $n$ lines of the test case begins with an integer $k_i$ ($1 \le k_i \le 10^5$)&nbsp;— the number of set bits in the number $c_i$. Next follow $k_i$ distinct integers $p_{i, 1}, p_{i, 2}, \dots, p_{i, k_i}$ ($1 \le p_i \le 2 \cdot 10^5$)&nbsp;—the numbers of bits that are set to one in number $c_i$. In other words, $c_i = 2^{p_{i, 1}} + 2^{p_{i, 2}} + \ldots + 2^{p_{i, k_i}}$.</p><p>It is guaranteed that the total sum of $k_i$ in all tests does not exceed $10^5$.</p></div><div class="output-specification"><p>For each set of input, print "<span class="tex-font-style-tt">Yes</span>" if there exist two different subsequences for which $f(a) = f(b)$, and "<span class="tex-font-style-tt">No</span>" otherwise.</p><p>You can output the answer in any case (upper or lower). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as positive responses.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^5$). The description of the test cases follows.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 10^5$)&nbsp;— the size of the array $c$.</p><p>The description of the array $c$ in this problem is given implicitly to speed up input.</p><p>The $(i + 1)$-st of the following $n$ lines of the test case begins with an integer $k_i$ ($1 \le k_i \le 10^5$)&nbsp;— the number of set bits in the number $c_i$. Next follow $k_i$ distinct integers $p_{i, 1}, p_{i, 2}, \dots, p_{i, k_i}$ ($1 \le p_i \le 2 \cdot 10^5$)&nbsp;—the numbers of bits that are set to one in number $c_i$. In other words, $c_i = 2^{p_{i, 1}} + 2^{p_{i, 2}} + \ldots + 2^{p_{i, k_i}}$.</p><p>It is guaranteed that the total sum of $k_i$ in all tests does not exceed $10^5$.</p>

## Output

<p>For each set of input, print "<span class="tex-font-style-tt">Yes</span>" if there exist two different subsequences for which $f(a) = f(b)$, and "<span class="tex-font-style-tt">No</span>" otherwise.</p><p>You can output the answer in any case (upper or lower). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as positive responses.</p>





```input1|2,3,4,5,9,10,11,12,13,20,21,22
5
3
2 1 5
2 2 4
2 2 3
2
2 1 2
1 2
4
3 1 2 4
2 2 4
4 1 2 5 6
2 2 5
5
3 3 1 2
3 2 5 3
5 7 2 3 1 4
5 1 2 6 3 5
3 2 6 3
2
1 1
1 2
```




```output1
No
Yes
Yes
Yes
No
```



## Note

<p>It can be proven that in the first test case there are no two different subsequences $a$ and $b$ for which $f(a) = f(b)$.</p><p>In the second test case, one of the possible answers are following subsequences: the subsequence $a$ formed by the element at position $1$, and the subsequence $b$ formed by the elements at positions $1$ and $2$.</p><p>In the third test case, one of the possible answers are following subsequences: the subsequence $a$ formed by elements at positions $1$, $2$, $3$ and $4$, and the subsequence $b$ formed by elements at positions $2$, $3$ and $4$.</p>
