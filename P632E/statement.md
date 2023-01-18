## Description

<div><p>A thief made his way to a shop.</p><p>As usual he has his lucky knapsack with him. The knapsack can contain <span class="tex-span"><i>k</i></span> objects. There are <span class="tex-span"><i>n</i></span> kinds of products in the shop and an infinite number of products of each kind. The cost of one product of kind <span class="tex-span"><i>i</i></span> is <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>The thief is greedy, so he will take exactly <span class="tex-span"><i>k</i></span> products (it's possible for some kinds to take several products of that kind).</p><p>Find all the possible total costs of products the thief can nick into his knapsack.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 1000</span>) — the number of kinds of products and the number of products the thief will take.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — the costs of products for kinds from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p></div><div class="output-specification"><p>Print the only line with all the possible total costs of stolen products, separated by a space. The numbers should be printed in the ascending order.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 1000</span>) — the number of kinds of products and the number of products the thief will take.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — the costs of products for kinds from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p>

## Output

<p>Print the only line with all the possible total costs of stolen products, separated by a space. The numbers should be printed in the ascending order.</p>





```input1
3 2
1 2 3

```




```input2
5 5
1 1 1 1 1

```




```input3
3 3
3 5 11

```




```output1
2 3 4 5 6

```




```output2
5

```




```output3
9 11 13 15 17 19 21 25 27 33

```


