## Description

<div><p>Vitya has learned that the answer for The Ultimate Question of Life, the Universe, and Everything is not the integer <span class="tex-font-style-striked">54</span> 42, but an increasing integer sequence $a_1, \ldots, a_n$. In order to not reveal the secret earlier than needed, Vitya encrypted the answer and obtained the sequence $b_1, \ldots, b_n$ using the following rules:</p><ul> <li> $b_1 = a_1$;</li><li> $b_i = a_i \oplus a_{i - 1}$ for all $i$ from 2 to $n$, where $x \oplus y$ is the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR</a> of $x$ and $y$. </li></ul><p>It is easy to see that the original sequence can be obtained using the rule $a_i = b_1 \oplus \ldots \oplus b_i$.</p><p>However, some time later Vitya discovered that the integers $b_i$ in the cypher got shuffled, and it can happen that when decrypted using the rule mentioned above, it can produce a sequence that is not increasing. In order to save his reputation in the scientific community, Vasya decided to find some permutation of integers $b_i$ so that the sequence $a_i = b_1 \oplus \ldots \oplus b_i$ is strictly increasing. Help him find such a permutation or determine that it is impossible.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \leq n \leq 10^5$).</p><p>The second line contains $n$ integers $b_1, \ldots, b_n$ ($1 \leq b_i &lt; 2^{60}$).</p></div><div class="output-specification"><p>If there are no valid permutations, print a single line containing "<span class="tex-font-style-tt">No</span>".</p><p>Otherwise in the first line print the word "<span class="tex-font-style-tt">Yes</span>", and in the second line print integers $b'_1, \ldots, b'_n$&nbsp;— a valid permutation of integers $b_i$. The unordered multisets $\{b_1, \ldots, b_n\}$ and $\{b'_1, \ldots, b'_n\}$ should be equal, i.&nbsp;e. for each integer $x$ the number of occurrences of $x$ in the first multiset should be equal to the number of occurrences of $x$ in the second multiset. Apart from this, the sequence $a_i = b'_1 \oplus \ldots \oplus b'_i$ should be strictly increasing.</p><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \leq n \leq 10^5$).</p><p>The second line contains $n$ integers $b_1, \ldots, b_n$ ($1 \leq b_i &lt; 2^{60}$).</p>

## Output

<p>If there are no valid permutations, print a single line containing "<span class="tex-font-style-tt">No</span>".</p><p>Otherwise in the first line print the word "<span class="tex-font-style-tt">Yes</span>", and in the second line print integers $b'_1, \ldots, b'_n$&nbsp;— a valid permutation of integers $b_i$. The unordered multisets $\{b_1, \ldots, b_n\}$ and $\{b'_1, \ldots, b'_n\}$ should be equal, i.&nbsp;e. for each integer $x$ the number of occurrences of $x$ in the first multiset should be equal to the number of occurrences of $x$ in the second multiset. Apart from this, the sequence $a_i = b'_1 \oplus \ldots \oplus b'_i$ should be strictly increasing.</p><p>If there are multiple answers, print any of them.</p>





```input1
3
1 2 3

```




```input2
6
4 7 7 12 31 61

```




```output1
No

```




```output2
Yes
4 12 7 31 7 61 

```



## Note

<p>In the first example no permutation is valid.</p><p>In the second example the given answer lead to the sequence $a_1 = 4$, $a_2 = 8$, $a_3 = 15$, $a_4 = 16$, $a_5 = 23$, $a_6 = 42$.</p>
