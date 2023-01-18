## Description

<div><p>Digital collectible card games have become very popular recently. So Vova decided to try one of these.</p><p>Vova has <span class="tex-span"><i>n</i></span> cards in his collection. Each of these cards is characterised by its power <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, magic number <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and level <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>. Vova wants to build a deck with total power not less than <span class="tex-span"><i>k</i></span>, but magic numbers may not allow him to do so — Vova can't place two cards in a deck if the sum of the magic numbers written on these cards is a prime number. Also Vova cannot use a card if its level is greater than the level of Vova's character.</p><p>At the moment Vova's character's level is <span class="tex-span">1</span>. Help Vova to determine the minimum level he needs to reach in order to build a deck with the required total power.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 100000</span>).</p><p>Then <span class="tex-span"><i>n</i></span> lines follow, each of these lines contains three numbers that represent the corresponding card: <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 100000</span>, <span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p></div><div class="output-specification"><p>If Vova won't be able to build a deck with required power, print <span class="tex-span"> - 1</span>. Otherwise print the minimum level Vova has to reach in order to build a deck.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 100000</span>).</p><p>Then <span class="tex-span"><i>n</i></span> lines follow, each of these lines contains three numbers that represent the corresponding card: <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 100000</span>, <span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p>

## Output

<p>If Vova won't be able to build a deck with required power, print <span class="tex-span"> - 1</span>. Otherwise print the minimum level Vova has to reach in order to build a deck.</p>





```input1
5 8
5 5 1
1 5 4
4 6 3
1 12 4
3 12 1

```




```input2
3 7
4 4 1
5 8 2
5 3 3

```




```output1
4

```




```output2
2

```


