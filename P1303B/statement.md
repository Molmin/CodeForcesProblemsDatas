## Description

<div><p>Your company was appointed to lay new asphalt on the highway of length $n$. You know that every day you can either repair one unit of the highway (lay new asphalt over one unit of the highway) or skip repairing.</p><p>Skipping the repair is necessary because of the climate. The climate in your region is periodical: there are $g$ days when the weather is good and if you lay new asphalt these days it becomes high-quality pavement; after that, the weather during the next $b$ days is bad, and if you lay new asphalt these days it becomes low-quality pavement; again $g$ good days, $b$ bad days and so on.</p><p>You can be sure that you start repairing at the start of a good season, in other words, days $1, 2, \dots, g$ are good.</p><p>You don't really care about the quality of the highway, you just want to make sure that <span class="tex-font-style-bf">at least half of the highway</span> will have high-quality pavement. For example, if the $n = 5$ then at least $3$ units of the highway should have high quality; if $n = 4$ then at least $2$ units should have high quality.</p><p>What is the minimum number of days is needed to finish the repair of <span class="tex-font-style-bf">the whole highway</span>?</p></div><div class="input-specification"><p>The first line contains a single integer $T$ ($1 \le T \le 10^4$) — the number of test cases.</p><p>Next $T$ lines contain test cases — one per line. Each line contains three integers $n$, $g$ and $b$ ($1 \le n, g, b \le 10^9$) — the length of the highway and the number of good and bad days respectively.</p></div><div class="output-specification"><p>Print $T$ integers — one per test case. For each test case, print the minimum number of days required to repair <span class="tex-font-style-bf">the whole highway if at least half of it should have high quality</span>.</p></div>

## Input

<p>The first line contains a single integer $T$ ($1 \le T \le 10^4$) — the number of test cases.</p><p>Next $T$ lines contain test cases — one per line. Each line contains three integers $n$, $g$ and $b$ ($1 \le n, g, b \le 10^9$) — the length of the highway and the number of good and bad days respectively.</p>

## Output

<p>Print $T$ integers — one per test case. For each test case, print the minimum number of days required to repair <span class="tex-font-style-bf">the whole highway if at least half of it should have high quality</span>.</p>





```input1
3
5 1 1
8 10 10
1000000 1 1000000
```




```output1
5
8
499999500000
```



## Note

<p>In the first test case, you can just lay new asphalt each day, since days $1, 3, 5$ are good.</p><p>In the second test case, you can also lay new asphalt each day, since days $1$-$8$ are good.</p>
