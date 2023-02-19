## Description

<div><p>This year a Chunin Selection Exam is held again in Konoha, and taking part in it are $n$ ninjas named $s_1$, $s_2$, ..., $s_n$. All names are distinct. One of the exam stages consists of fights between the participants. This year the rules determining the ninjas for each fight are the following: ninjas $i$ and $j$ fight against each other if the following conditions are held:</p><ul> <li> $i \neq j$; </li><li> $s_{j}$ is a substring of $s_{i}$; </li><li> there is no $k$ except $i$ and $j$ that $s_{j}$ is a substring of $s_{k}$, and $s_{k}$ is a substring of $s_{i}$. </li></ul><p>A string $a$ is a substring of a string $b$ if $a$ can be obtained from $b$ by deletion of several (possibly, zero or all) characters from the beginning and several (possibly, zero or all) characters from the end.</p><p>Your task is to find out how many fights are going to take place this year.</p></div><div class="input-specification"><p>The first line consists of the only integer $n$ ($1 \leq n \leq 10^{6}$) standing for the number of examinees.</p><p>The following $n$ lines contain their names. No two names coincide, all names are non-empty and consist of lowercase English letters. The total length of all names doesn't exceed $10^6$.</p></div><div class="output-specification"><p>Print the only integer standing for the number of fights.</p></div>

## Input

<p>The first line consists of the only integer $n$ ($1 \leq n \leq 10^{6}$) standing for the number of examinees.</p><p>The following $n$ lines contain their names. No two names coincide, all names are non-empty and consist of lowercase English letters. The total length of all names doesn't exceed $10^6$.</p>

## Output

<p>Print the only integer standing for the number of fights.</p>





```input1
5
hidan
dan
hanabi
bi
nabi
```




```input2
4
abacaba
abaca
acaba
aca
```




```output1
3
```




```output2
4
```



## Note

<p>In the first example <span class="tex-font-style-tt">hidan</span> fights against <span class="tex-font-style-tt">dan</span>, and <span class="tex-font-style-tt">hanabi</span> fights against <span class="tex-font-style-tt">nabi</span>, who also fights <span class="tex-font-style-tt">bi</span>. Ninjas named <span class="tex-font-style-tt">hanabi</span> and <span class="tex-font-style-tt">bi</span> don't fight each other since there is the ninja called <span class="tex-font-style-tt">nabi</span> who breaks the third condition for them.</p><p>In the second example the fights are held between <span class="tex-font-style-tt">abacaba</span> and <span class="tex-font-style-tt">acaba</span>, <span class="tex-font-style-tt">abacaba</span> and <span class="tex-font-style-tt">abaca</span>, <span class="tex-font-style-tt">acaba</span> and <span class="tex-font-style-tt">aca</span>, <span class="tex-font-style-tt">abaca</span> and <span class="tex-font-style-tt">aca</span>.</p>
