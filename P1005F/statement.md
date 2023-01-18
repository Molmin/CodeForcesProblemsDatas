## Description

<div><p>There are $n$ cities in Berland. Some pairs of cities are connected by roads. All roads are bidirectional. Each road connects two different cities. There is at most one road between a pair of cities. The cities are numbered from $1$ to $n$.</p><p>It is known that, from the capital (the city with the number $1$), you can reach any other city by moving along the roads.</p><p>The President of Berland plans to improve the country's road network. The budget is enough to repair exactly $n-1$ roads. The President plans to choose a set of $n-1$ roads such that:</p><ul> <li> it is possible to travel from the capital to any other city along the $n-1$ chosen roads, </li><li> if $d_i$ is the number of roads needed to travel from the capital to city $i$, moving only along the $n-1$ chosen roads, then $d_1 + d_2 + \dots + d_n$ is minimized (i.e. as minimal as possible). </li></ul><p>In other words, the set of $n-1$ roads should preserve the connectivity of the country, and the sum of distances from city $1$ to all cities should be minimized (where you can only use the $n-1$ chosen roads).</p><p>The president instructed the ministry to prepare $k$ possible options to choose $n-1$ roads so that both conditions above are met.</p><p>Write a program that will find $k$ possible ways to choose roads for repair. If there are fewer than $k$ ways, then the program should output all possible valid ways to choose roads.</p></div><div class="input-specification"><p>The first line of the input contains integers $n$, $m$ and $k$ ($2 \le n \le 2\cdot10^5, n-1 \le m \le 2\cdot10^5, 1 \le k \le 2\cdot10^5$), where $n$ is the number of cities in the country, $m$ is the number of roads and $k$ is the number of options to choose a set of roads for repair. It is guaranteed that $m \cdot k \le 10^6$.</p><p>The following $m$ lines describe the roads, one road per line. Each line contains two integers $a_i$, $b_i$ ($1 \le a_i, b_i \le n$, $a_i \ne b_i$) — the numbers of the cities that the $i$-th road connects. There is at most one road between a pair of cities. The given set of roads is such that you can reach any city from the capital.</p></div><div class="output-specification"><p>Print $t$ ($1 \le t \le k$) — the number of ways to choose a set of roads for repair. Recall that you need to find $k$ different options; if there are fewer than $k$ of them, then you need to find all possible different valid options.</p><p>In the following $t$ lines, print the options, one per line. Print an option as a string of $m$ characters where the $j$-th character is equal to '<span class="tex-font-style-tt">1</span>' if the $j$-th road is included in the option, and is equal to '<span class="tex-font-style-tt">0</span>' if the road is not included. The roads should be numbered according to their order in the input. The options can be printed in any order. All the $t$ lines should be different.</p><p>Since it is guaranteed that $m \cdot k \le 10^6$, the total length of all the $t$ lines will not exceed $10^6$.</p><p>If there are several answers, output any of them.</p></div>

## Input

<p>The first line of the input contains integers $n$, $m$ and $k$ ($2 \le n \le 2\cdot10^5, n-1 \le m \le 2\cdot10^5, 1 \le k \le 2\cdot10^5$), where $n$ is the number of cities in the country, $m$ is the number of roads and $k$ is the number of options to choose a set of roads for repair. It is guaranteed that $m \cdot k \le 10^6$.</p><p>The following $m$ lines describe the roads, one road per line. Each line contains two integers $a_i$, $b_i$ ($1 \le a_i, b_i \le n$, $a_i \ne b_i$) — the numbers of the cities that the $i$-th road connects. There is at most one road between a pair of cities. The given set of roads is such that you can reach any city from the capital.</p>

## Output

<p>Print $t$ ($1 \le t \le k$) — the number of ways to choose a set of roads for repair. Recall that you need to find $k$ different options; if there are fewer than $k$ of them, then you need to find all possible different valid options.</p><p>In the following $t$ lines, print the options, one per line. Print an option as a string of $m$ characters where the $j$-th character is equal to '<span class="tex-font-style-tt">1</span>' if the $j$-th road is included in the option, and is equal to '<span class="tex-font-style-tt">0</span>' if the road is not included. The roads should be numbered according to their order in the input. The options can be printed in any order. All the $t$ lines should be different.</p><p>Since it is guaranteed that $m \cdot k \le 10^6$, the total length of all the $t$ lines will not exceed $10^6$.</p><p>If there are several answers, output any of them.</p>





```input1
4 4 3
1 2
2 3
1 4
4 3

```




```input2
4 6 3
1 2
2 3
1 4
4 3
2 4
1 3

```




```input3
5 6 2
1 2
1 3
2 4
2 5
3 4
3 5

```




```output1
2
1110
1011

```




```output2
1
101001

```




```output3
2
111100
110110

```


