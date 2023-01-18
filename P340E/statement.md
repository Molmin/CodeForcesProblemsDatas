## Description

<div><p>Iahub is so happy about inventing bubble sort graphs that he's staying all day long at the office and writing permutations. Iahubina is angry that she is no more important for Iahub. When Iahub goes away, Iahubina comes to his office and sabotage his research work.</p><p>The girl finds an important permutation for the research. The permutation contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>. She replaces some of permutation elements with -1 value as a revenge. </p><p>When Iahub finds out his important permutation is broken, he tries to recover it. The only thing he remembers about the permutation is it didn't have any fixed point. A fixed point for a permutation is an element <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub></span> which has value equal to <span class="tex-span"><i>k</i></span> <span class="tex-span">(<i>a</i><sub class="lower-index"><i>k</i></sub> = <i>k</i>)</span>. Your job is to proof to Iahub that trying to recover it is not a good idea. Output the number of permutations which could be originally Iahub's important permutation, modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2000</span>). On the second line, there are <span class="tex-span"><i>n</i></span> integers, representing Iahub's important permutation after Iahubina replaces some values with -1. </p><p>It's guaranteed that there are no fixed points in the given permutation. Also, the given sequence contains at least two numbers -1 and each positive number occurs in the sequence at most once. It's guaranteed that there is at least one suitable permutation.</p></div><div class="output-specification"><p>Output a single integer, the number of ways Iahub could recover his permutation, modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2000</span>). On the second line, there are <span class="tex-span"><i>n</i></span> integers, representing Iahub's important permutation after Iahubina replaces some values with -1. </p><p>It's guaranteed that there are no fixed points in the given permutation. Also, the given sequence contains at least two numbers -1 and each positive number occurs in the sequence at most once. It's guaranteed that there is at least one suitable permutation.</p>

## Output

<p>Output a single integer, the number of ways Iahub could recover his permutation, modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p>





```input1
5
-1 -1 4 3 -1

```




```output1
2

```



## Note

<p>For the first test example there are two permutations with no fixed points are [2, 5, 4, 3, 1] and [5, 1, 4, 3, 2]. Any other permutation would have at least one fixed point. </p>
