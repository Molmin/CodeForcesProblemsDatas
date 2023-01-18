## Description

<div><p>JATC loves Banh-mi (a Vietnamese food). His affection for Banh-mi is so much that he always has it for breakfast. This morning, as usual, he buys a Banh-mi and decides to enjoy it in a special way.</p><p>First, he splits the Banh-mi into $n$ parts, places them on a row and numbers them from $1$ through $n$. For each part $i$, he defines the <span class="tex-font-style-it">deliciousness</span> of the part as $x_i \in \{0, 1\}$. JATC's going to eat those parts one by one. At each step, he chooses arbitrary remaining part and eats it. Suppose that part is the $i$-th part then his <span class="tex-font-style-it">enjoyment</span> of the Banh-mi will increase by $x_i$ and the deliciousness of all the remaining parts will also increase by $x_i$. The initial enjoyment of JATC is equal to $0$.</p><p>For example, suppose the deliciousness of $3$ parts are $[0, 1, 0]$. If JATC eats the second part then his enjoyment will become $1$ and the deliciousness of remaining parts will become $[1, \_, 1]$. Next, if he eats the first part then his enjoyment will become $2$ and the remaining parts will become $[\_, \_, 2]$. After eating the last part, JATC's enjoyment will become $4$.</p><p>However, JATC doesn't want to eat all the parts but to save some for later. He gives you $q$ queries, each of them consisting of two integers $l_i$ and $r_i$. For each query, you have to let him know what is the maximum enjoyment he can get if he eats all the parts with indices in the range $[l_i, r_i]$ in some order.</p><p>All the queries are independent of each other. Since the answer to the query could be very large, print it modulo $10^9+7$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($1 \le n, q \le 100\,000$).</p><p>The second line contains a string of $n$ characters, each character is either '<span class="tex-font-style-tt">0</span>' or '<span class="tex-font-style-tt">1</span>'. The $i$-th character defines the deliciousness of the $i$-th part.</p><p>Each of the following $q$ lines contains two integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le n$)&nbsp;— the segment of the corresponding query.</p></div><div class="output-specification"><p>Print $q$ lines, where $i$-th of them contains a single integer&nbsp;— the answer to the $i$-th query modulo $10^9 + 7$.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($1 \le n, q \le 100\,000$).</p><p>The second line contains a string of $n$ characters, each character is either '<span class="tex-font-style-tt">0</span>' or '<span class="tex-font-style-tt">1</span>'. The $i$-th character defines the deliciousness of the $i$-th part.</p><p>Each of the following $q$ lines contains two integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le n$)&nbsp;— the segment of the corresponding query.</p>

## Output

<p>Print $q$ lines, where $i$-th of them contains a single integer&nbsp;— the answer to the $i$-th query modulo $10^9 + 7$.</p>





```input1
4 2
1011
1 4
3 4

```




```input2
3 2
111
1 2
3 3

```




```output1
14
3

```




```output2
3
1

```



## Note

<p>In the first example: </p><ul> <li> For query $1$: One of the best ways for JATC to eats those parts is in this order: $1$, $4$, $3$, $2$. </li><li> For query $2$: Both $3$, $4$ and $4$, $3$ ordering give the same answer. </li></ul><p>In the second example, any order of eating parts leads to the same answer.</p>
