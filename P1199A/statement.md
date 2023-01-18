## Description

<div><p>For years, the Day of city N was held in the most rainy day of summer. New mayor decided to break this tradition and select a <span class="tex-font-style-it">not-so-rainy</span> day for the celebration. The mayor knows the weather forecast for the $n$ days of summer. On the $i$-th day, $a_i$ millimeters of rain will fall. All values $a_i$ are distinct.</p><p>The mayor knows that citizens will watch the weather $x$ days before the celebration and $y$ days after. Because of that, he says that a day $d$ is <span class="tex-font-style-it">not-so-rainy</span> if $a_d$ is smaller than rain amounts at each of $x$ days before day $d$ and and each of $y$ days after day $d$. In other words, $a_d &lt; a_j$ should hold for all $d - x \le j &lt; d$ and $d &lt; j \le d + y$. Citizens only watch the weather during summer, so we only consider such $j$ that $1 \le j \le n$.</p><p>Help mayor find the <span class="tex-font-style-bf">earliest</span> <span class="tex-font-style-it">not-so-rainy</span> day of summer.</p></div><div class="input-specification"><p>The first line contains three integers $n$, $x$ and $y$ ($1 \le n \le 100\,000$, $0 \le x, y \le 7$)&nbsp;— the number of days in summer, the number of days citizens watch the weather before the celebration and the number of days they do that after.</p><p>The second line contains $n$ distinct integers $a_1$, $a_2$, ..., $a_n$ ($1 \le a_i \le 10^9$), where $a_i$ denotes the rain amount on the $i$-th day.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the index of the earliest <span class="tex-font-style-it">not-so-rainy</span> day of summer. We can show that the answer always exists.</p></div>

## Input

<p>The first line contains three integers $n$, $x$ and $y$ ($1 \le n \le 100\,000$, $0 \le x, y \le 7$)&nbsp;— the number of days in summer, the number of days citizens watch the weather before the celebration and the number of days they do that after.</p><p>The second line contains $n$ distinct integers $a_1$, $a_2$, ..., $a_n$ ($1 \le a_i \le 10^9$), where $a_i$ denotes the rain amount on the $i$-th day.</p>

## Output

<p>Print a single integer&nbsp;— the index of the earliest <span class="tex-font-style-it">not-so-rainy</span> day of summer. We can show that the answer always exists.</p>





```input1
10 2 2
10 9 6 7 8 3 2 1 4 5
```




```input2
10 2 3
10 9 6 7 8 3 2 1 4 5
```




```input3
5 5 5
100000 10000 1000 100 10
```




```output1
3
```




```output2
8
```




```output3
5
```



## Note

<p>In the first example days $3$ and $8$ are <span class="tex-font-style-it">not-so-rainy</span>. The $3$-rd day is earlier.</p><p>In the second example day $3$ is not <span class="tex-font-style-it">not-so-rainy</span>, because $3 + y = 6$ and $a_3 &gt; a_6$. Thus, day $8$ is the answer. Note that $8 + y = 11$, but we don't consider day $11$, because it is not summer.</p>
