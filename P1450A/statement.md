## Description

<div><p>A string $b$ is a subsequence of a string $a$ if $b$ can be obtained from $a$ by deletion of several (possibly, zero or all) characters. For example, "<span class="tex-font-style-tt">xy</span>" is a subsequence of "<span class="tex-font-style-tt">xzyw</span>" and "<span class="tex-font-style-tt">xy</span>", but not "<span class="tex-font-style-tt">yx</span>".</p><p>You are given a string $a$. Your task is to reorder the characters of $a$ so that "<span class="tex-font-style-tt">trygub</span>" is not a subsequence of the resulting string.</p><p>In other words, you should find a string $b$ which is a permutation of symbols of the string $a$ and "<span class="tex-font-style-tt">trygub</span>" is not a subsequence of $b$.</p><p>We have a truly marvelous proof that any string can be arranged not to contain "<span class="tex-font-style-tt">trygub</span>" as a subsequence, but this problem statement is too short to contain it.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1\le t\le 100$) — the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1\le n\le 200$) — the length of $a$.</p><p>The next line contains the string $a$ of length $n$, consisting of lowercase English letters.</p></div><div class="output-specification"><p>For each test case, output a string $b$ of length $n$ which is a permutation of characters of the string $a$, and such that "<span class="tex-font-style-tt">trygub</span>" is not a subsequence of it.</p><p>If there exist multiple possible strings $b$, you can print any.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1\le t\le 100$) — the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1\le n\le 200$) — the length of $a$.</p><p>The next line contains the string $a$ of length $n$, consisting of lowercase English letters.</p>

## Output

<p>For each test case, output a string $b$ of length $n$ which is a permutation of characters of the string $a$, and such that "<span class="tex-font-style-tt">trygub</span>" is not a subsequence of it.</p><p>If there exist multiple possible strings $b$, you can print any.</p>





```input1
3
11
antontrygub
15
bestcoordinator
19
trywatchinggurabruh
```




```output1
bugyrtnotna
bestcoordinator
bruhtrywatchinggura
```



## Note

<p>In the first test case, "<span class="tex-font-style-tt">bugyrtnotna</span>" does not contain "<span class="tex-font-style-tt">trygub</span>" as a subsequence. It does contain the letters of "<span class="tex-font-style-tt">trygub</span>", but not in the correct order, so it is not a subsequence.</p><p>In the second test case, we did not change the order of characters because it is not needed.</p><p>In the third test case, "<span class="tex-font-style-tt">bruhtrywatchinggura</span>" does contain "<span class="tex-font-style-tt">trygu</span>" as a subsequence, but not "<span class="tex-font-style-tt">trygub</span>".</p>
