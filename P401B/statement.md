## Description

<div><p>Sereja is a coder and he likes to take part in Codesorfes rounds. However, Uzhland doesn't have good internet connection, so Sereja sometimes skips rounds.</p><p>Codesorfes has rounds of two types: <span class="tex-span"><i>Div</i>1</span> (for advanced coders) and <span class="tex-span"><i>Div</i>2</span> (for beginner coders). Two rounds, <span class="tex-span"><i>Div</i>1</span> and <span class="tex-span"><i>Div</i>2</span>, can go simultaneously, (<span class="tex-span"><i>Div</i>1</span> round cannot be held without <span class="tex-span"><i>Div</i>2</span>) in all other cases the rounds don't overlap in time. Each round has a unique identifier — a positive integer. The rounds are sequentially (without gaps) numbered with identifiers by the starting time of the round. The identifiers of rounds that are run simultaneously are different by one, also the identifier of the <span class="tex-span"><i>Div</i>1</span> round is always greater.</p><p>Sereja is a beginner coder, so he can take part only in rounds of <span class="tex-span"><i>Div</i>2</span> type. At the moment he is taking part in a <span class="tex-span"><i>Div</i>2</span> round, its identifier equals to <span class="tex-span"><i>x</i></span>. Sereja remembers very well that he has taken part in exactly <span class="tex-span"><i>k</i></span> rounds before this round. Also, he remembers all identifiers of the rounds he has taken part in and all identifiers of the rounds that went simultaneously with them. Sereja doesn't remember anything about the rounds he missed.</p><p>Sereja is wondering: what minimum and what maximum number of <span class="tex-span"><i>Div</i>2</span> rounds could he have missed? Help him find these two numbers.</p></div><div class="input-specification"><p>The first line contains two integers: <span class="tex-span"><i>x</i></span> <span class="tex-span">(1 ≤ <i>x</i> ≤ 4000)</span> — the round Sereja is taking part in today, and <span class="tex-span"><i>k</i></span> <span class="tex-span">(0 ≤ <i>k</i> &lt; 4000)</span> — the number of rounds he took part in.</p><p>Next <span class="tex-span"><i>k</i></span> lines contain the descriptions of the rounds that Sereja took part in before. If Sereja took part in one of two simultaneous rounds, the corresponding line looks like: "1 <span class="tex-span"><i>num</i><sub class="lower-index">2</sub></span> <span class="tex-span"><i>num</i><sub class="lower-index">1</sub></span>" (where <span class="tex-span"><i>num</i><sub class="lower-index">2</sub></span> is the identifier of this <span class="tex-span"><i>Div</i>2</span> round, <span class="tex-span"><i>num</i><sub class="lower-index">1</sub></span> is the identifier of the <span class="tex-span"><i>Div</i>1</span> round). It is guaranteed that <span class="tex-span"><i>num</i><sub class="lower-index">1</sub> - <i>num</i><sub class="lower-index">2</sub> = 1</span>. If Sereja took part in a usual <span class="tex-span"><i>Div</i>2</span> round, then the corresponding line looks like: "2 <span class="tex-span"><i>num</i></span>" (where <span class="tex-span"><i>num</i></span> is the identifier of this <span class="tex-span"><i>Div</i>2</span> round). It is guaranteed that the identifiers of all given rounds are less than <span class="tex-span"><i>x</i></span>.</p></div><div class="output-specification"><p>Print in a single line two integers — the minimum and the maximum number of rounds that Sereja could have missed.</p></div>

## Input

<p>The first line contains two integers: <span class="tex-span"><i>x</i></span> <span class="tex-span">(1 ≤ <i>x</i> ≤ 4000)</span> — the round Sereja is taking part in today, and <span class="tex-span"><i>k</i></span> <span class="tex-span">(0 ≤ <i>k</i> &lt; 4000)</span> — the number of rounds he took part in.</p><p>Next <span class="tex-span"><i>k</i></span> lines contain the descriptions of the rounds that Sereja took part in before. If Sereja took part in one of two simultaneous rounds, the corresponding line looks like: "1 <span class="tex-span"><i>num</i><sub class="lower-index">2</sub></span> <span class="tex-span"><i>num</i><sub class="lower-index">1</sub></span>" (where <span class="tex-span"><i>num</i><sub class="lower-index">2</sub></span> is the identifier of this <span class="tex-span"><i>Div</i>2</span> round, <span class="tex-span"><i>num</i><sub class="lower-index">1</sub></span> is the identifier of the <span class="tex-span"><i>Div</i>1</span> round). It is guaranteed that <span class="tex-span"><i>num</i><sub class="lower-index">1</sub> - <i>num</i><sub class="lower-index">2</sub> = 1</span>. If Sereja took part in a usual <span class="tex-span"><i>Div</i>2</span> round, then the corresponding line looks like: "2 <span class="tex-span"><i>num</i></span>" (where <span class="tex-span"><i>num</i></span> is the identifier of this <span class="tex-span"><i>Div</i>2</span> round). It is guaranteed that the identifiers of all given rounds are less than <span class="tex-span"><i>x</i></span>.</p>

## Output

<p>Print in a single line two integers — the minimum and the maximum number of rounds that Sereja could have missed.</p>





```input1
3 2
2 1
2 2

```




```input2
9 3
1 2 3
2 8
1 4 5

```




```input3
10 0

```




```output1
0 0
```




```output2
2 3
```




```output3
5 9
```



## Note

<p>In the second sample we have unused identifiers of rounds 1, 6, 7. The minimum number of rounds Sereja could have missed equals to 2. In this case, the round with the identifier 1 will be a usual <span class="tex-span"><i>Div</i>2</span> round and the round with identifier <span class="tex-span">6</span> will be synchronous with the <span class="tex-span"><i>Div</i>1</span> round. </p><p>The maximum number of rounds equals <span class="tex-span">3</span>. In this case all unused identifiers belong to usual <span class="tex-span"><i>Div</i>2</span> rounds.</p>
