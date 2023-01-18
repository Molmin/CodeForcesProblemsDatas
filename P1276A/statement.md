## Description

<div><p>You are given a non-empty string $s=s_1s_2\dots s_n$, which consists only of lowercase Latin letters. Polycarp does not like a string if it contains at least one string "<span class="tex-font-style-tt">one</span>" or at least one string "<span class="tex-font-style-tt">two</span>" (or both at the same time) as a <span class="tex-font-style-bf">substring</span>. In other words, Polycarp does not like the string $s$ if there is an integer $j$ ($1 \le j \le n-2$), that $s_{j}s_{j+1}s_{j+2}=$"<span class="tex-font-style-tt">one</span>" or $s_{j}s_{j+1}s_{j+2}=$"<span class="tex-font-style-tt">two</span>".</p><p>For example:</p><ul> <li> Polycarp does not like strings "<span class="tex-font-style-tt">oneee</span>", "<span class="tex-font-style-tt">ontwow</span>", "<span class="tex-font-style-tt">twone</span>" and "<span class="tex-font-style-tt">oneonetwo</span>" (they all have at least one substring "<span class="tex-font-style-tt">one</span>" or "<span class="tex-font-style-tt">two</span>"), </li><li> Polycarp likes strings "<span class="tex-font-style-tt">oonnee</span>", "<span class="tex-font-style-tt">twwwo</span>" and "<span class="tex-font-style-tt">twnoe</span>" (they have no substrings "<span class="tex-font-style-tt">one</span>" and "<span class="tex-font-style-tt">two</span>"). </li></ul><p>Polycarp wants to select a certain set of indices (positions) and remove all letters on these positions. All removals are made at the same time.</p><p>For example, if the string looks like $s=$"<span class="tex-font-style-tt">onetwone</span>", then if Polycarp selects two indices $3$ and $6$, then "<span class="tex-font-style-tt">on<span class="tex-font-style-underline"><span class="tex-font-style-bf">e</span></span>tw<span class="tex-font-style-underline"><span class="tex-font-style-bf">o</span></span>ne</span>" will be selected and the result is "<span class="tex-font-style-tt">ontwne</span>".</p><p>What is the minimum number of indices (positions) that Polycarp needs to select to make the string liked? What should these positions be?</p></div><div class="input-specification"><p>The first line of the input contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the input. Next, the test cases are given.</p><p>Each test case consists of one non-empty string $s$. Its length does not exceed $1.5\cdot10^5$. The string $s$ consists only of lowercase Latin letters.</p><p>It is guaranteed that the sum of lengths of all lines for all input data in the test does not exceed $1.5\cdot10^6$.</p></div><div class="output-specification"><p>Print an answer for each test case in the input in order of their appearance.</p><p>The first line of each answer should contain $r$ ($0 \le r \le |s|$) — the required minimum number of positions to be removed, where $|s|$ is the length of the given line. The second line of each answer should contain $r$ different integers — the indices themselves for removal in any order. Indices are numbered from left to right from $1$ to the length of the string. If $r=0$, then the second line can be skipped (or you can print empty). If there are several answers, print any of them.</p></div>

## Input

<p>The first line of the input contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the input. Next, the test cases are given.</p><p>Each test case consists of one non-empty string $s$. Its length does not exceed $1.5\cdot10^5$. The string $s$ consists only of lowercase Latin letters.</p><p>It is guaranteed that the sum of lengths of all lines for all input data in the test does not exceed $1.5\cdot10^6$.</p>

## Output

<p>Print an answer for each test case in the input in order of their appearance.</p><p>The first line of each answer should contain $r$ ($0 \le r \le |s|$) — the required minimum number of positions to be removed, where $|s|$ is the length of the given line. The second line of each answer should contain $r$ different integers — the indices themselves for removal in any order. Indices are numbered from left to right from $1$ to the length of the string. If $r=0$, then the second line can be skipped (or you can print empty). If there are several answers, print any of them.</p>





```input1
4
onetwone
testme
oneoneone
twotwo
```




```input2
10
onetwonetwooneooonetwooo
two
one
twooooo
ttttwo
ttwwoo
ooone
onnne
oneeeee
oneeeeeeetwooooo
```




```output1
2
6 3
0

3
4 1 7 
2
1 4
```




```output2
6
18 11 12 1 6 21 
1
1 
1
3 
1
2 
1
6 
0

1
4 
0

1
1 
2
1 11
```



## Note

<p>In the first example, answers are:</p><ul> <li> "<span class="tex-font-style-tt">on<span class="tex-font-style-underline"><span class="tex-font-style-bf">e</span></span>tw<span class="tex-font-style-underline"><span class="tex-font-style-bf">o</span></span>ne</span>", </li><li> "<span class="tex-font-style-tt">testme</span>" — Polycarp likes it, there is nothing to remove, </li><li> "<span class="tex-font-style-tt"><span class="tex-font-style-underline"><span class="tex-font-style-bf">o</span></span>ne<span class="tex-font-style-underline"><span class="tex-font-style-bf">o</span></span>ne<span class="tex-font-style-underline"><span class="tex-font-style-bf">o</span></span>ne</span>", </li><li> "<span class="tex-font-style-tt"><span class="tex-font-style-underline"><span class="tex-font-style-bf">t</span></span>wo<span class="tex-font-style-underline"><span class="tex-font-style-bf">t</span></span>wo</span>". </li></ul><p>In the second example, answers are: </p><ul> <li> "<span class="tex-font-style-tt"><span class="tex-font-style-underline"><span class="tex-font-style-bf">o</span></span>netw<span class="tex-font-style-underline"><span class="tex-font-style-bf">o</span></span>netw<span class="tex-font-style-underline"><span class="tex-font-style-bf">o</span></span><span class="tex-font-style-underline"><span class="tex-font-style-bf">o</span></span>neooo<span class="tex-font-style-underline"><span class="tex-font-style-bf">n</span></span>e<span class="tex-font-style-underline"><span class="tex-font-style-bf">t</span></span>wooo</span>", </li><li> "<span class="tex-font-style-tt"><span class="tex-font-style-underline"><span class="tex-font-style-bf">t</span></span>wo</span>", </li><li> "<span class="tex-font-style-tt"><span class="tex-font-style-underline"><span class="tex-font-style-bf">o</span></span>ne</span>", </li><li> "<span class="tex-font-style-tt"><span class="tex-font-style-underline"><span class="tex-font-style-bf">t</span></span>wooooo</span>", </li><li> "<span class="tex-font-style-tt">tttt<span class="tex-font-style-underline"><span class="tex-font-style-bf">w</span></span>o</span>", </li><li> "<span class="tex-font-style-tt">ttwwoo</span>" — Polycarp likes it, there is nothing to remove, </li><li> "<span class="tex-font-style-tt">ooo<span class="tex-font-style-underline"><span class="tex-font-style-bf">n</span></span>e</span>", </li><li> "<span class="tex-font-style-tt">onnne</span>" — Polycarp likes it, there is nothing to remove, </li><li> "<span class="tex-font-style-tt"><span class="tex-font-style-underline"><span class="tex-font-style-bf">o</span></span>neeeee</span>", </li><li> "<span class="tex-font-style-tt"><span class="tex-font-style-underline"><span class="tex-font-style-bf">o</span></span>neeeeeee<span class="tex-font-style-underline"><span class="tex-font-style-bf">t</span></span>wooooo</span>". </li></ul>
