## Description

<div><p>There are <span class="tex-span"><i>n</i></span> cities situated along the main road of Berland. Cities are represented by their coordinates — integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. All coordinates are pairwise distinct.</p><p>It is possible to get from one city to another only by bus. But all buses and roads are very old, so the Minister of Transport decided to build a new bus route. The Minister doesn't want to spend large amounts of money — he wants to choose two cities in such a way that the distance between them is minimal possible. The distance between two cities is equal to the absolute value of the difference between their coordinates.</p><p>It is possible that there are multiple pairs of cities with minimal possible distance, so the Minister wants to know the quantity of such pairs. </p><p>Your task is to write a program that will calculate the minimal possible distance between two pairs of cities and the quantity of pairs which have this distance.</p></div><div class="input-specification"><p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). All numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are pairwise distinct.</p></div><div class="output-specification"><p>Print two integer numbers — the minimal distance and the quantity of pairs with this distance.</p></div>

## Input

<p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). All numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are pairwise distinct.</p>

## Output

<p>Print two integer numbers — the minimal distance and the quantity of pairs with this distance.</p>





```input1
4
6 -3 0 4

```




```input2
3
-2 0 2

```




```output1
2 1

```




```output2
2 2

```



## Note

<p>In the first example the distance between the first city and the fourth city is <span class="tex-span">|4 - 6| = 2</span>, and it is the only pair with this distance.</p>
