## Description

<div><p><span class="tex-span"><i>n</i></span> fish, numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, live in a lake. Every day right one pair of fish meet, and the probability of each other pair meeting is the same. If two fish with indexes i and j meet, the first will eat up the second with the probability <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span>, and the second will eat up the first with the probability <span class="tex-span"><i>a</i><sub class="lower-index"><i>ji</i></sub> = 1 - <i>a</i><sub class="lower-index"><i>ij</i></sub></span>. The described process goes on until there are at least two fish in the lake. For each fish find out the probability that it will survive to be the last in the lake.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 18</span>) — the amount of fish in the lake. Then there follow <span class="tex-span"><i>n</i></span> lines with <span class="tex-span"><i>n</i></span> real numbers each — matrix <span class="tex-span"><i>a</i></span>. <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 1</span>) — the probability that fish with index <span class="tex-span"><i>i</i></span> eats up fish with index <span class="tex-span"><i>j</i></span>. It's guaranteed that the main diagonal contains zeros only, and for other elements the following is true: <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub> = 1 - <i>a</i><sub class="lower-index"><i>ji</i></sub></span>. All real numbers are given with not more than 6 characters after the decimal point.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>n</i></span> space-separated real numbers accurate to not less than 6 decimal places. Number with index <span class="tex-span"><i>i</i></span> should be equal to the probability that fish with index <span class="tex-span"><i>i</i></span> will survive to be the last in the lake.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 18</span>) — the amount of fish in the lake. Then there follow <span class="tex-span"><i>n</i></span> lines with <span class="tex-span"><i>n</i></span> real numbers each — matrix <span class="tex-span"><i>a</i></span>. <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 1</span>) — the probability that fish with index <span class="tex-span"><i>i</i></span> eats up fish with index <span class="tex-span"><i>j</i></span>. It's guaranteed that the main diagonal contains zeros only, and for other elements the following is true: <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub> = 1 - <i>a</i><sub class="lower-index"><i>ji</i></sub></span>. All real numbers are given with not more than 6 characters after the decimal point.</p>

## Output

<p>Output <span class="tex-span"><i>n</i></span> space-separated real numbers accurate to not less than 6 decimal places. Number with index <span class="tex-span"><i>i</i></span> should be equal to the probability that fish with index <span class="tex-span"><i>i</i></span> will survive to be the last in the lake.</p>





```input1
2
0 0.5
0.5 0

```




```input2
5
0 1 1 1 1
0 0 0.5 0.5 0.5
0 0.5 0 0.5 0.5
0 0.5 0.5 0 0.5
0 0.5 0.5 0.5 0

```




```output1
0.500000 0.500000
```




```output2
1.000000 0.000000 0.000000 0.000000 0.000000
```


