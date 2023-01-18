## Description

<div><p>Mad scientist Mike entertains himself by arranging rows of dominoes. He doesn't need dominoes, though: he uses rectangular magnets instead. Each magnet has two poles, positive (a "plus") and negative (a "minus"). If two magnets are put together at a close distance, then the like poles will repel each other and the opposite poles will attract each other.</p><p>Mike starts by laying one magnet horizontally on the table. During each following step Mike adds one more magnet horizontally to the right end of the row. Depending on how Mike puts the magnet on the table, it is either attracted to the previous one (forming a group of multiple magnets linked together) or repelled by it (then Mike lays this magnet at some distance to the right from the previous one). We assume that a sole magnet not linked to others forms a group of its own.</p><center> <img class="tex-graphics" src="file://avwlZ8qB.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Mike arranged multiple magnets in a row. Determine the number of groups that the magnets formed.</p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100000</span>) — the number of magnets. Then <span class="tex-span"><i>n</i></span> lines follow. The <span class="tex-span"><i>i</i></span>-th line (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) contains either characters "<span class="tex-font-style-tt">01</span>", if Mike put the <span class="tex-span"><i>i</i></span>-th magnet in the "plus-minus" position, or characters "<span class="tex-font-style-tt">10</span>", if Mike put the magnet in the "minus-plus" position.</p></div><div class="output-specification"><p>On the single line of the output print the number of groups of magnets.</p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100000</span>) — the number of magnets. Then <span class="tex-span"><i>n</i></span> lines follow. The <span class="tex-span"><i>i</i></span>-th line (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) contains either characters "<span class="tex-font-style-tt">01</span>", if Mike put the <span class="tex-span"><i>i</i></span>-th magnet in the "plus-minus" position, or characters "<span class="tex-font-style-tt">10</span>", if Mike put the magnet in the "minus-plus" position.</p>

## Output

<p>On the single line of the output print the number of groups of magnets.</p>





```input1
6
10
10
10
01
10
10

```




```input2
4
01
01
10
10

```




```output1
3

```




```output2
2

```



## Note

<p>The first testcase corresponds to the figure. The testcase has three groups consisting of three, one and two magnets.</p><p>The second testcase has two groups, each consisting of two magnets.</p>
