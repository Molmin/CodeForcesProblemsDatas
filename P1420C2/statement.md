## Description

<div><p><span class="tex-font-style-bf">This is the hard version of the problem. The difference between the versions is that the easy version has no swap operations. You can make hacks only if all versions of the problem are solved.</span></p><p>Pikachu is a cute and friendly pokémon living in the wild pikachu herd.</p><p>But it has become known recently that infamous team R wanted to steal all these pokémon! Pokémon trainer Andrew decided to help Pikachu to build a pokémon army to resist.</p><p>First, Andrew counted all the pokémon&nbsp;— there were exactly $n$ pikachu. The strength of the $i$-th pokémon is equal to $a_i$, and all these numbers are distinct.</p><p>As an army, Andrew can choose any non-empty subsequence of pokemons. In other words, Andrew chooses some array $b$ from $k$ indices such that $1 \le b_1 &lt; b_2 &lt; \dots &lt; b_k \le n$, and his army will consist of pokémons with forces $a_{b_1}, a_{b_2}, \dots, a_{b_k}$.</p><p>The strength of the army is equal to the alternating sum of elements of the subsequence; that is, $a_{b_1} - a_{b_2} + a_{b_3} - a_{b_4} + \dots$.</p><p>Andrew is experimenting with pokémon order. He performs $q$ operations. In $i$-th operation Andrew swaps $l_i$-th and $r_i$-th pokémon.</p><p>Andrew wants to know the maximal stregth of the army he can achieve with the initial pokémon placement. He also needs to know the maximal strength after each operation.</p><p>Help Andrew and the pokémon, or team R will realize their tricky plan!</p></div><div class="input-specification"><p>Each test contains multiple test cases.</p><p>The first line contains one positive integer $t$ ($1 \le t \le 10^3$) denoting the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $q$ ($1 \le n \le 3 \cdot 10^5, 0 \le q \le 3 \cdot 10^5$) denoting the number of pokémon and number of operations respectively.</p><p>The second line contains $n$ distinct positive integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$) denoting the strengths of the pokémon.</p><p>$i$-th of the last $q$ lines contains two positive integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le n$) denoting the indices of pokémon that were swapped in the $i$-th operation.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3 \cdot 10^5$, and the sum of $q$ over all test cases does not exceed $3 \cdot 10^5$. </p></div><div class="output-specification"><p>For each test case, print $q+1$ integers: the maximal strength of army before the swaps and after each swap.</p></div>

## Input

<p>Each test contains multiple test cases.</p><p>The first line contains one positive integer $t$ ($1 \le t \le 10^3$) denoting the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $q$ ($1 \le n \le 3 \cdot 10^5, 0 \le q \le 3 \cdot 10^5$) denoting the number of pokémon and number of operations respectively.</p><p>The second line contains $n$ distinct positive integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$) denoting the strengths of the pokémon.</p><p>$i$-th of the last $q$ lines contains two positive integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le n$) denoting the indices of pokémon that were swapped in the $i$-th operation.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3 \cdot 10^5$, and the sum of $q$ over all test cases does not exceed $3 \cdot 10^5$. </p>

## Output

<p>For each test case, print $q+1$ integers: the maximal strength of army before the swaps and after each swap.</p>





```input1
3
3 1
1 3 2
1 2
2 2
1 2
1 2
1 2
7 5
1 2 5 4 3 6 7
1 2
6 7
3 4
1 2
2 3
```




```output1
3
4
2
2
2
9
10
10
10
9
11
```



## Note

<p>Let's look at the third test case:</p><p>Initially we can build an army in such way: [1 2 <span class="tex-font-style-bf">5</span> 4 <span class="tex-font-style-bf">3</span> 6 <span class="tex-font-style-bf">7</span>], its strength will be $5-3+7=9$.</p><p>After first operation we can build an army in such way: [<span class="tex-font-style-bf">2</span> <span class="tex-font-style-bf">1</span> <span class="tex-font-style-bf">5</span> 4 <span class="tex-font-style-bf">3</span> 6 <span class="tex-font-style-bf">7</span>], its strength will be $2-1+5-3+7=10$.</p><p>After second operation we can build an army in such way: [<span class="tex-font-style-bf">2</span> <span class="tex-font-style-bf">1</span> <span class="tex-font-style-bf">5</span> 4 <span class="tex-font-style-bf">3</span> <span class="tex-font-style-bf">7</span> 6], its strength will be $2-1+5-3+7=10$.</p><p>After third operation we can build an army in such way: [<span class="tex-font-style-bf">2</span> <span class="tex-font-style-bf">1</span> 4 <span class="tex-font-style-bf">5</span> <span class="tex-font-style-bf">3</span> <span class="tex-font-style-bf">7</span> 6], its strength will be $2-1+5-3+7=10$.</p><p>After forth operation we can build an army in such way: [1 2 4 <span class="tex-font-style-bf">5</span> <span class="tex-font-style-bf">3</span> <span class="tex-font-style-bf">7</span> 6], its strength will be $5-3+7=9$.</p><p>After all operations we can build an army in such way: [1 <span class="tex-font-style-bf">4</span> <span class="tex-font-style-bf">2</span> <span class="tex-font-style-bf">5</span> <span class="tex-font-style-bf">3</span> <span class="tex-font-style-bf">7</span> 6], its strength will be $4-2+5-3+7=11$.</p>
