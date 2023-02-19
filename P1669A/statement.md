## Description

<div><p>Codeforces separates its users into $4$ divisions by their rating:</p><ul> <li> For Division 1: $1900 \leq \mathrm{rating}$ </li><li> For Division 2: $1600 \leq \mathrm{rating} \leq 1899$ </li><li> For Division 3: $1400 \leq \mathrm{rating} \leq 1599$ </li><li> For Division 4: $\mathrm{rating} \leq 1399$ </li></ul><p>Given a $\mathrm{rating}$, print in which division the $\mathrm{rating}$ belongs.</p></div><div class="input-specification"><p>The first line of the input contains an integer $t$ ($1 \leq t \leq 10^4$) — the number of testcases.</p><p>The description of each test consists of one line containing one integer $\mathrm{rating}$ ($-5000 \leq \mathrm{rating} \leq 5000$).</p></div><div class="output-specification"><p>For each test case, output a single line containing the correct division in the format "<span class="tex-font-style-tt">Division X</span>", where $X$ is an integer between $1$ and $4$ representing the division for the corresponding rating.</p></div>

## Input

<p>The first line of the input contains an integer $t$ ($1 \leq t \leq 10^4$) — the number of testcases.</p><p>The description of each test consists of one line containing one integer $\mathrm{rating}$ ($-5000 \leq \mathrm{rating} \leq 5000$).</p>

## Output

<p>For each test case, output a single line containing the correct division in the format "<span class="tex-font-style-tt">Division X</span>", where $X$ is an integer between $1$ and $4$ representing the division for the corresponding rating.</p>





```input1
7
-789
1299
1300
1399
1400
1679
2300
```




```output1
Division 4
Division 4
Division 4
Division 4
Division 3
Division 2
Division 1
```



## Note

<p>For test cases $1-4$, the corresponding ratings are $-789$, $1299$, $1300$, $1399$, so all of them are in division $4$.</p><p>For the fifth test case, the corresponding rating is $1400$, so it is in division $3$.</p><p>For the sixth test case, the corresponding rating is $1679$, so it is in division $2$.</p><p>For the seventh test case, the corresponding rating is $2300$, so it is in division $1$.</p>
