## Description

<div><p>AquaMoon had $n$ strings of length $m$ each. $n$ is an <span class="tex-font-style-bf">odd</span> number.</p><p>When AquaMoon was gone, Cirno tried to pair these $n$ strings together. After making $\frac{n-1}{2}$ pairs, she found out that there was exactly one string without the pair!</p><p>In her rage, she disrupted each pair of strings. For each pair, she selected some positions (at least $1$ and at most $m$) and swapped the letters in the two strings of this pair at the selected positions.</p><p>For example, if $m = 6$ and two strings "<span class="tex-font-style-tt">abcdef</span>" and "<span class="tex-font-style-tt">xyzklm</span>" are in one pair and Cirno selected positions $2$, $3$ and $6$ she will swap '<span class="tex-font-style-tt">b</span>' with '<span class="tex-font-style-tt">y</span>', '<span class="tex-font-style-tt">c</span>' with '<span class="tex-font-style-tt">z</span>' and '<span class="tex-font-style-tt">f</span>' with '<span class="tex-font-style-tt">m</span>'. The resulting strings will be "<span class="tex-font-style-tt">ayzdem</span>" and "<span class="tex-font-style-tt">xbcklf</span>".</p><p>Cirno then stole away the string without pair and shuffled all remaining strings in arbitrary order.</p><p>AquaMoon found the remaining $n-1$ strings in complete disarray. Also, she remembers the initial $n$ strings. She wants to know which string was stolen, but she is not good at programming. Can you help her?</p></div><div class="input-specification"><p><span class="tex-font-style-bf">This problem is made as interactive. It means, that your solution will read the input, given by the interactor. But the interactor will give you the full input at the beginning and after that, you should print the answer. So you should solve the problem, like as you solve the usual, non-interactive problem because you won't have any interaction process. The only thing you should not forget is to flush the output buffer, after printing the answer. Otherwise, you can get an "Idleness limit exceeded" verdict. Refer to the <a href="https://codeforces.com/blog/entry/45307">interactive problems guide</a> for the detailed information about flushing the output buffer.</span></p><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 100$) — the number of test cases.</p><p>The first line of each test case contains two integers $n$, $m$ ($1 \leq n \leq 10^5$, $1 \leq m \leq 10^5$) — the number of strings and the length of each string, respectively.</p><p>The next $n$ lines each contain a string with length $m$, describing the original $n$ strings. All string consists of lowercase Latin letters.</p><p>The next $n-1$ lines each contain a string with length $m$, describing the strings after Cirno exchanged and reordered them.</p><p>It is guaranteed that $n$ is odd and that the sum of $n \cdot m$ over all test cases does not exceed $10^5$.</p><p><span class="tex-font-style-bf">Hack format</span>:</p><p>The first line should contain a single integer $t$. After that $t$ test cases should follow in the following format:</p><p>The first line should contain two integers $n$ and $m$.</p><p>The following $n$ lines should contain $n$ strings of length $m$, describing the original strings.</p><p>The following $\frac{n-1}{2}$ lines should describe the pairs. They should contain, in the following order: the index of the first string $i$ ($1 \leq i \leq n$), the index of the second string $j$ ($1 \leq j \leq n$, $i \neq j$), the number of exchanged positions $k$ ($1 \leq k \leq m$), and the list of $k$ positions that are exchanged ($k$ distinct indices from $1$ to $m$ in any order).</p><p>The final line should contain a permutation of integers from $1$ to $n$, describing the way the strings should be reordered. The strings will be placed in the order indices placed in this permutation, the stolen string index will be ignored.</p></div><div class="output-specification"><p>For each test case print a single line with the stolen string.</p></div>

## Input

<p><span class="tex-font-style-bf">This problem is made as interactive. It means, that your solution will read the input, given by the interactor. But the interactor will give you the full input at the beginning and after that, you should print the answer. So you should solve the problem, like as you solve the usual, non-interactive problem because you won't have any interaction process. The only thing you should not forget is to flush the output buffer, after printing the answer. Otherwise, you can get an "Idleness limit exceeded" verdict. Refer to the <a href="https://codeforces.com/blog/entry/45307">interactive problems guide</a> for the detailed information about flushing the output buffer.</span></p><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 100$) — the number of test cases.</p><p>The first line of each test case contains two integers $n$, $m$ ($1 \leq n \leq 10^5$, $1 \leq m \leq 10^5$) — the number of strings and the length of each string, respectively.</p><p>The next $n$ lines each contain a string with length $m$, describing the original $n$ strings. All string consists of lowercase Latin letters.</p><p>The next $n-1$ lines each contain a string with length $m$, describing the strings after Cirno exchanged and reordered them.</p><p>It is guaranteed that $n$ is odd and that the sum of $n \cdot m$ over all test cases does not exceed $10^5$.</p><p><span class="tex-font-style-bf">Hack format</span>:</p><p>The first line should contain a single integer $t$. After that $t$ test cases should follow in the following format:</p><p>The first line should contain two integers $n$ and $m$.</p><p>The following $n$ lines should contain $n$ strings of length $m$, describing the original strings.</p><p>The following $\frac{n-1}{2}$ lines should describe the pairs. They should contain, in the following order: the index of the first string $i$ ($1 \leq i \leq n$), the index of the second string $j$ ($1 \leq j \leq n$, $i \neq j$), the number of exchanged positions $k$ ($1 \leq k \leq m$), and the list of $k$ positions that are exchanged ($k$ distinct indices from $1$ to $m$ in any order).</p><p>The final line should contain a permutation of integers from $1$ to $n$, describing the way the strings should be reordered. The strings will be placed in the order indices placed in this permutation, the stolen string index will be ignored.</p>

## Output

<p>For each test case print a single line with the stolen string.</p>





```input1
3
3 5
aaaaa
bbbbb
ccccc
aaaaa
bbbbb
3 4
aaaa
bbbb
cccc
aabb
bbaa
5 6
abcdef
uuuuuu
kekeke
ekekek
xyzklm
xbcklf
eueueu
ayzdem
ukukuk
```




```output1
ccccc
cccc
kekeke
```



## Note

<p>In the first test case, "<span class="tex-font-style-tt">aaaaa</span>" and "<span class="tex-font-style-tt">bbbbb</span>" exchanged all positions, and "<span class="tex-font-style-tt">ccccc</span>" is the stolen string.</p><p>In the second test case, "<span class="tex-font-style-tt">aaaa</span>" and "<span class="tex-font-style-tt">bbbb</span>" exchanged two first positions, and "<span class="tex-font-style-tt">cccc</span>" is the stolen string.</p><p>This is the first test in the hack format: </p><pre class="verbatim"><br>3<br>3 5<br>aaaaa<br>bbbbb<br>ccccc<br>1 2 5 1 2 3 4 5<br>2 1 3<br>3 4<br>aaaa<br>bbbb<br>cccc<br>1 2 2 1 2<br>2 1 3<br>5 6<br>abcdef<br>uuuuuu<br>kekeke<br>ekekek<br>xyzklm<br>1 5 3 2 3 6<br>2 4 3 2 4 6<br>5 4 1 2 3<br></pre>
