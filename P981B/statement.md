## Description

<div><p>Two famous competing companies <span class="tex-font-style-it">ChemForces</span> and <span class="tex-font-style-it">TopChemist</span> decided to show their sets of recently discovered chemical elements on an exhibition. However they know that no element should be present in the sets of both companies.</p><p>In order to avoid this representatives of both companies decided to make an agreement on the sets the companies should present. The sets should be chosen in the way that maximizes the total income of the companies.</p><p>All elements are enumerated with integers. The <span class="tex-font-style-it">ChemForces</span> company has discovered $n$ distinct chemical elements with indices $a_1, a_2, \ldots, a_n$, and will get an income of $x_i$ Berland rubles if the $i$-th element from this list is in the set of this company.</p><p>The <span class="tex-font-style-it">TopChemist</span> company discovered $m$ distinct chemical elements with indices $b_1, b_2, \ldots, b_m$, and it will get an income of $y_j$ Berland rubles for including the $j$-th element from this list to its set.</p><p>In other words, the first company can present any subset of elements from $\{a_1, a_2, \ldots, a_n\}$ (possibly empty subset), the second company can present any subset of elements from $\{b_1, b_2, \ldots, b_m\}$ (possibly empty subset). There shouldn't be equal elements in the subsets.</p><p>Help the representatives select the sets in such a way that no element is presented in both sets and the total income is the maximum possible.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \leq n \leq 10^5$) &nbsp;— the number of elements discovered by <span class="tex-font-style-it">ChemForces</span>.</p><p>The $i$-th of the next $n$ lines contains two integers $a_i$ and $x_i$ ($1 \leq a_i \leq 10^9$, $1 \leq x_i \leq 10^9$) &nbsp;— the index of the $i$-th element and the income of its usage on the exhibition. It is guaranteed that all $a_i$ are distinct.</p><p>The next line contains a single integer $m$ ($1 \leq m \leq 10^5$) &nbsp;— the number of chemicals invented by <span class="tex-font-style-it">TopChemist</span>.</p><p>The $j$-th of the next $m$ lines contains two integers $b_j$ and $y_j$, ($1 \leq b_j \leq 10^9$, $1 \leq y_j \leq 10^9$) &nbsp;— the index of the $j$-th element and the income of its usage on the exhibition. It is guaranteed that all $b_j$ are distinct.</p></div><div class="output-specification"><p>Print the maximum total income you can obtain by choosing the sets for both companies in such a way that no element is presented in both sets.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \leq n \leq 10^5$) &nbsp;— the number of elements discovered by <span class="tex-font-style-it">ChemForces</span>.</p><p>The $i$-th of the next $n$ lines contains two integers $a_i$ and $x_i$ ($1 \leq a_i \leq 10^9$, $1 \leq x_i \leq 10^9$) &nbsp;— the index of the $i$-th element and the income of its usage on the exhibition. It is guaranteed that all $a_i$ are distinct.</p><p>The next line contains a single integer $m$ ($1 \leq m \leq 10^5$) &nbsp;— the number of chemicals invented by <span class="tex-font-style-it">TopChemist</span>.</p><p>The $j$-th of the next $m$ lines contains two integers $b_j$ and $y_j$, ($1 \leq b_j \leq 10^9$, $1 \leq y_j \leq 10^9$) &nbsp;— the index of the $j$-th element and the income of its usage on the exhibition. It is guaranteed that all $b_j$ are distinct.</p>

## Output

<p>Print the maximum total income you can obtain by choosing the sets for both companies in such a way that no element is presented in both sets.</p>





```input1
3
1 2
7 2
3 10
4
1 4
2 4
3 4
4 4

```




```input2
1
1000000000 239
3
14 15
92 65
35 89

```




```output1
24

```




```output2
408

```



## Note

<p>In the first example <span class="tex-font-style-it">ChemForces</span> can choose the set ($3, 7$), while <span class="tex-font-style-it">TopChemist</span> can choose ($1, 2, 4$). This way the total income is $(10 + 2) + (4 + 4 + 4) = 24$.</p><p>In the second example <span class="tex-font-style-it">ChemForces</span> can choose the only element $10^9$, while <span class="tex-font-style-it">TopChemist</span> can choose ($14, 92, 35$). This way the total income is $(239) + (15 + 65 + 89) = 408$.</p>
