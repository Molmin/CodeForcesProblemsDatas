## Description

<div><p>There were $n$ types of swords in the theater basement which had been used during the plays. Moreover there were <span class="tex-font-style-bf">exactly</span> $x$ swords of each type. $y$ people have broken into the theater basement and each of them has taken exactly $z$ swords of some <span class="tex-font-style-bf">single type</span>. Note that different people might have taken different types of swords. Note that the values $x, y$ and $z$ are unknown for you.</p><p>The next morning the director of the theater discovers the loss. He counts all swords — exactly $a_i$ swords of the $i$-th type are left untouched.</p><p>The director has no clue about the initial number of swords of each type in the basement, the number of people who have broken into the basement and how many swords each of them have taken.</p><p>For example, if $n=3$, $a = [3, 12, 6]$ then one of the possible situations is $x=12$, $y=5$ and $z=3$. Then the first three people took swords of the first type and the other two people took swords of the third type. Note that you don't know values $x, y$ and $z$ beforehand but know values of $n$ and $a$.</p><p>Thus he seeks for your help. Determine the <span class="tex-font-style-bf">minimum</span> number of people $y$, which could have broken into the theater basement, and the number of swords $z$ each of them has taken.</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ $(2 \le n \le 2 \cdot 10^{5})$ — the number of types of swords.</p><p>The second line of the input contains the sequence $a_1, a_2, \dots, a_n$ $(0 \le a_i \le 10^{9})$, where $a_i$ equals to the number of swords of the $i$-th type, which have remained in the basement after the theft. It is guaranteed that there exists at least one such pair of indices $(j, k)$ that $a_j \neq a_k$.</p></div><div class="output-specification"><p>Print two integers $y$ and $z$ — the minimum number of people which could have broken into the basement and the number of swords each of them has taken.</p></div>

## Input

<p>The first line of the input contains one integer $n$ $(2 \le n \le 2 \cdot 10^{5})$ — the number of types of swords.</p><p>The second line of the input contains the sequence $a_1, a_2, \dots, a_n$ $(0 \le a_i \le 10^{9})$, where $a_i$ equals to the number of swords of the $i$-th type, which have remained in the basement after the theft. It is guaranteed that there exists at least one such pair of indices $(j, k)$ that $a_j \neq a_k$.</p>

## Output

<p>Print two integers $y$ and $z$ — the minimum number of people which could have broken into the basement and the number of swords each of them has taken.</p>





```input1
3
3 12 6
```




```input2
2
2 9
```




```input3
7
2 1000000000 4 6 8 4 2
```




```input4
6
13 52 0 13 26 52
```




```output1
5 3
```




```output2
1 7
```




```output3
2999999987 2
```




```output4
12 13
```



## Note

<p>In the first example the minimum value of $y$ equals to $5$, i.e. the minimum number of people who could have broken into the basement, is $5$. Each of them has taken $3$ swords: three of them have taken $3$ swords of the first type, and two others have taken $3$ swords of the third type.</p><p>In the second example the minimum value of $y$ is $1$, i.e. the minimum number of people who could have broken into the basement, equals to $1$. He has taken $7$ swords of the first type.</p>
