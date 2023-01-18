## Description

<div><p>Roman and Denis are on the trip to the programming competition. Since the trip was long, they soon got bored, and hence decided to came up with something. Roman invented a pizza's recipe, while Denis invented a string multiplication. According to Denis, the result of multiplication (product) of strings $s$ of length $m$ and $t$ is a string $t + s_1 + t + s_2 + \ldots + t + s_m + t$, where $s_i$ denotes the $i$-th symbol of the string $s$, and "<span class="tex-font-style-tt">+</span>" denotes string concatenation. For example, the product of strings "<span class="tex-font-style-tt">abc</span>" and "<span class="tex-font-style-tt">de</span>" is a string "<span class="tex-font-style-tt">deadebdecde</span>", while the product of the strings "<span class="tex-font-style-tt">ab</span>" and "<span class="tex-font-style-tt">z</span>" is a string "<span class="tex-font-style-tt">zazbz</span>". Note, that unlike the numbers multiplication, the product of strings $s$ and $t$ is not necessarily equal to product of $t$ and $s$.</p><p>Roman was jealous of Denis, since he invented such a cool operation, and hence decided to invent something string-related too. Since Roman is beauty-lover, he decided to define the <span class="tex-font-style-it">beauty</span> of the string as the length of the longest substring, consisting of only one letter. For example, the beauty of the string "<span class="tex-font-style-tt">xayyaaabca</span>" is equal to $3$, since there is a substring "<span class="tex-font-style-tt">aaa</span>", while the beauty of the string "<span class="tex-font-style-tt">qwerqwer</span>" is equal to $1$, since all neighboring symbols in it are different.</p><p>In order to entertain Roman, Denis wrote down $n$ strings $p_1, p_2, p_3, \ldots, p_n$ on the paper and asked him to calculate the beauty of the string $( \ldots (((p_1 \cdot p_2) \cdot p_3) \cdot \ldots ) \cdot p_n$, where $s \cdot t$ denotes a multiplication of strings $s$ and $t$. Roman hasn't fully realized how Denis's multiplication works, so he asked you for a help. Denis knows, that Roman is very impressionable, he guarantees, that the beauty of the resulting string is at most $10^9$.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \leq n \leq 100\,000$)&nbsp;— the number of strings, wroted by Denis.</p><p>Next $n$ lines contain non-empty strings $p_1, p_2, \ldots, p_n$, consisting of lowercase english letters.</p><p>It's guaranteed, that the total length of the strings $p_i$ is at most $100\,000$, and that's the beauty of the resulting product is at most $10^9$.</p></div><div class="output-specification"><p>Print exactly one integer&nbsp;— the beauty of the product of the strings.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \leq n \leq 100\,000$)&nbsp;— the number of strings, wroted by Denis.</p><p>Next $n$ lines contain non-empty strings $p_1, p_2, \ldots, p_n$, consisting of lowercase english letters.</p><p>It's guaranteed, that the total length of the strings $p_i$ is at most $100\,000$, and that's the beauty of the resulting product is at most $10^9$.</p>

## Output

<p>Print exactly one integer&nbsp;— the beauty of the product of the strings.</p>





```input1
3
a
b
a
```




```input2
2
bnn
a
```




```output1
3
```




```output2
1
```



## Note

<p>In the first example, the product of strings is equal to "<span class="tex-font-style-tt">abaaaba</span>".</p><p>In the second example, the product of strings is equal to "<span class="tex-font-style-tt">abanana</span>".</p>
