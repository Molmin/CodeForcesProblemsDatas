## Description

<div><p>A sequence of round and square brackets is given. You can change the sequence by performing the following operations:</p><ol> <li> change the direction of a bracket from opening to closing and vice versa without changing the form of the bracket: i.e. you can change '<span class="tex-font-style-tt">(</span>' to '<span class="tex-font-style-tt">)</span>' and '<span class="tex-font-style-tt">)</span>' to '<span class="tex-font-style-tt">(</span>'; you can change '<span class="tex-font-style-tt">[</span>' to '<span class="tex-font-style-tt">]</span>' and '<span class="tex-font-style-tt">]</span>' to '<span class="tex-font-style-tt">[</span>'. The operation costs $0$ burles.</li><li> change any <span class="tex-font-style-bf">square</span> bracket to <span class="tex-font-style-bf">round</span> bracket having the same direction: i.e. you can change '<span class="tex-font-style-tt">[</span>' to '<span class="tex-font-style-tt">(</span>' but <span class="tex-font-style-bf">not</span> from '<span class="tex-font-style-tt">(</span>' to '<span class="tex-font-style-tt">[</span>'; similarly, you can change '<span class="tex-font-style-tt">]</span>' to '<span class="tex-font-style-tt">)</span>' but <span class="tex-font-style-bf">not</span> from '<span class="tex-font-style-tt">)</span>' to '<span class="tex-font-style-tt">]</span>'. The operation costs $1$ burle. </li></ol><p>The operations can be performed in any order any number of times.</p><p>You are given a string $s$ of the length $n$ and $q$ queries of the type "<span class="tex-font-style-tt">l r</span>" where $1 \le l &lt; r \le n$. For every substring $s[l \dots r]$, find the minimum cost to pay to make it a correct bracket sequence. It is guaranteed that the substring $s[l \dots r]$ has an even length.</p><p>The queries must be processed independently, i.e. the changes made in the string for the answer to a question $i$ don't affect the queries $j$ ($j &gt; i$). In other words, for every query, the substring $s[l \dots r]$ is given from the initially given string $s$.</p><p>A correct bracket sequence is a sequence that can be built according the following rules:</p><ul> <li> an empty sequence is a correct bracket sequence; </li><li> if "<span class="tex-font-style-tt">s</span>" is a correct bracket sequence, the sequences "<span class="tex-font-style-tt">(s)</span>" and "<span class="tex-font-style-tt">[s]</span>" are correct bracket sequences. </li><li> if "<span class="tex-font-style-tt">s</span>" and "<span class="tex-font-style-tt">t</span>" are correct bracket sequences, the sequence "<span class="tex-font-style-tt">st</span>" (the concatenation of the sequences) is a correct bracket sequence. </li></ul><p>E.g. the sequences "<span class="tex-font-style-tt"></span>", "<span class="tex-font-style-tt">(()[])</span>", "<span class="tex-font-style-tt">[()()]()</span>" and "<span class="tex-font-style-tt">(())()</span>" are correct bracket sequences whereas "<span class="tex-font-style-tt">(</span>", "<span class="tex-font-style-tt">[(])</span>" and "<span class="tex-font-style-tt">)))</span>" are not.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 100$) — the number of test cases. Then $t$ test cases follow.</p><p>For each test case, the first line contains a non-empty string $s$ containing only round ('<span class="tex-font-style-tt">(</span>', '<span class="tex-font-style-tt">)</span>') and square ('<span class="tex-font-style-tt">[</span>', '<span class="tex-font-style-tt">]</span>') brackets. The length of the string doesn't exceed $10^6$. The string contains at least $2$ characters.</p><p>The second line contains one integer $q$ ($1 \le q \le 2 \cdot 10^5$) — the number of queries.</p><p>Then $q$ lines follow, each of them contains two integers $l$ and $r$ ($1 \le l &lt; r \le n$ where $n$ is the length of $s$). It is guaranteed that the substring $s[l \dots r]$ has even length.</p><p>It is guaranteed that the sum of the lengths of all strings given in all test cases doesn't exceed $10^6$. The sum of all $q$ given in all test cases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case output in a separate line for each query one integer $x$ ($x \ge 0$) — the minimum cost to pay to make the given substring a correct bracket sequence.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 100$) — the number of test cases. Then $t$ test cases follow.</p><p>For each test case, the first line contains a non-empty string $s$ containing only round ('<span class="tex-font-style-tt">(</span>', '<span class="tex-font-style-tt">)</span>') and square ('<span class="tex-font-style-tt">[</span>', '<span class="tex-font-style-tt">]</span>') brackets. The length of the string doesn't exceed $10^6$. The string contains at least $2$ characters.</p><p>The second line contains one integer $q$ ($1 \le q \le 2 \cdot 10^5$) — the number of queries.</p><p>Then $q$ lines follow, each of them contains two integers $l$ and $r$ ($1 \le l &lt; r \le n$ where $n$ is the length of $s$). It is guaranteed that the substring $s[l \dots r]$ has even length.</p><p>It is guaranteed that the sum of the lengths of all strings given in all test cases doesn't exceed $10^6$. The sum of all $q$ given in all test cases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case output in a separate line for each query one integer $x$ ($x \ge 0$) — the minimum cost to pay to make the given substring a correct bracket sequence.</p>





```input1
3
([))[)()][]]
3
1 12
4 9
3 6
))))))
2
2 3
1 4
[]
1
1 2
```




```output1
0
2
1
0
0
0
```



## Note

<p>Consider the first test case. The first query describes the whole given string, the string can be turned into the following correct bracket sequence: "<span class="tex-font-style-tt">([()])()[[]]</span>". The forms of the brackets aren't changed so the cost of changing is $0$.</p><p>The second query describes the substring "<span class="tex-font-style-tt">)[)()]</span>". It may be turned into "<span class="tex-font-style-tt">(()())</span>", the cost is equal to $2$.</p><p>The third query describes the substring "<span class="tex-font-style-tt">))[)</span>". It may be turned into "<span class="tex-font-style-tt">()()</span>", the cost is equal to $1$.</p><p>The substrings of the second test case contain only round brackets. It's possible to prove that any sequence of round brackets having an even length may be turned into a correct bracket sequence for the cost of $0$ burles.</p><p>In the third test case, the single query describes the string "<span class="tex-font-style-tt">[]</span>" that is already a correct bracket sequence.</p>
