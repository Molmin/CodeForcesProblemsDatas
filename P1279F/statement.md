## Description

<div><p>New Year is getting near. So it's time to change handles on codeforces. Mishka wants to change his handle but in such a way that people would not forget who he is.</p><p>To make it work, he only allowed to change letters case. More formally, during <span class="tex-font-style-bf">one</span> handle change he can choose any segment of his handle $[i; i + l - 1]$ and apply <span class="tex-font-style-tt">tolower</span> or <span class="tex-font-style-tt">toupper</span> to all letters of his handle on this segment (more fomally, replace all uppercase letters with corresponding lowercase or vice versa). The length $l$ is fixed for all changes.</p><p>Because it is not allowed to change codeforces handle too often, Mishka can perform at most $k$ such operations. What is the <span class="tex-font-style-bf">minimum</span> value of $min(lower, upper)$ (where $lower$ is the number of lowercase letters, and $upper$ is the number of uppercase letters) can be obtained after optimal sequence of changes?</p></div><div class="input-specification"><p>The first line of the input contains three integers $n, k$ and $l$ ($1 \le n, k, l \le 10^6, l \le n)$ — the length of Mishka's handle, the number of changes and the length of the segment.</p><p>The second line of the input contains one string $s$, consisting of $n$ lowercase and uppercase Latin letters — Mishka's handle.</p></div><div class="output-specification"><p>Print one integer — the minimum value of $min(lower, upper)$ after that Mishka change his handle at most $k$ times in a way described in the problem statement.</p></div>

## Input

<p>The first line of the input contains three integers $n, k$ and $l$ ($1 \le n, k, l \le 10^6, l \le n)$ — the length of Mishka's handle, the number of changes and the length of the segment.</p><p>The second line of the input contains one string $s$, consisting of $n$ lowercase and uppercase Latin letters — Mishka's handle.</p>

## Output

<p>Print one integer — the minimum value of $min(lower, upper)$ after that Mishka change his handle at most $k$ times in a way described in the problem statement.</p>





```input1
7 1 4
PikMike
```




```input2
15 2 2
AaAaAAaaAAAAaaA
```




```input3
14 2 6
aBcdEFGHIJklMn
```




```input4
9 2 2
aAaAAAaaA
```




```output1
0
```




```output2
2
```




```output3
0
```




```output4
1
```


