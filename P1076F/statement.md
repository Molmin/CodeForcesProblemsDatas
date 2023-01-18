## Description

<div><p>Vova has taken his summer practice this year and now he should write a report on how it went.</p><p>Vova has already drawn all the tables and wrote down all the formulas. Moreover, he has already decided that the report will consist of exactly $n$ pages and the $i$-th page will include $x_i$ tables and $y_i$ formulas. The pages are numbered from $1$ to $n$.</p><p>Vova fills the pages one after another, he can't go filling page $i + 1$ before finishing page $i$ and he can't skip pages. </p><p>However, if he draws <span class="tex-font-style-bf">strictly more</span> than $k$ tables in a row or writes <span class="tex-font-style-bf">strictly more</span> than $k$ formulas in a row then he will get bored. Vova wants to rearrange tables and formulas in each page in such a way that he doesn't get bored in the process. Vova can't move some table or some formula to another page.</p><p>Note that the count doesn't reset on the start of the new page. For example, if the page ends with $3$ tables and the next page starts with $5$ tables, then it's counted as $8$ tables in a row.</p><p>Help Vova to determine if he can rearrange tables and formulas on each page in such a way that there is no more than $k$ tables in a row and no more than $k$ formulas in a row.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1 \le n \le 3 \cdot 10^5$, $1 \le k \le 10^6$).</p><p>The second line contains $n$ integers $x_1, x_2, \dots, x_n$ ($1 \le x_i \le 10^6$) — the number of tables on the $i$-th page.</p><p>The third line contains $n$ integers $y_1, y_2, \dots, y_n$ ($1 \le y_i \le 10^6$) — the number of formulas on the $i$-th page.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" if Vova can rearrange tables and formulas on each page in such a way that there is no more than $k$ tables in a row and no more than $k$ formulas in a row.</p><p>Otherwise print "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1 \le n \le 3 \cdot 10^5$, $1 \le k \le 10^6$).</p><p>The second line contains $n$ integers $x_1, x_2, \dots, x_n$ ($1 \le x_i \le 10^6$) — the number of tables on the $i$-th page.</p><p>The third line contains $n$ integers $y_1, y_2, \dots, y_n$ ($1 \le y_i \le 10^6$) — the number of formulas on the $i$-th page.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" if Vova can rearrange tables and formulas on each page in such a way that there is no more than $k$ tables in a row and no more than $k$ formulas in a row.</p><p>Otherwise print "<span class="tex-font-style-tt">NO</span>".</p>





```input1
2 2
5 5
2 2
```




```input2
2 2
5 6
2 2
```




```input3
4 1
4 1 10 1
3 2 10 1
```




```output1
YES
```




```output2
NO
```




```output3
YES
```



## Note

<p>In the first example the only option to rearrange everything is the following (let table be '<span class="tex-font-style-tt">T</span>' and formula be '<span class="tex-font-style-tt">F</span>'): </p><ul> <li> page $1$: "<span class="tex-font-style-tt">TTFTTFT</span>" </li><li> page $2$: "<span class="tex-font-style-tt">TFTTFTT</span>" </li></ul><p>That way all blocks of tables have length $2$.</p><p>In the second example there is no way to fit everything in such a way that there are no more than $2$ tables in a row and $2$ formulas in a row.</p>
