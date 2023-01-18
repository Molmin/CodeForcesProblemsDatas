## Description

<div><p>You are given a string $s$ consisting of $n$ lowercase Latin letters. Polycarp wants to remove exactly $k$ characters ($k \le n$) from the string $s$. Polycarp uses the following algorithm $k$ times:</p><ul> <li> if there is at least one letter '<span class="tex-font-style-tt">a</span>', remove the leftmost occurrence and stop the algorithm, otherwise go to next item; </li><li> if there is at least one letter '<span class="tex-font-style-tt">b</span>', remove the leftmost occurrence and stop the algorithm, otherwise go to next item; </li><li> ... </li><li> remove the leftmost occurrence of the letter '<span class="tex-font-style-tt">z</span>' and stop the algorithm. </li></ul><p>This algorithm removes a single letter from the string. Polycarp performs this algorithm exactly $k$ times, thus removing exactly $k$ characters.</p><p>Help Polycarp find the resulting string.</p></div><div class="input-specification"><p>The first line of input contains two integers $n$ and $k$ ($1 \le k \le n \le 4 \cdot 10^5$) — the length of the string and the number of letters Polycarp will remove.</p><p>The second line contains the string $s$ consisting of $n$ lowercase Latin letters.</p></div><div class="output-specification"><p>Print the string that will be obtained from $s$ after Polycarp removes exactly $k$ letters using the above algorithm $k$ times.</p><p>If the resulting string is empty, print nothing. It is allowed to print nothing or an empty line (line break).</p></div>

## Input

<p>The first line of input contains two integers $n$ and $k$ ($1 \le k \le n \le 4 \cdot 10^5$) — the length of the string and the number of letters Polycarp will remove.</p><p>The second line contains the string $s$ consisting of $n$ lowercase Latin letters.</p>

## Output

<p>Print the string that will be obtained from $s$ after Polycarp removes exactly $k$ letters using the above algorithm $k$ times.</p><p>If the resulting string is empty, print nothing. It is allowed to print nothing or an empty line (line break).</p>





```input1
15 3
cccaabababaccbc

```




```input2
15 9
cccaabababaccbc

```




```input3
1 1
u

```




```output1
cccbbabaccbc

```




```output2
cccccc

```




```output3

```


