## Description

<div><p>Let's denote a $k$-step ladder as the following structure: exactly $k + 2$ wooden planks, of which</p><ul> <li> two planks of length <span class="tex-font-style-bf">at least</span> $k+1$ — the base of the ladder; </li><li> $k$ planks of length <span class="tex-font-style-bf">at least</span> $1$ — the steps of the ladder; </li></ul><p>Note that neither the base planks, nor the steps planks are required to be equal.</p><p>For example, ladders $1$ and $3$ are correct $2$-step ladders and ladder $2$ is a correct $1$-step ladder. On the first picture the lengths of planks are $[3, 3]$ for the base and $[1]$ for the step. On the second picture lengths are $[3, 3]$ for the base and $[2]$ for the step. On the third picture lengths are $[3, 4]$ for the base and $[2, 3]$ for the steps. </p><center> <img class="tex-graphics" src="file://uQFDzyaY.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>You have $n$ planks. The length of the $i$-th planks is $a_i$. You don't have a saw, so you can't cut the planks you have. Though you have a hammer and nails, so you can assemble the improvised "ladder" from the planks.</p><p>The question is: what is the maximum number $k$ such that you can choose some subset of the given planks and assemble a $k$-step ladder using them?</p></div><div class="input-specification"><p>The first line contains a single integer $T$ ($1 \le T \le 100$) — the number of queries. The queries are independent.</p><p>Each query consists of two lines. The first line contains a single integer $n$ ($2 \le n \le 10^5$) — the number of planks you have.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^5$) — the lengths of the corresponding planks.</p><p>It's guaranteed that the total number of planks from all queries doesn't exceed $10^5$.</p></div><div class="output-specification"><p>Print $T$ integers — one per query. The $i$-th integer is the maximum number $k$, such that you can choose some subset of the planks given in the $i$-th query and assemble a $k$-step ladder using them.</p><p>Print $0$ if you can't make even $1$-step ladder from the given set of planks.</p></div>

## Input

<p>The first line contains a single integer $T$ ($1 \le T \le 100$) — the number of queries. The queries are independent.</p><p>Each query consists of two lines. The first line contains a single integer $n$ ($2 \le n \le 10^5$) — the number of planks you have.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^5$) — the lengths of the corresponding planks.</p><p>It's guaranteed that the total number of planks from all queries doesn't exceed $10^5$.</p>

## Output

<p>Print $T$ integers — one per query. The $i$-th integer is the maximum number $k$, such that you can choose some subset of the planks given in the $i$-th query and assemble a $k$-step ladder using them.</p><p>Print $0$ if you can't make even $1$-step ladder from the given set of planks.</p>





```input1
4
4
1 3 1 3
3
3 3 2
5
2 3 3 4 2
3
1 1 2
```




```output1
2
1
2
0
```



## Note

<p>Examples for the queries $1-3$ are shown at the image in the legend section.</p><p>The Russian meme to express the quality of the ladders:</p><center> <img class="tex-graphics" src="file://SHoeCsML.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
