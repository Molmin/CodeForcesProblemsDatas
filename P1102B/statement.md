## Description

<div><p>You are given an array $a$ consisting of $n$ integer numbers.</p><p>You have to color this array in $k$ colors in such a way that: </p><ul> <li> Each element of the array should be colored in some color; </li><li> For each $i$ from $1$ to $k$ there should be <span class="tex-font-style-bf">at least one</span> element colored in the $i$-th color in the array; </li><li> For each $i$ from $1$ to $k$ all elements colored in the $i$-th color should be <span class="tex-font-style-bf">distinct</span>. </li></ul><p>Obviously, such coloring might be impossible. In this case, print "<span class="tex-font-style-tt">NO</span>". Otherwise print "<span class="tex-font-style-tt">YES</span>" and <span class="tex-font-style-bf">any</span> coloring (i.e. numbers $c_1, c_2, \dots c_n$, where $1 \le c_i \le k$ and $c_i$ is the color of the $i$-th element of the given array) satisfying the conditions above. If there are multiple answers, you can print <span class="tex-font-style-bf">any</span>.</p></div><div class="input-specification"><p>The first line of the input contains two integers $n$ and $k$ ($1 \le k \le n \le 5000$) — the length of the array $a$ and the number of colors, respectively.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 5000$) — elements of the array $a$.</p></div><div class="output-specification"><p>If there is no answer, print "<span class="tex-font-style-tt">NO</span>". Otherwise print "<span class="tex-font-style-tt">YES</span>" and <span class="tex-font-style-bf">any</span> coloring (i.e. numbers $c_1, c_2, \dots c_n$, where $1 \le c_i \le k$ and $c_i$ is the color of the $i$-th element of the given array) satisfying the conditions described in the problem statement. If there are multiple answers, you can print <span class="tex-font-style-bf">any</span>.</p></div>

## Input

<p>The first line of the input contains two integers $n$ and $k$ ($1 \le k \le n \le 5000$) — the length of the array $a$ and the number of colors, respectively.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 5000$) — elements of the array $a$.</p>

## Output

<p>If there is no answer, print "<span class="tex-font-style-tt">NO</span>". Otherwise print "<span class="tex-font-style-tt">YES</span>" and <span class="tex-font-style-bf">any</span> coloring (i.e. numbers $c_1, c_2, \dots c_n$, where $1 \le c_i \le k$ and $c_i$ is the color of the $i$-th element of the given array) satisfying the conditions described in the problem statement. If there are multiple answers, you can print <span class="tex-font-style-bf">any</span>.</p>





```input1
4 2
1 2 2 3
```




```input2
5 2
3 2 1 2 3
```




```input3
5 2
2 1 1 2 1
```




```output1
YES
1 1 2 2
```




```output2
YES
2 1 1 2 1
```




```output3
NO
```



## Note

<p>In the first example the answer $2~ 1~ 2~ 1$ is also acceptable.</p><p>In the second example the answer $1~ 1~ 1~ 2~ 2$ is also acceptable.</p><p>There exist other acceptable answers for both examples.</p>
