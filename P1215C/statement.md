## Description

<div><p>Monocarp has got two strings $s$ and $t$ having equal length. Both strings consist of lowercase Latin letters "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">b</span>". </p><p>Monocarp wants to make these two strings $s$ and $t$ equal to each other. He can do the following operation any number of times: choose an index $pos_1$ in the string $s$, choose an index $pos_2$ in the string $t$, and swap $s_{pos_1}$ with $t_{pos_2}$.</p><p>You have to determine the minimum number of operations Monocarp has to perform to make $s$ and $t$ equal, and print any optimal sequence of operations — or say that it is impossible to make these strings equal.</p></div><div class="input-specification"><p>The first line contains one integer $n$ $(1 \le n \le 2 \cdot 10^{5})$ — the length of $s$ and $t$.</p><p>The second line contains one string $s$ consisting of $n$ characters "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">b</span>". </p><p>The third line contains one string $t$ consisting of $n$ characters "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">b</span>". </p></div><div class="output-specification"><p>If it is impossible to make these strings equal, print $-1$.</p><p>Otherwise, in the first line print $k$ — the minimum number of operations required to make the strings equal. In each of the next $k$ lines print two integers — the index in the string $s$ and the index in the string $t$ that should be used in the corresponding swap operation. </p></div>

## Input

<p>The first line contains one integer $n$ $(1 \le n \le 2 \cdot 10^{5})$ — the length of $s$ and $t$.</p><p>The second line contains one string $s$ consisting of $n$ characters "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">b</span>". </p><p>The third line contains one string $t$ consisting of $n$ characters "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">b</span>". </p>

## Output

<p>If it is impossible to make these strings equal, print $-1$.</p><p>Otherwise, in the first line print $k$ — the minimum number of operations required to make the strings equal. In each of the next $k$ lines print two integers — the index in the string $s$ and the index in the string $t$ that should be used in the corresponding swap operation. </p>





```input1
4
abab
aabb
```




```input2
1
a
b
```




```input3
8
babbaabb
abababaa
```




```output1
2
3 3
3 2
```




```output2
-1
```




```output3
3
2 6
1 3
7 8
```



## Note

<p>In the first example two operations are enough. For example, you can swap the third letter in $s$ with the third letter in $t$. Then $s = $ "<span class="tex-font-style-tt">abbb</span>", $t = $ "<span class="tex-font-style-tt">aaab</span>". Then swap the third letter in $s$ and the second letter in $t$. Then both $s$ and $t$ are equal to "<span class="tex-font-style-tt">abab</span>".</p><p>In the second example it's impossible to make two strings equal.</p>
