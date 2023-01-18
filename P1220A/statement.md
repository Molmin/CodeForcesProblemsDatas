## Description

<div><p>When Serezha was three years old, he was given a set of cards with letters for his birthday. They were arranged into words in the way which formed the boy's mother favorite number in binary notation. Serezha started playing with them immediately and shuffled them because he wasn't yet able to read. His father decided to rearrange them. Help him restore the original number, on condition that it was the maximum possible one. </p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \leqslant n \leqslant 10^5$)&nbsp;— the length of the string. The second line contains a string consisting of English lowercase letters: '<span class="tex-font-style-tt">z</span>', '<span class="tex-font-style-tt">e</span>', '<span class="tex-font-style-tt">r</span>', '<span class="tex-font-style-tt">o</span>' and '<span class="tex-font-style-tt">n</span>'.</p><p>It is guaranteed that it is possible to rearrange the letters in such a way that they form a sequence of words, each being either "<span class="tex-font-style-tt">zero</span>" which corresponds to the digit $0$ or "<span class="tex-font-style-tt">one</span>" which corresponds to the digit $1$.</p></div><div class="output-specification"><p>Print the maximum possible number in binary notation. Print binary digits separated by a space. The leading zeroes are allowed.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \leqslant n \leqslant 10^5$)&nbsp;— the length of the string. The second line contains a string consisting of English lowercase letters: '<span class="tex-font-style-tt">z</span>', '<span class="tex-font-style-tt">e</span>', '<span class="tex-font-style-tt">r</span>', '<span class="tex-font-style-tt">o</span>' and '<span class="tex-font-style-tt">n</span>'.</p><p>It is guaranteed that it is possible to rearrange the letters in such a way that they form a sequence of words, each being either "<span class="tex-font-style-tt">zero</span>" which corresponds to the digit $0$ or "<span class="tex-font-style-tt">one</span>" which corresponds to the digit $1$.</p>

## Output

<p>Print the maximum possible number in binary notation. Print binary digits separated by a space. The leading zeroes are allowed.</p>





```input1
4
ezor
```




```input2
10
nznooeeoer
```




```output1
0
```




```output2
1 1 0
```



## Note

<p>In the first example, the correct initial ordering is "<span class="tex-font-style-tt">zero</span>".</p><p>In the second example, the correct initial ordering is "<span class="tex-font-style-tt">oneonezero</span>".</p>
