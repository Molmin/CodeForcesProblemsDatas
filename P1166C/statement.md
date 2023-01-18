## Description

<div><p>The legend of the foundation of Vectorland talks of two integers $x$ and $y$. Centuries ago, the array king placed two markers at points $|x|$ and $|y|$ on the number line and conquered all the land in between (including the endpoints), which he declared to be Arrayland. Many years later, the vector king placed markers at points $|x - y|$ and $|x + y|$ and conquered all the land in between (including the endpoints), which he declared to be Vectorland. He did so in such a way that the land of Arrayland was completely inside (including the endpoints) the land of Vectorland.</p><p>Here $|z|$ denotes the absolute value of $z$.</p><p>Now, Jose is stuck on a question of his history exam: "What are the values of $x$ and $y$?" Jose doesn't know the answer, but he believes he has narrowed the possible answers down to $n$ integers $a_1, a_2, \dots, a_n$. Now, he wants to know the number of <span class="tex-font-style-bf">unordered</span> pairs formed by two <span class="tex-font-style-bf">different</span> elements from these $n$ integers such that the legend could be true if $x$ and $y$ were equal to these two values. Note that it is possible that Jose is wrong, and that no pairs could possibly make the legend true.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$) &nbsp;— the number of choices.</p><p>The second line contains $n$ pairwise distinct integers $a_1, a_2, \dots, a_n$ ($-10^9 \le a_i \le 10^9$)&nbsp;— the choices Jose is considering.</p></div><div class="output-specification"><p>Print a single integer number&nbsp;— the number of unordered pairs $\{x, y\}$ formed by different numbers from Jose's choices that could make the legend true.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$) &nbsp;— the number of choices.</p><p>The second line contains $n$ pairwise distinct integers $a_1, a_2, \dots, a_n$ ($-10^9 \le a_i \le 10^9$)&nbsp;— the choices Jose is considering.</p>

## Output

<p>Print a single integer number&nbsp;— the number of unordered pairs $\{x, y\}$ formed by different numbers from Jose's choices that could make the legend true.</p>





```input1
3
2 5 -3
```




```input2
2
3 6
```




```output1
2
```




```output2
1
```



## Note

<p>Consider the first sample. For the pair $\{2, 5\}$, the situation looks as follows, with the Arrayland markers at $|2| = 2$ and $|5| = 5$, while the Vectorland markers are located at $|2 - 5| = 3$ and $|2 + 5| = 7$:</p><center> <img class="tex-graphics" src="file://zcQRSG5c.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The legend is not true in this case, because the interval $[2, 3]$ is not conquered by Vectorland. For the pair $\{5, -3\}$ the situation looks as follows, with Arrayland consisting of the interval $[3, 5]$ and Vectorland consisting of the interval $[2, 8]$:</p><center> <img class="tex-graphics" src="file://ZORC6R1W.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>As Vectorland completely contains Arrayland, the legend is true. It can also be shown that the legend is true for the pair $\{2, -3\}$, for a total of two pairs.</p><p>In the second sample, the only pair is $\{3, 6\}$, and the situation looks as follows:</p><center> <img class="tex-graphics" src="file://3wMfqni3.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Note that even though Arrayland and Vectorland share $3$ as endpoint, we still consider Arrayland to be completely inside of Vectorland.</p>
