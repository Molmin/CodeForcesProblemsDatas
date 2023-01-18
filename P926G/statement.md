## Description

<div><p>A flower shop has got <span class="tex-span"><i>n</i></span> bouquets, and the <span class="tex-span"><i>i</i></span>-th bouquet consists of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> flowers. Vasya, the manager of the shop, decided to make large bouquets from these bouquets. </p><p>Vasya thinks that a bouquet is large if it is made of <span class="tex-font-style-bf">two or more</span> initial bouquets, and there is a constraint: the total number of flowers in a large bouquet should be <span class="tex-font-style-bf">odd</span>. Each of the initial bouquets can be a part of at most one large bouquet. If an initial bouquet becomes a part of a large bouquet, all its flowers are included in the large bouquet.</p><p>Determine the maximum possible number of large bouquets Vasya can make. </p></div><div class="input-specification"><p>The first line contains a single positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of initial bouquets.</p><p>The second line contains a sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the number of flowers in each of the initial bouquets.</p></div><div class="output-specification"><p>Print the maximum number of large bouquets Vasya can make. </p></div>

## Input

<p>The first line contains a single positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of initial bouquets.</p><p>The second line contains a sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the number of flowers in each of the initial bouquets.</p>

## Output

<p>Print the maximum number of large bouquets Vasya can make. </p>





```input1
5
2 3 4 2 7

```




```input2
6
2 2 6 8 6 12

```




```input3
3
11 4 10

```




```output1
2

```




```output2
0

```




```output3
1

```



## Note

<p>In the first example Vasya can make <span class="tex-span">2</span> large bouquets. For example, the first bouquet can contain the first and the fifth initial bouquets (the total number of flowers is then equal to <span class="tex-span">9</span>), and the second bouquet can consist of the second and the third initial bouquets (the total number of flowers is then equal to <span class="tex-span">7</span>). The fourth initial bouquet is unused in this scheme. </p><p>In the second example it is not possible to form a single bouquet with odd number of flowers.</p><p>In the third example Vasya can make one large bouquet. For example, he can make it using all three initial bouquets. The size of the large bouquet is then equal to <span class="tex-span">11 + 4 + 10 = 25</span>.</p>
