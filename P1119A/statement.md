## Description

<div><p>Ilya lives in a beautiful city of Chordalsk.</p><p>There are $n$ houses on the street Ilya lives, they are numerated from $1$ to $n$ from left to right; the distance between every two neighboring houses is equal to $1$ unit. The neighboring houses are $1$ and $2$, $2$ and $3$, ..., $n-1$ and $n$. The houses $n$ and $1$ are not neighboring.</p><p>The houses are colored in colors $c_1, c_2, \ldots, c_n$ so that the $i$-th house is colored in the color $c_i$. Everyone knows that Chordalsk is not boring, so there are at least two houses colored in different colors.</p><p>Ilya wants to select two houses $i$ and $j$ so that $1 \leq i &lt; j \leq n$, and they have different colors: $c_i \neq c_j$. He will then walk from the house $i$ to the house $j$ the distance of $(j-i)$ units.</p><p>Ilya loves long walks, so he wants to choose the houses so that the distance between them is the maximum possible.</p><p>Help Ilya, find this maximum possible distance.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($3 \leq n \leq 300\,000$)&nbsp;— the number of cities on the street.</p><p>The second line contains $n$ integers $c_1, c_2, \ldots, c_n$ ($1 \leq c_i \leq n$)&nbsp;— the colors of the houses.</p><p>It is guaranteed that there is at least one pair of indices $i$ and $j$ so that $1 \leq i &lt; j \leq n$ and $c_i \neq c_j$.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the maximum possible distance Ilya can walk.</p></div>

## Input

<p>The first line contains a single integer $n$ ($3 \leq n \leq 300\,000$)&nbsp;— the number of cities on the street.</p><p>The second line contains $n$ integers $c_1, c_2, \ldots, c_n$ ($1 \leq c_i \leq n$)&nbsp;— the colors of the houses.</p><p>It is guaranteed that there is at least one pair of indices $i$ and $j$ so that $1 \leq i &lt; j \leq n$ and $c_i \neq c_j$.</p>

## Output

<p>Print a single integer&nbsp;— the maximum possible distance Ilya can walk.</p>





```input1
5
1 2 3 2 3
```




```input2
3
1 2 1
```




```input3
7
1 1 3 1 1 1 1
```




```output1
4
```




```output2
1
```




```output3
4
```



## Note

<p>In the first example the optimal way is to walk from the first house to the last one, where Ilya can walk the distance of $5-1 = 4$ units.</p><p>In the second example the optimal way is to either walk from the first house to the second or from the second to the third. Both these ways have the distance of $1$ unit.</p><p>In the third example the optimal way is to walk from the third house to the last one, where Ilya can walk the distance of $7-3 = 4$ units. </p>
