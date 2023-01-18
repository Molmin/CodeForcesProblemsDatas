## Description

<div><p>Volodya has recently visited a very odd town. There are <span class="tex-span"><i>N</i></span> tourist attractions in the town and every two of them are connected by a bidirectional road. Each road has some travel price (natural number) assigned to it and all prices are distinct. But the most striking thing about this town is that each city sightseeing tour has the same total price! That is, if we choose any city sightseeing tour — a cycle which visits every attraction exactly once — the sum of the costs of the tour roads is independent of the tour. Volodya is curious if you can find such price system with all road prices not greater than 1000.</p></div><div class="input-specification"><p>Input contains just one natural number (<span class="tex-span">3 ≤ <i>N</i> ≤ 20</span>) — the number of town attractions.</p></div><div class="output-specification"><p>Output should contain <span class="tex-span"><i>N</i></span> rows containing <span class="tex-span"><i>N</i></span> positive integer numbers each — the adjacency matrix of the prices graph (thus, <span class="tex-span"><i>j</i></span>-th number in <span class="tex-span"><i>i</i></span>-th row should be equal to the price of the road between the <span class="tex-span"><i>j</i></span>-th and the <span class="tex-span"><i>i</i></span>-th attraction). Diagonal numbers should be equal to zero. All numbers should not be greater than 1000. All prices should be positive and pairwise distinct. If there are several solutions, output any of them.</p></div>

## Input

<p>Input contains just one natural number (<span class="tex-span">3 ≤ <i>N</i> ≤ 20</span>) — the number of town attractions.</p>

## Output

<p>Output should contain <span class="tex-span"><i>N</i></span> rows containing <span class="tex-span"><i>N</i></span> positive integer numbers each — the adjacency matrix of the prices graph (thus, <span class="tex-span"><i>j</i></span>-th number in <span class="tex-span"><i>i</i></span>-th row should be equal to the price of the road between the <span class="tex-span"><i>j</i></span>-th and the <span class="tex-span"><i>i</i></span>-th attraction). Diagonal numbers should be equal to zero. All numbers should not be greater than 1000. All prices should be positive and pairwise distinct. If there are several solutions, output any of them.</p>





```input1
3

```




```output1
0 3 4 
3 0 5 
4 5 0 

```


