## Description

<div><p>Mike decided to teach programming to children in an elementary school. He knows that it is not an easy task to interest children in that age to code. That is why he decided to give each child <span class="tex-font-style-bf">two</span> sweets.</p><p>Mike has $n$ sweets with sizes $a_1, a_2, \ldots, a_n$. All his sweets have <span class="tex-font-style-bf">different</span> sizes. That is, there is no such pair $(i, j)$ ($1 \leq i, j \leq n$) such that $i \ne j$ and $a_i = a_j$.</p><p>Since Mike has taught for many years, he knows that if he gives two sweets with sizes $a_i$ and $a_j$ to one child and $a_k$ and $a_p$ to another, where $(a_i + a_j) \neq (a_k + a_p)$, then a child who has a smaller sum of sizes will be upset. That is, if there are two children who have different sums of sweets, then one of them will be upset. Apparently, Mike does not want somebody to be upset. </p><p>Mike wants to invite children giving each of them <span class="tex-font-style-bf">two</span> sweets. Obviously, he can't give one sweet to two or more children. His goal is to invite as many children as he can. </p><p>Since Mike is busy preparing to his first lecture in the elementary school, he is asking you to find the maximum number of children he can invite giving each of them two sweets in such way that nobody will be upset.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($2 \leq n \leq 1\,000$)&nbsp;— the number of sweets Mike has.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^5$)&nbsp;— the sizes of the sweets. It is guaranteed that all integers are distinct.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the maximum number of children Mike can invite giving each of them two sweets in such way that nobody will be upset.</p></div>

## Input

<p>The first line contains one integer $n$ ($2 \leq n \leq 1\,000$)&nbsp;— the number of sweets Mike has.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^5$)&nbsp;— the sizes of the sweets. It is guaranteed that all integers are distinct.</p>

## Output

<p>Print one integer&nbsp;— the maximum number of children Mike can invite giving each of them two sweets in such way that nobody will be upset.</p>





```input1
8
1 8 3 11 4 9 2 7
```




```input2
7
3 1 7 11 9 2 12
```




```output1
3
```




```output2
2
```



## Note

<p>In the first example, Mike can give $9+2=11$ to one child, $8+3=11$ to another one, and $7+4=11$ to the third child. Therefore, Mike can invite three children. Note that it is <span class="tex-font-style-bf">not</span> the only solution.</p><p>In the second example, Mike can give $3+9=12$ to one child and $1+11$ to another one. Therefore, Mike can invite two children. Note that it is <span class="tex-font-style-bf">not</span> the only solution.</p>
