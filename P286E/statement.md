## Description

<div><p>A ladies' shop has recently opened in the city of Ultima Thule. To get ready for the opening, the shop bought <span class="tex-span"><i>n</i></span> bags. Each bag is characterised by the total weight <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> of the items you can put there. The weird thing is, you <span class="tex-font-style-bf">cannot</span> use these bags to put a set of items with the total weight strictly less than <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. However the weights of the items that will be sold in the shop haven't yet been defined. That's what you should determine right now.</p><p>Your task is to find the set of the items' weights <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index">1</sub> &lt; <i>p</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>p</i><sub class="lower-index"><i>k</i></sub>)</span>, such that:</p><ol> <li> Any bag will be used. That is, for any <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i>)</span> there will be such set of items that their total weight will equal <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. We assume that there is the infinite number of items of any weight. You can put multiple items of the same weight in one bag. </li><li> For any set of items that have total weight less than or equal to <span class="tex-span"><i>m</i></span>, there is a bag into which you can put this set. Similarly, a set of items can contain multiple items of the same weight. </li><li> Of all sets of the items' weights that satisfy points 1 and 2, find the set with the minimum number of weights. In other words, value <span class="tex-span"><i>k</i></span> should be as small as possible. </li></ol><p>Find and print the required set.</p></div><div class="input-specification"><p>The first line contains space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> distinct space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index">1</sub> &lt; <i>a</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>a</i><sub class="lower-index"><i>n</i></sub> ≤ <i>m</i></span>) — the bags' weight limits.</p></div><div class="output-specification"><p>In the first line print "<span class="tex-font-style-tt">NO</span>" (without the quotes) if there isn't set <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, that would meet the conditions.</p><p>Otherwise, in the first line print "<span class="tex-font-style-tt">YES</span>" (without the quotes), in the second line print an integer <span class="tex-span"><i>k</i></span> (showing how many numbers are in the suitable set with the minimum number of weights), in the third line print <span class="tex-span"><i>k</i></span> space-separated integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index">1</sub> &lt; <i>p</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>p</i><sub class="lower-index"><i>k</i></sub>)</span>. If there are multiple solutions, print any of them.</p></div>

## Input

<p>The first line contains space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> distinct space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index">1</sub> &lt; <i>a</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>a</i><sub class="lower-index"><i>n</i></sub> ≤ <i>m</i></span>) — the bags' weight limits.</p>

## Output

<p>In the first line print "<span class="tex-font-style-tt">NO</span>" (without the quotes) if there isn't set <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, that would meet the conditions.</p><p>Otherwise, in the first line print "<span class="tex-font-style-tt">YES</span>" (without the quotes), in the second line print an integer <span class="tex-span"><i>k</i></span> (showing how many numbers are in the suitable set with the minimum number of weights), in the third line print <span class="tex-span"><i>k</i></span> space-separated integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index">1</sub> &lt; <i>p</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>p</i><sub class="lower-index"><i>k</i></sub>)</span>. If there are multiple solutions, print any of them.</p>





```input1
6 10
5 6 7 8 9 10

```




```input2
1 10
1

```




```input3
1 10
6

```




```output1
YES
5
5 6 7 8 9 

```




```output2
NO

```




```output3
YES
1
6 

```


