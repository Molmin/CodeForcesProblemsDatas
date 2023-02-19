## Description

<div><p>There is a deck of $n$ cards. The $i$-th card has a number $a_i$ on the front and a number $b_i$ on the back. Every integer between $1$ and $2n$ appears exactly once on the cards.</p><p>A deck is called sorted if the front values are in <span class="tex-font-style-bf">increasing</span> order and the back values are in <span class="tex-font-style-bf">decreasing</span> order. That is, if $a_i&lt; a_{i+1}$ and $b_i&gt; b_{i+1}$ for all $1\le i&lt;n$.</p><p>To flip a card $i$ means swapping the values of $a_i$ and $b_i$. You must flip some subset of cards (possibly, none), then put all the cards in any order you like. What is the minimum number of cards you must flip in order to sort the deck?</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1\le n\le 2\cdot 10^5$) — the number of cards.</p><p>The next $n$ lines describe the cards. The $i$-th of these lines contains two integers $a_i, b_i$ ($1\le a_i, b_i\le 2n$). Every integer between $1$ and $2n$ appears exactly once.</p></div><div class="output-specification"><p>If it is impossible to sort the deck, output "<span class="tex-font-style-tt">-1</span>". Otherwise, output the minimum number of flips required to sort the deck.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1\le n\le 2\cdot 10^5$) — the number of cards.</p><p>The next $n$ lines describe the cards. The $i$-th of these lines contains two integers $a_i, b_i$ ($1\le a_i, b_i\le 2n$). Every integer between $1$ and $2n$ appears exactly once.</p>

## Output

<p>If it is impossible to sort the deck, output "<span class="tex-font-style-tt">-1</span>". Otherwise, output the minimum number of flips required to sort the deck.</p>





```input1
5
3 10
6 4
1 9
5 8
2 7
```




```input2
2
1 2
3 4
```




```input3
3
1 2
3 6
4 5
```




```output1
2
```




```output2
-1
```




```output3
-1
```



## Note

<p>In the first test case, we flip the cards $(1, 9)$ and $(2, 7)$. The deck is then ordered $(3,10), (5,8), (6,4), (7,2), (9,1)$. It is sorted because $3&lt;5&lt;6&lt;7&lt;9$ and $10&gt;8&gt;4&gt;2&gt;1$.</p><p>In the second test case, it is impossible to sort the deck.</p>
