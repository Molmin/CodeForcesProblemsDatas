## Description

<div><p>Martian scientists explore Ganymede, one of Jupiter's numerous moons. Recently, they have found ruins of an ancient civilization. The scientists brought to Mars some tablets with writings in a language unknown to science.</p><p>They found out that the inhabitants of Ganymede used an alphabet consisting of two letters, and each word was exactly $\ell$ letters long. So, the scientists decided to write each word of this language as an integer from $0$ to $2^{\ell} - 1$ inclusively. The first letter of the alphabet corresponds to zero bit in this integer, and the second letter corresponds to one bit.</p><p>The same word may have various forms in this language. Then, you need to restore the initial form. The process of doing it is described below.</p><p>Denote the <span class="tex-font-style-it">distance</span> between two words as the amount of positions, in which these words differ. For example, the distance between $1001_2$ and $1100_2$ (in binary) is equal to two, as these words have different letters in the second and the fourth positions, counting from left to right. Further, denote the distance between words $x$ and $y$ as $d(x, y)$.</p><p>Let the word have $n$ forms, the $i$-th of which is described with an integer $x_i$. All the $x_i$ are not necessarily different, as two various forms of the word can be written the same. Consider some word $y$. Then, <span class="tex-font-style-it">closeness</span> of the word $y$ is equal to the sum of distances to each of the word forms, i.&nbsp;e. the sum $d(x_i, y)$ over all $1 \le i \le n$.</p><p>The initial form is the word $y$ with minimal possible nearness.</p><p>You need to help the scientists and write the program which finds the initial form of the word given all its known forms. Note that the initial form is <span class="tex-font-style-bf">not necessarily</span> equal to any of the $n$ given forms.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 100$) — the number of test cases. The following are descriptions of the test cases.</p><p>The first line contains two integers $n$ and $\ell$ ($1 \le n \le 100$, $1 \le \ell \le 30$) — the amount of word forms, and the number of letters in one word.</p><p>The second line contains $n$ integers $x_i$ ($0 \le x_i \le 2^\ell - 1$) — word forms. The integers are not necessarily different.</p></div><div class="output-specification"><p>For each test, print a single integer, the initial form of the word, i.&nbsp;e. such $y$ ($0 \le y \le 2^\ell - 1$) that the sum $d(x_i, y)$ over all $1 \le i \le n$ is minimal possible. Note that $y$ can differ from all the integers $x_i$.</p><p>If there are multiple ways to restore the initial form, print any.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 100$) — the number of test cases. The following are descriptions of the test cases.</p><p>The first line contains two integers $n$ and $\ell$ ($1 \le n \le 100$, $1 \le \ell \le 30$) — the amount of word forms, and the number of letters in one word.</p><p>The second line contains $n$ integers $x_i$ ($0 \le x_i \le 2^\ell - 1$) — word forms. The integers are not necessarily different.</p>

## Output

<p>For each test, print a single integer, the initial form of the word, i.&nbsp;e. such $y$ ($0 \le y \le 2^\ell - 1$) that the sum $d(x_i, y)$ over all $1 \le i \le n$ is minimal possible. Note that $y$ can differ from all the integers $x_i$.</p><p>If there are multiple ways to restore the initial form, print any.</p>





```input1
7
3 5
18 9 21
3 5
18 18 18
1 1
1
5 30
1 2 3 4 5
6 10
99 35 85 46 78 55
2 1
0 1
8 8
5 16 42 15 83 65 78 42
```




```output1
17
18
1
1
39
0
2
```



## Note

<p>In the first test case, the words can be written as $x_1 = 10010_2$, $x_2 = 01001_2$ and $x_3 = 10101_2$ in binary. Let $y = 10001_2$. Then, $d(x_1, y) = 2$ (the difference is in the fourth and the fifth positions), $d(x_2, y) = 2$ (the difference is in the first and the second positions), $d(x_3, y) = 1$ (the difference is in the third position). So, the closeness is $2 + 2 + 1 = 5$. It can be shown that you cannot achieve smaller closeness.</p><p>In the second test case, all the forms are equal to $18$ ($10010_2$ in binary), so the initial form is also $18$. It's easy to see that closeness is equal to zero in this case.</p>
