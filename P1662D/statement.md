## Description

<div><p>A wild basilisk just appeared at your doorstep. You are not entirely sure what a basilisk is and you wonder whether it evolved from your favorite animal, the weasel. </p><p>How can you find out whether basilisks evolved from weasels? Certainly, a good first step is to sequence both of their DNAs. Then you can try to check whether there is a sequence of possible mutations from the DNA of the weasel to the DNA of the basilisk. </p><p>Your friend Ron is a talented alchemist and has studied DNA sequences in many of his experiments. He has found out that DNA strings consist of the letters <span class="tex-font-style-tt">A</span>, <span class="tex-font-style-tt">B</span> and <span class="tex-font-style-tt">C</span> and that single mutations can only remove or add substrings at any position in the string (a substring is a contiguous sequence of characters). The substrings that can be removed or added by a mutation are <span class="tex-font-style-tt">AA</span>, <span class="tex-font-style-tt">BB</span>, <span class="tex-font-style-tt">CC</span>, <span class="tex-font-style-tt">ABAB</span> or <span class="tex-font-style-tt">BCBC</span>. During a sequence of mutations a DNA string may even become empty.</p><p>Ron has agreed to sequence the DNA of the weasel and the basilisk for you, but finding out whether there is a sequence of possible mutations that leads from one to the other is too difficult for him, so you have to do it on your own. </p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains an integer $t$ ($1\le t\le 100$) — the number of test cases. The descriptions of the $t$ test cases follow.</p><p>The first line of each test case contains a string $u$ ($1\le |u|\le 200$) — the DNA of the weasel.</p><p>The second line of each test case contains a string $v$ ($1\le |v|\le 200$) — the DNA of the basilisk. </p><p>The values $|u|$, $|v|$ denote the lengths of the strings $u$ and $v$. It is guaranteed that both strings $u$ and $v$ consist of the letters <span class="tex-font-style-tt">A</span>, <span class="tex-font-style-tt">B</span> and <span class="tex-font-style-tt">C</span>.</p></div><div class="output-specification"><p>For each test case, print <span class="tex-font-style-tt">YES</span> if there is a sequence of mutations to get from $u$ to $v$ and <span class="tex-font-style-tt">NO</span> otherwise. </p></div>

## Input

<p>Each test contains multiple test cases. The first line contains an integer $t$ ($1\le t\le 100$) — the number of test cases. The descriptions of the $t$ test cases follow.</p><p>The first line of each test case contains a string $u$ ($1\le |u|\le 200$) — the DNA of the weasel.</p><p>The second line of each test case contains a string $v$ ($1\le |v|\le 200$) — the DNA of the basilisk. </p><p>The values $|u|$, $|v|$ denote the lengths of the strings $u$ and $v$. It is guaranteed that both strings $u$ and $v$ consist of the letters <span class="tex-font-style-tt">A</span>, <span class="tex-font-style-tt">B</span> and <span class="tex-font-style-tt">C</span>.</p>

## Output

<p>For each test case, print <span class="tex-font-style-tt">YES</span> if there is a sequence of mutations to get from $u$ to $v$ and <span class="tex-font-style-tt">NO</span> otherwise. </p>





```input1|2,3,6,7,10,11,14,15
8
A
B
B
C
C
A
AA
BB
BB
CC
CC
AA
ABAB
BCBC
ABC
CBA
```




```output1
NO
NO
NO
YES
YES
YES
YES
NO
```


