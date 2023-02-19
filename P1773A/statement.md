## Description

<div><p>Alice is a magician and she creates a new trick. She has $n$ cards with different numbers from $1$ to $n$ written on them. First, she asks an audience member to shuffle the deck and put cards in a row. Let's say the $i$-th card from the left has the number $a_i$ on it. </p><p>Then Alice picks two permutations $p$ and $q$. There is a restriction on $p$ and $q$&nbsp;— <span class="tex-font-style-bf">permutations can't have fixed points</span>. Which means $\forall i: p_i \ne i\ and\ q_i \ne i$.</p><p>After permutations are chosen, Alice shuffles the cards according to them. Now the $i$-th card from the left is the card $a[p[q[i]]$. The trick is considered successful if $i$-th card from the left has the number $i$ on it after the shuffles.</p><p>Help Alice pick the permutations $p$ and $q$ or say it is not possible for the specific starting permutation $a$. </p></div><div class="input-specification"><p>The first line of the input contains the number of tests $t$ ($1 \leq t \leq 10^5$). </p><p>Each test is described in two lines. The first line contains one integer $n$&nbsp;— the number of cards ($1 \leq n \leq 10^5$). The second line contains $n$ integers $a_i$&nbsp;— the initial permutation of the cards ($1 \leq a_i \leq n$; $\forall i \neq j: a_i \neq a_j$). </p><p>It is guaranteed that the sum of $n$ over all tests does not exceed $10^5$.</p></div><div class="output-specification"><p>Print the answer for each test case in the same order the cases appear in the input.</p><p>For each test case, print "<span class="tex-font-style-tt">Impossible</span>" in a single line, if no solution exists.</p><p>Otherwise, print "<span class="tex-font-style-tt">Possible</span>" in the first line, and in the following two lines print permutations $p$ and $q$.</p></div>

## Input

<p>The first line of the input contains the number of tests $t$ ($1 \leq t \leq 10^5$). </p><p>Each test is described in two lines. The first line contains one integer $n$&nbsp;— the number of cards ($1 \leq n \leq 10^5$). The second line contains $n$ integers $a_i$&nbsp;— the initial permutation of the cards ($1 \leq a_i \leq n$; $\forall i \neq j: a_i \neq a_j$). </p><p>It is guaranteed that the sum of $n$ over all tests does not exceed $10^5$.</p>

## Output

<p>Print the answer for each test case in the same order the cases appear in the input.</p><p>For each test case, print "<span class="tex-font-style-tt">Impossible</span>" in a single line, if no solution exists.</p><p>Otherwise, print "<span class="tex-font-style-tt">Possible</span>" in the first line, and in the following two lines print permutations $p$ and $q$.</p>





```input1|2,3,6,7
4
2
2 1
3
1 2 3
4
2 1 4 3
5
5 1 4 2 3
```




```output1
Impossible
Possible
3 1 2
2 3 1
Possible
3 4 2 1
3 4 2 1
Possible
4 1 2 5 3
3 1 4 5 2
```


