## Description

<div><p>During her tantrums the princess usually smashes some collectable porcelain. Every furious shriek is accompanied with one item smashed.</p><p>The collection of porcelain is arranged neatly on <span class="tex-span"><i>n</i></span> shelves. Within each shelf the items are placed in one row, so that one can access only the outermost items — the leftmost or the rightmost item, not the ones in the middle of the shelf. Once an item is taken, the next item on that side of the shelf can be accessed (see example). Once an item is taken, it can't be returned to the shelves.</p><p>You are given the values of all items. Your task is to find the maximal damage the princess' tantrum of <span class="tex-span"><i>m</i></span> shrieks can inflict on the collection of porcelain.</p></div><div class="input-specification"><p>The first line of input data contains two integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10000</span>). The next <span class="tex-span"><i>n</i></span> lines contain the values of the items on the shelves: the first number gives the number of items on this shelf (an integer between <span class="tex-span">1</span> and <span class="tex-span">100</span>, inclusive), followed by the values of the items (integers between <span class="tex-span">1</span> and <span class="tex-span">100</span>, inclusive), in the order in which they appear on the shelf (the first number corresponds to the leftmost item, the last one — to the rightmost one). The total number of items is guaranteed to be at least <span class="tex-span"><i>m</i></span>.</p></div><div class="output-specification"><p>Output the maximal total value of a tantrum of <span class="tex-span"><i>m</i></span> shrieks.</p></div>

## Input

<p>The first line of input data contains two integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10000</span>). The next <span class="tex-span"><i>n</i></span> lines contain the values of the items on the shelves: the first number gives the number of items on this shelf (an integer between <span class="tex-span">1</span> and <span class="tex-span">100</span>, inclusive), followed by the values of the items (integers between <span class="tex-span">1</span> and <span class="tex-span">100</span>, inclusive), in the order in which they appear on the shelf (the first number corresponds to the leftmost item, the last one — to the rightmost one). The total number of items is guaranteed to be at least <span class="tex-span"><i>m</i></span>.</p>

## Output

<p>Output the maximal total value of a tantrum of <span class="tex-span"><i>m</i></span> shrieks.</p>





```input1
2 3
3 3 7 2
3 4 1 5

```




```input2
1 3
4 4 3 1 2

```




```output1
15

```




```output2
9

```



## Note

<p>In the first case there are two shelves, each with three items. To maximize the total value of the items chosen, one can take two items from the left side of the first shelf and one item from the right side of the second shelf.</p><p>In the second case there is only one shelf, so all three items are taken from it — two from the left side and one from the right side.</p>
