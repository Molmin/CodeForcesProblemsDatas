## Description

<div><p>Little beaver is a beginner programmer, so informatics is his favorite subject. Soon his informatics teacher is going to have a birthday and the beaver has decided to prepare a present for her. He planted <span class="tex-span"><i>n</i></span> flowers in a row on his windowsill and started waiting for them to grow. However, after some time the beaver noticed that the flowers stopped growing. The beaver thinks it is bad manners to present little flowers. So he decided to come up with some solutions. </p><p>There are <span class="tex-span"><i>m</i></span> days left to the birthday. The height of the <span class="tex-span"><i>i</i></span>-th flower (assume that the flowers in the row are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from left to right) is equal to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> at the moment. At each of the remaining <span class="tex-span"><i>m</i></span> days the beaver can take a special watering and water <span class="tex-span"><i>w</i></span> contiguous flowers (he can do that only once at a day). At that each watered flower grows by one height unit on that day. The beaver wants the height of the smallest flower be as large as possible in the end. What maximum height of the smallest flower can he get?</p></div><div class="input-specification"><p>The first line contains space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>w</i></span> <span class="tex-span">(1 ≤ <i>w</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p></div><div class="output-specification"><p>Print a single integer — the maximum final height of the smallest flower.</p></div>

## Input

<p>The first line contains space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>w</i></span> <span class="tex-span">(1 ≤ <i>w</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p>

## Output

<p>Print a single integer — the maximum final height of the smallest flower.</p>





```input1
6 2 3
2 2 2 2 1 1

```




```input2
2 5 1
5 8

```




```output1
2

```




```output2
9

```



## Note

<p>In the first sample beaver can water the last 3 flowers at the first day. On the next day he may not to water flowers at all. In the end he will get the following heights: [2, 2, 2, 3, 2, 2]. The smallest flower has height equal to 2. It's impossible to get height 3 in this test.</p>
