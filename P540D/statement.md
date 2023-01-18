## Description

<div><p>The Bad Luck Island is inhabited by three kinds of species: <span class="tex-span"><i>r</i></span> rocks, <span class="tex-span"><i>s</i></span> scissors and <span class="tex-span"><i>p</i></span> papers. At some moments of time two random individuals meet (all pairs of individuals can meet equiprobably), and if they belong to different species, then one individual kills the other one: a rock kills scissors, scissors kill paper, and paper kills a rock. Your task is to determine for each species what is the probability that this species will be the only one to inhabit this island after a long enough period of time.</p></div><div class="input-specification"><p>The single line contains three integers <span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>r</i>, <i>s</i>, <i>p</i> ≤ 100</span>)&nbsp;— the original number of individuals in the species of rock, scissors and paper, respectively.</p></div><div class="output-specification"><p>Print three space-separated real numbers: the probabilities, at which the rocks, the scissors and the paper will be the only surviving species, respectively. The answer will be considered correct if the relative or absolute error of each number doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p></div>

## Input

<p>The single line contains three integers <span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>r</i>, <i>s</i>, <i>p</i> ≤ 100</span>)&nbsp;— the original number of individuals in the species of rock, scissors and paper, respectively.</p>

## Output

<p>Print three space-separated real numbers: the probabilities, at which the rocks, the scissors and the paper will be the only surviving species, respectively. The answer will be considered correct if the relative or absolute error of each number doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p>





```input1
2 2 2

```




```input2
2 1 2

```




```input3
1 1 3

```




```output1
0.333333333333 0.333333333333 0.333333333333

```




```output2
0.150000000000 0.300000000000 0.550000000000

```




```output3
0.057142857143 0.657142857143 0.285714285714

```


