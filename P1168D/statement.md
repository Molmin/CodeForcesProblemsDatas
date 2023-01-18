## Description

<div><p>Toad Ilya has a rooted binary tree with vertex $1$ being the root. A tree is a connected graph without cycles. A tree is rooted if one vertex is selected and called the root. A vertex $u$ is a child of a vertex $v$ if $u$ and $v$ are connected by an edge and $v$ is closer to the root than $u$. A leaf is a non-root vertex that has no children.</p><p>In the tree Ilya has each vertex has <span class="tex-font-style-bf">at most two</span> children, and each edge has some character written on it. The character can be a lowercase English letter or the question mark '<span class="tex-font-style-tt">?</span>'.</p><p>Ilya will $q$ times update the tree a bit. Each update will replace exactly one character on some edge. After each update Ilya needs to find if the tree is <span class="tex-font-style-it">anagrammable</span> and if yes, find its <span class="tex-font-style-it">anagramnity</span> for each letter. Well, that's difficult to explain, but we'll try.</p><p>To start with, a string $a$ is an <span class="tex-font-style-it">anagram</span> of a string $b$ if it is possible to rearrange letters in $a$ (without changing the letters itself) so that it becomes $b$. For example, the string "<span class="tex-font-style-tt">fortyfive</span>" is an anagram of the string "<span class="tex-font-style-tt">overfifty</span>", but the string "<span class="tex-font-style-tt">aabb</span>" is not an anagram of the string "<span class="tex-font-style-tt">bbba</span>".</p><p>Consider a path from the root of the tree to a leaf. The characters on the edges on this path form a string, we say that this string is associated with this leaf. The tree is <span class="tex-font-style-it">anagrammable</span> if and only if it is possible to replace each question mark with a lowercase English letter so that for all pair of leaves the associated strings for these leaves are anagrams of each other.</p><p>If the tree is <span class="tex-font-style-it">anagrammable</span>, then its <span class="tex-font-style-it">anagramnity</span> for the letter $c$ is the maximum possible number of letters $c$ in a string associated with some leaf in a valid replacement of all question marks.</p><p>Please after each update find if the tree is <span class="tex-font-style-it">anagrammable</span> and if yes, find the $\sum{f(c) \cdot ind(c)}$ for all letters $c$, where $f(c)$ is the <span class="tex-font-style-it">anagramnity</span> for the letter $c$, and $ind(x)$ is the index of this letter in the alphabet ($ind($"<span class="tex-font-style-tt">a</span>"$) = 1$, $ind($"<span class="tex-font-style-tt">b</span>"$) = 2$, ..., $ind($"<span class="tex-font-style-tt">z</span>"$) = 26$).</p></div><div class="input-specification"><p>The first line of input contains two integers $n$ and $q$ ($2 \leq n \leq 150\,000$, $1 \leq q \leq 150\,000$)&nbsp;— the number of vertices in the tree and the number of queries.</p><p>The next $n-1$ lines describe the initial tree. The $i$-th of them contains an integer $p_i$ and a character $c_i$ ($1 \leq p_i \leq i$, $c_i$ is a lowercase English letter or the question mark '<span class="tex-font-style-tt">?</span>') describing an edge between vertices $p_i$ and $i+1$ with character $c_i$ written on it.</p><p>The root of this tree is the vertex $1$, and each vertex has at most two children.</p><p>The next $q$ lines describe the queries. The $i$-th of them contains two integers $v$ and $c$ ($2 \leq v \leq n$, $c$ is a lowercase English letter or the question mark '<span class="tex-font-style-tt">?</span>'), meaning that updated character on the edge between $p_{v-1}$ to $v$ is $c$. The updated character can be the same as was written before.</p></div><div class="output-specification"><p>Output $q$ lines. In the $i$-th of them print "<span class="tex-font-style-tt">Fou</span>" if the tree is <span class="tex-font-style-bf">not</span> <span class="tex-font-style-it">anagrammable</span> after the first $i$ updates.</p><p>Otherwise output "<span class="tex-font-style-tt">Shi</span>" and the $\sum{f(c) \cdot ind(c)}$ for all letters $c$.</p></div>

## Input

<p>The first line of input contains two integers $n$ and $q$ ($2 \leq n \leq 150\,000$, $1 \leq q \leq 150\,000$)&nbsp;— the number of vertices in the tree and the number of queries.</p><p>The next $n-1$ lines describe the initial tree. The $i$-th of them contains an integer $p_i$ and a character $c_i$ ($1 \leq p_i \leq i$, $c_i$ is a lowercase English letter or the question mark '<span class="tex-font-style-tt">?</span>') describing an edge between vertices $p_i$ and $i+1$ with character $c_i$ written on it.</p><p>The root of this tree is the vertex $1$, and each vertex has at most two children.</p><p>The next $q$ lines describe the queries. The $i$-th of them contains two integers $v$ and $c$ ($2 \leq v \leq n$, $c$ is a lowercase English letter or the question mark '<span class="tex-font-style-tt">?</span>'), meaning that updated character on the edge between $p_{v-1}$ to $v$ is $c$. The updated character can be the same as was written before.</p>

## Output

<p>Output $q$ lines. In the $i$-th of them print "<span class="tex-font-style-tt">Fou</span>" if the tree is <span class="tex-font-style-bf">not</span> <span class="tex-font-style-it">anagrammable</span> after the first $i$ updates.</p><p>Otherwise output "<span class="tex-font-style-tt">Shi</span>" and the $\sum{f(c) \cdot ind(c)}$ for all letters $c$.</p>





```input1
3 4
1 ?
1 ?
2 ?
2 a
3 b
2 b
```




```input2
5 2
1 ?
1 ?
2 ?
3 ?
4 a
5 b
```




```output1
Shi 351
Shi 1
Fou
Shi 2
```




```output2
Shi 352
Shi 3
```



## Note

<p>In the first example after the first query, for each character, you can set all edges equal to that character, and you will get $1$ such character on each path, so the answer is $1 \cdot (1+2+\ldots+26) = 351$.</p><p>In the first example after the second query, you know that all paths should be an anagram of "<span class="tex-font-style-tt">a</span>", so all paths should be "<span class="tex-font-style-tt">a</span>", so the answer is $1 \cdot 1 = 1$.</p><p>In the first example after the third query, you have two paths with strings "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">b</span>", but these strings are not anagrams, so the answer is "<span class="tex-font-style-tt">Fou</span>".</p><p>In the first example after the fourth query, you know that all paths should be "<span class="tex-font-style-tt">b</span>", so the answer is $1 \cdot 2 = 2$.</p><p>In the second example after the first query, you know that $f($'<span class="tex-font-style-tt">a</span>'$) = 2$ and $f(c) = 1$ for all other characters, so the answer is $1 \cdot (2 + 3 + \ldots + 26) + 2 = 352$.</p><p>In the second example after the second query, you know that each path should contain one '<span class="tex-font-style-tt">a</span>' and one '<span class="tex-font-style-tt">b</span>', so the answer is $1 \cdot 1 + 1 \cdot 2 = 3$.</p>
