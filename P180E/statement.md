## Description

<div><p>Let's imagine that you're playing the following simple computer game. The screen displays <span class="tex-span"><i>n</i></span> lined-up cubes. Each cube is painted one of <span class="tex-span"><i>m</i></span> colors. You are allowed to delete not more than <span class="tex-span"><i>k</i></span> cubes (that do not necessarily go one after another). After that, the remaining cubes join together (so that the gaps are closed) and the system counts the score. The number of points you score equals to the length of the maximum sequence of cubes of the same color that follow consecutively. Write a program that determines the maximum possible number of points you can score.</p><p>Remember, you may delete no more than <span class="tex-span"><i>k</i></span> any cubes. It is allowed not to delete cubes at all.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup>, 1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>k</i> &lt; <i>n</i></span>). The second line contains <span class="tex-span"><i>n</i></span> integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> — the numbers of cube colors. The numbers of colors are separated by single spaces.</p></div><div class="output-specification"><p>Print the maximum possible number of points you can score.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup>, 1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>k</i> &lt; <i>n</i></span>). The second line contains <span class="tex-span"><i>n</i></span> integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> — the numbers of cube colors. The numbers of colors are separated by single spaces.</p>

## Output

<p>Print the maximum possible number of points you can score.</p>





```input1
10 3 2
1 2 1 1 3 2 1 1 2 2

```




```input2
10 2 2
1 2 1 2 1 1 2 1 1 2

```




```input3
3 1 2
1 1 1

```




```output1
4

```




```output2
5

```




```output3
3

```



## Note

<p>In the first sample you should delete the fifth and the sixth cubes.</p><p>In the second sample you should delete the fourth and the seventh cubes.</p><p>In the third sample you shouldn't delete any cubes.</p>
