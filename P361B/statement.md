## Description

<div><p>Levko loves permutations very much. A permutation of length <span class="tex-span"><i>n</i></span> is a sequence of distinct positive integers, each is at most <span class="tex-span"><i>n</i></span>.</p><p>Let’s assume that value <span class="tex-span"><i>gcd</i>(<i>a</i>, <i>b</i>)</span> shows the greatest common divisor of numbers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. Levko assumes that element <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> of permutation <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ... , <i>p</i><sub class="lower-index"><i>n</i></sub></span> is good if <span class="tex-span"><i>gcd</i>(<i>i</i>, <i>p</i><sub class="lower-index"><i>i</i></sub>) &gt; 1</span>. Levko considers a permutation <span class="tex-font-style-it">beautiful</span>, if it has exactly <span class="tex-span"><i>k</i></span> good elements. Unfortunately, he doesn’t know any beautiful permutation. Your task is to help him to find at least one of them.</p></div><div class="input-specification"><p>The single line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ <i>n</i></span>).</p></div><div class="output-specification"><p>In a single line print either any beautiful permutation or -1, if such permutation doesn’t exist.</p><p>If there are multiple suitable permutations, you are allowed to print any of them.</p></div>

## Input

<p>The single line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ <i>n</i></span>).</p>

## Output

<p>In a single line print either any beautiful permutation or -1, if such permutation doesn’t exist.</p><p>If there are multiple suitable permutations, you are allowed to print any of them.</p>





```input1
4 2

```




```input2
1 1

```




```output1
2 4 3 1
```




```output2
-1

```



## Note

<p>In the first sample elements <span class="tex-span">4</span> and <span class="tex-span">3</span> are good because <span class="tex-span"><i>gcd</i>(2, 4) = 2 &gt; 1</span> and <span class="tex-span"><i>gcd</i>(3, 3) = 3 &gt; 1</span>. Elements <span class="tex-span">2</span> and <span class="tex-span">1</span> are not good because <span class="tex-span"><i>gcd</i>(1, 2) = 1</span> and <span class="tex-span"><i>gcd</i>(4, 1) = 1</span>. As there are exactly 2 good elements, the permutation is beautiful.</p><p>The second sample has no beautiful permutations.</p>
