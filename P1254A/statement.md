## Description

<div><p>Long is a huge fan of CFC (Codeforces Fried Chicken). But the price of CFC is increasing, so he decides to breed the chicken on his own farm.</p><p>His farm is presented by a rectangle grid with $r$ rows and $c$ columns. Some of these cells contain rice, others are empty. $k$ chickens are living on his farm. <span class="tex-font-style-bf">The number of chickens is not greater than the number of cells with rice on the farm.</span></p><p>Long wants to give his chicken playgrounds by assigning these farm cells to his chickens. He would like to satisfy the following requirements:</p><ul> <li> Each cell of the farm is assigned to <span class="tex-font-style-bf">exactly one</span> chicken. </li><li> Each chicken is assigned <span class="tex-font-style-bf">at least one</span> cell. </li><li> The set of cells assigned to every chicken forms a connected area. More precisely, if two cells $(x, y)$ and $(u, v)$ are assigned to the same chicken, this chicken is able to walk from $(x, y)$ to $(u, v)$ by passing only its cells and moving from each cell to another cell sharing a side. </li></ul><p>Long also wants to prevent his chickens from fighting for food. Hence he wants the difference between the maximum and the minimum number of cells with rice assigned to a chicken to be as small as possible. Please help him.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $T$ ($1 \le T \le 2 \cdot 10^4$). Description of the test cases follows.</p><p>The first line of each test case contains three integers $r$, $c$ and $k$ ($1 \leq r, c \leq 100, 1 \leq k \leq 62$), representing the size of Long's farm and the number of chickens Long has. </p><p>Each of the next $r$ lines contains $c$ characters, each is either "<span class="tex-font-style-tt">.</span>" or "<span class="tex-font-style-tt">R</span>", representing an empty cell or a cell with rice. It is guaranteed that <span class="tex-font-style-bf">the number of chickens is not greater than the number of cells with rice on the farm.</span></p><p>It is guaranteed that the sum of $r \cdot c$ over all test cases does not exceed $2 \cdot 10^4$.</p></div><div class="output-specification"><p>For each test case, print $r$ lines with $c$ characters on each line. Each character should be either a lowercase English character, an uppercase English character, or a digit. Two characters should be equal if and only if the two corresponding cells are assigned to the same chicken. <span class="tex-font-style-bf">Uppercase and lowercase characters are considered different, so "<span class="tex-font-style-tt">A</span>" and "<span class="tex-font-style-tt">a</span>" belong to two different chickens.</span></p><p>If there are multiple optimal answers, print any.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $T$ ($1 \le T \le 2 \cdot 10^4$). Description of the test cases follows.</p><p>The first line of each test case contains three integers $r$, $c$ and $k$ ($1 \leq r, c \leq 100, 1 \leq k \leq 62$), representing the size of Long's farm and the number of chickens Long has. </p><p>Each of the next $r$ lines contains $c$ characters, each is either "<span class="tex-font-style-tt">.</span>" or "<span class="tex-font-style-tt">R</span>", representing an empty cell or a cell with rice. It is guaranteed that <span class="tex-font-style-bf">the number of chickens is not greater than the number of cells with rice on the farm.</span></p><p>It is guaranteed that the sum of $r \cdot c$ over all test cases does not exceed $2 \cdot 10^4$.</p>

## Output

<p>For each test case, print $r$ lines with $c$ characters on each line. Each character should be either a lowercase English character, an uppercase English character, or a digit. Two characters should be equal if and only if the two corresponding cells are assigned to the same chicken. <span class="tex-font-style-bf">Uppercase and lowercase characters are considered different, so "<span class="tex-font-style-tt">A</span>" and "<span class="tex-font-style-tt">a</span>" belong to two different chickens.</span></p><p>If there are multiple optimal answers, print any.</p>





```input1
4
3 5 3
..R..
...R.
....R
6 4 6
R..R
R..R
RRRR
RRRR
R..R
R..R
5 5 4
RRR..
R.R..
RRR..
R..R.
R...R
2 31 62
RRRRRRRRRRRRRRRRRRRRRRRRRRRRRRR
RRRRRRRRRRRRRRRRRRRRRRRRRRRRRRR
```




```output1
11122
22223
33333
aacc
aBBc
aBBc
CbbA
CbbA
CCAA
11114
22244
32444
33344
33334
abcdefghijklmnopqrstuvwxyzABCDE
FGHIJKLMNOPQRSTUVWXYZ0123456789
```



## Note

<p>These pictures explain the sample output. Each color represents one chicken. Cells filled with patterns (not solid colors) contain rice.</p><p>In the first test case, each chicken has one cell with rice. Hence, the difference between the maximum and the minimum number of cells with rice assigned to a chicken is $0$.</p><p><img class="tex-graphics" src="file://jrq0TpjZ.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>In the second test case, there are $4$ chickens with $3$ cells of rice, and $2$ chickens with $2$ cells of rice. Hence, the difference between the maximum and the minimum number of cells with rice assigned to a chicken is $3 - 2 = 1$.</p><p><img class="tex-graphics" src="file://MmVELrMP.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>In the third test case, each chicken has $3$ cells with rice. <img class="tex-graphics" src="file://5zsfUGzv.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>In the last test case, since there are $62$ chicken with exactly $62$ cells of rice, each chicken must be assigned to exactly one cell. The sample output is one of the possible way.</p>
