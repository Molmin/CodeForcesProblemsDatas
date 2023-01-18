## Description

<div><p>During the archaeological research in the Middle East you found the traces of three ancient religions: First religion, Second religion and Third religion. You compiled the information on the evolution of each of these beliefs, and you now wonder if the followers of each religion could coexist in peace.</p><p>The <span class="tex-font-style-underline">Word of Universe</span> is a long word containing the lowercase English characters only. At each moment of time, each of the religion beliefs could be described by a word consisting of lowercase English characters.</p><p>The three religions can coexist in peace if their descriptions form disjoint subsequences of the <span class="tex-font-style-underline">Word of Universe</span>. More formally, one can paint some of the characters of the <span class="tex-font-style-underline">Word of Universe</span> in three colors: $1$, $2$, $3$, so that each character is painted in <span class="tex-font-style-underline">at most</span> one color, and the description of the $i$-th religion can be constructed from the <span class="tex-font-style-underline">Word of Universe</span> by removing all characters that aren't painted in color $i$.</p><p>The religions however evolve. In the beginning, each religion description is empty. Every once in a while, either a character is appended to the end of the description of a single religion, or the last character is dropped from the description. After each change, determine if the religions could coexist in peace.</p></div><div class="input-specification"><p>The first line of the input contains two integers $n, q$ ($1 \leq n \leq 100\,000$, $1 \leq q \leq 1000$) — the length of the <span class="tex-font-style-underline">Word of Universe</span> and the number of religion evolutions, respectively. The following line contains the <span class="tex-font-style-underline">Word of Universe</span> — a string of length $n$ consisting of lowercase English characters.</p><p>Each of the following line describes a single evolution and is in one of the following formats: </p><ul> <li> <span class="tex-font-style-tt">+</span> $i$ $c$ ($i \in \{1, 2, 3\}$, $c \in \{\mathtt{a}, \mathtt{b}, \dots, \mathtt{z}\}$: append the character $c$ to the end of $i$-th religion description. </li><li> <span class="tex-font-style-tt">-</span> $i$ ($i \in \{1, 2, 3\}$) – remove the last character from the $i$-th religion description. You can assume that the pattern is non-empty. </li></ul><p>You can assume that no religion will have description longer than $250$ characters.</p></div><div class="output-specification"><p>Write $q$ lines. The $i$-th of them should be <span class="tex-font-style-tt">YES</span> if the religions could coexist in peace after the $i$-th evolution, or <span class="tex-font-style-tt">NO</span> otherwise.</p><p>You can print each character in any case (either upper or lower).</p></div>

## Input

<p>The first line of the input contains two integers $n, q$ ($1 \leq n \leq 100\,000$, $1 \leq q \leq 1000$) — the length of the <span class="tex-font-style-underline">Word of Universe</span> and the number of religion evolutions, respectively. The following line contains the <span class="tex-font-style-underline">Word of Universe</span> — a string of length $n$ consisting of lowercase English characters.</p><p>Each of the following line describes a single evolution and is in one of the following formats: </p><ul> <li> <span class="tex-font-style-tt">+</span> $i$ $c$ ($i \in \{1, 2, 3\}$, $c \in \{\mathtt{a}, \mathtt{b}, \dots, \mathtt{z}\}$: append the character $c$ to the end of $i$-th religion description. </li><li> <span class="tex-font-style-tt">-</span> $i$ ($i \in \{1, 2, 3\}$) – remove the last character from the $i$-th religion description. You can assume that the pattern is non-empty. </li></ul><p>You can assume that no religion will have description longer than $250$ characters.</p>

## Output

<p>Write $q$ lines. The $i$-th of them should be <span class="tex-font-style-tt">YES</span> if the religions could coexist in peace after the $i$-th evolution, or <span class="tex-font-style-tt">NO</span> otherwise.</p><p>You can print each character in any case (either upper or lower).</p>





```input1
6 8
abdabc
+ 1 a
+ 1 d
+ 2 b
+ 2 c
+ 3 a
+ 3 b
+ 1 c
- 2
```




```input2
6 8
abbaab
+ 1 a
+ 2 a
+ 3 a
+ 1 b
+ 2 b
+ 3 b
- 1
+ 2 z
```




```output1
YES
YES
YES
YES
YES
YES
NO
YES
```




```output2
YES
YES
YES
YES
YES
NO
YES
NO
```



## Note

<p>In the first example, after the 6th evolution the religion descriptions are: <span class="tex-font-style-tt">ad</span>, <span class="tex-font-style-tt">bc</span>, and <span class="tex-font-style-tt">ab</span>. The following figure shows how these descriptions form three disjoint subsequences of the <span class="tex-font-style-underline">Word of Universe</span>:</p><center> <img class="tex-graphics" src="file://hGQNMhbe.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
