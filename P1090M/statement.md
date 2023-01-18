## Description

<div><p>There are $n$ houses along the road where Anya lives, each one is painted in one of $k$ possible colors.</p><p>Anya likes walking along this road, but she doesn't like when two adjacent houses at the road have the same color. She wants to select a long segment of the road such that no two adjacent houses have the same color.</p><p>Help Anya find the longest segment with this property.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$&nbsp;— the number of houses and the number of colors ($1 \le n \le 100\,000$, $1 \le k \le 100\,000$).</p><p>The next line contains $n$ integers $a_1, a_2, \ldots, a_n$&nbsp;— the colors of the houses along the road ($1 \le a_i \le k$).</p></div><div class="output-specification"><p>Output a single integer&nbsp;— the maximum number of houses on the road segment having no two adjacent houses of the same color.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$&nbsp;— the number of houses and the number of colors ($1 \le n \le 100\,000$, $1 \le k \le 100\,000$).</p><p>The next line contains $n$ integers $a_1, a_2, \ldots, a_n$&nbsp;— the colors of the houses along the road ($1 \le a_i \le k$).</p>

## Output

<p>Output a single integer&nbsp;— the maximum number of houses on the road segment having no two adjacent houses of the same color.</p>





```input1
8 3
1 2 3 3 2 1 2 2
```




```output1
4
```



## Note

<p>In the example, the longest segment without neighboring houses of the same color is from the house 4 to the house 7. The colors of the houses are $[3, 2, 1, 2]$ and its length is 4 houses.</p>
