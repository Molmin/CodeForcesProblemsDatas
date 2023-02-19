## Description

<div><p>Monocarp would like to open a bakery in his local area. But, at first, he should figure out whether he can compete with other shops.</p><p>Monocarp plans that the bakery will work for $n$ days. On the $i$-th day, $a_i$ loaves of bread will be baked in the morning before the opening. At the end of the $n$-th day, Monocarp will sell all the remaining bread that wasn't sold earlier with a huge discount.</p><p>Because of how bread is stored, the bakery seller sells the bread in the following order: firstly, he sells the loaves that were baked that morning; secondly, he sells the loaves that were baked the day before and weren't sold yet; then the loaves that were baked two days before and weren't sold yet, and so on. That's why some customers may buy a rather stale bread and will definitely spread negative rumors.</p><p>Let's define loaf <span class="tex-font-style-it">spoilage</span> as the difference between the day it was baked and the day it was sold. Then the <span class="tex-font-style-it">unattractiveness</span> of the bakery will be equal to the maximum spoilage among all loaves of bread baked at the bakery.</p><p>Suppose Monocarp's local area has <span class="tex-font-style-it">consumer demand</span> equal to $k$, it means that each day $k$ customers will come to the bakery and each of them will ask for one loaf of bread (the loaves are sold according to the aforementioned order). If there is no bread left, then the person just doesn't buy anything. During the last day sale, all the remaining loaves will be sold (and they will still count in the calculation of the unattractiveness).</p><p>Monocarp analyzed his competitors' data and came up with $m$ possible consumer demand values $k_1, k_2, \dots, k_m$, and now he'd like to calculate the unattractiveness of the bakery for each value of demand. Can you help him?</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n \le 2 \cdot 10^5$; $1 \le m \le 2 \cdot 10^5$)&nbsp;— the number of days the bakery is open and the number of possible values of consumer demand.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the number of bread loaves that will be baked each day.</p><p>The third line contains $m$ integers $k_1, k_2, \dots, k_m$ ($1 \le k_1 &lt; k_2 &lt; \dots &lt; k_m \le 10^9$)&nbsp;— the possible consumer demand values in the ascending order.</p></div><div class="output-specification"><p>Print $m$ integers: for each consumer demand, print the unattractiveness of the bakery.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n \le 2 \cdot 10^5$; $1 \le m \le 2 \cdot 10^5$)&nbsp;— the number of days the bakery is open and the number of possible values of consumer demand.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the number of bread loaves that will be baked each day.</p><p>The third line contains $m$ integers $k_1, k_2, \dots, k_m$ ($1 \le k_1 &lt; k_2 &lt; \dots &lt; k_m \le 10^9$)&nbsp;— the possible consumer demand values in the ascending order.</p>

## Output

<p>Print $m$ integers: for each consumer demand, print the unattractiveness of the bakery.</p>





```input1
5 4
5 2 1 3 7
1 3 4 10
```




```input2
8 9
3 1 4 1 5 9 2 6
1 2 3 4 5 6 7 8 9
```




```output1
4 2 1 0
```




```output2
7 5 3 3 2 1 1 1 0
```



## Note

<p>In the first example, let's describe what happens for couple consumer demands:</p><p>If consumer demand is equal to $1$: </p><ul> <li> at day $1$: $5$ loaves are baked and only $1$ is sold with spoilage equal to $1 - 1 = 0$; </li><li> at day $2$: $4$ loaves are left and $2$ more are baked. Only $1$ loaf was sold and it was the loaf baked today with spoilage $2 - 2 = 0$; </li><li> at day $3$: $4$ loaves from the first day and $1$ loaf from the second day left. One more loaf was baked and was sold this day with spoilage $3 - 3 = 0$; </li><li> at day $4$: $4$ loaves from the first day and $1$ loaf from the second day left. $3$ more loaves were baked and one of them was sold this day with spoilage $4 - 4 = 0$; </li><li> at day $5$: $4$ loaves from the first day, $1$ loaf from the second day and $2$ loaves from the fourth day left. $7$ more loaves were baked and, since it's the last day, all $14$ loaves were sold. $4$ loaves from the first day have the maximum spoilage equal to $5 - 1 = 4$. </li></ul> In total, the unattractiveness of the bakery will be equal to $4$.<p>If consumer demand is equal to $10$ then all baked bread will be sold in the day it was baked and will have spoilage equal to $0$.</p>
