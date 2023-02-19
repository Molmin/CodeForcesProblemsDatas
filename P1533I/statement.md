## Description

<div><p>Irina works in an excursion company in Saratov. Today, she is going to organize excursions in the cities of Saratov and Engels.</p><p>There are $n_1$ sights in Saratov and $n_2$ sights in Engels. The cities are separated by a river, but there are $m$ bus routes that go along the bridges and allow tourists to go from Saratov to Engels and vice versa. The $i$-th bus route goes from the $x_i$-th sight in Saratov to the $y_i$-th sight in Engels, and in the opposite direction as well.</p><p>Irina wants to plan excursions for the current day. The excursion trips start in Saratov in the morning, continue in Engels in the afternoon, and finish in Saratov in the evening.</p><p>Each tourist starts their excursion day at some sight in Saratov, $k_i$ tourists start at the $i$-th sight. Then the tour guides lead them to Engels: at each sight in Saratov, a tour guide chooses a bus route leading from this sight to Engels, and <span class="tex-font-style-bf">all the tourists starting from this sight</span> transfer to Engels along this bus route. After the excursions in Engels are finished, the same thing happens: at each sight in Engels, a tour guide chooses a bus route leading from this sight to Saratov, and <span class="tex-font-style-bf">all the tourists at this sight</span> transfer to Saratov along this bus route.</p><p>This process can lead to a situation such that some tourists return to the same sight in Saratov where they started in the morning. Obviously, tourists don't like it; so Irina wants to choose where the tour guides take the tourists (both on the way from Saratov to Engels and on the way from Engels to Saratov), so that the minimum possible number of tourists return to the same sight where they started. Help Irina to find an optimal plan!</p></div><div class="input-specification"><p>The first line contains three integers $n_1$, $n_2$ and $m$ ($1 \le n_1, n_2 \le 100$; $\max(n_1, n_2) \le m \le n_1 \cdot n_2$) — the number of sights in Saratov, the number of sights in Engels, and the number of bus routes, respectively.</p><p>The second line contains $n_1$ integers $k_1, k_2, \dots, k_{n_1}$ ($1 \le k_i \le 10^6$), where $k_i$ is the number of tourists starting at the $i$-th sight in Saratov.</p><p>Then $m$ lines follow, each describing a bus route: the $i$-th line contains two integers $x_i$ and $y_i$ ($1 \le x_i \le n_1$; $1 \le y_i \le n_2$) meaning that the $i$-th bus route connects the $x_i$-th sight in Saratov and the $y_i$-th sight in Engels. All these bus routes are distinct, and each sight has at least one bus route leading to/from it.</p></div><div class="output-specification"><p>Print one integer — the minimum possible number of tourists that will return to the same sight where they started.</p></div>

## Input

<p>The first line contains three integers $n_1$, $n_2$ and $m$ ($1 \le n_1, n_2 \le 100$; $\max(n_1, n_2) \le m \le n_1 \cdot n_2$) — the number of sights in Saratov, the number of sights in Engels, and the number of bus routes, respectively.</p><p>The second line contains $n_1$ integers $k_1, k_2, \dots, k_{n_1}$ ($1 \le k_i \le 10^6$), where $k_i$ is the number of tourists starting at the $i$-th sight in Saratov.</p><p>Then $m$ lines follow, each describing a bus route: the $i$-th line contains two integers $x_i$ and $y_i$ ($1 \le x_i \le n_1$; $1 \le y_i \le n_2$) meaning that the $i$-th bus route connects the $x_i$-th sight in Saratov and the $y_i$-th sight in Engels. All these bus routes are distinct, and each sight has at least one bus route leading to/from it.</p>

## Output

<p>Print one integer — the minimum possible number of tourists that will return to the same sight where they started.</p>





```input1
2 1 2
10 20
1 1
2 1
```




```input2
3 3 6
10 20 30
1 3
3 1
2 3
2 1
3 2
1 2
```




```output1
10
```




```output2
0
```


