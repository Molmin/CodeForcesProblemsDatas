## Description

<div><p>In Berland the opposition is going to arrange mass walking on the boulevard. The boulevard consists of <span class="tex-span"><i>n</i></span> tiles that are lain in a row and are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from right to left. The opposition should start walking on the tile number <span class="tex-span">1</span> and the finish on the tile number <span class="tex-span"><i>n</i></span>. During the walk it is allowed to move from right to left between adjacent tiles in a row, and jump over a tile. More formally, if you are standing on the tile number <span class="tex-span"><i>i</i></span> <span class="tex-span">(<i>i</i> &lt; <i>n</i> - 1)</span>, you can reach the tiles number <span class="tex-span"><i>i</i> + 1</span> or the tile number <span class="tex-span"><i>i</i> + 2</span> from it (if you stand on the tile number <span class="tex-span"><i>n</i> - 1</span>, you can only reach tile number <span class="tex-span"><i>n</i></span>). We can assume that all the opposition movements occur instantaneously.</p><p>In order to thwart an opposition rally, the Berland bloody regime organized the rain. The tiles on the boulevard are of poor quality and they are rapidly destroyed in the rain. We know that the <span class="tex-span"><i>i</i></span>-th tile is destroyed after <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> days of rain (on day <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> tile isn't destroyed yet, and on day <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> + 1</span> it is already destroyed). Of course, no one is allowed to walk on the destroyed tiles! So the walk of the opposition is considered thwarted, if either the tile number <span class="tex-span">1</span> is broken, or the tile number <span class="tex-span"><i>n</i></span> is broken, or it is impossible to reach the tile number <span class="tex-span"><i>n</i></span> from the tile number <span class="tex-span">1</span> if we can walk on undestroyed tiles.</p><p>The opposition wants to gather more supporters for their walk. Therefore, the more time they have to pack, the better. Help the opposition to calculate how much time they still have and tell us for how many days the walk from the tile number <span class="tex-span">1</span> to the tile number <span class="tex-span"><i>n</i></span> will be possible.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup></span>) — the boulevard's length in tiles.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> — the number of days after which the <span class="tex-span"><i>i</i></span>-th tile gets destroyed (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">3</sup></span>). </p></div><div class="output-specification"><p>Print a single number — the sought number of days.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup></span>) — the boulevard's length in tiles.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> — the number of days after which the <span class="tex-span"><i>i</i></span>-th tile gets destroyed (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">3</sup></span>). </p>

## Output

<p>Print a single number — the sought number of days.</p>





```input1
4
10 3 5 10

```




```input2
5
10 2 8 3 5

```




```output1
5

```




```output2
5

```



## Note

<p>In the first sample the second tile gets destroyed after day three, and the only path left is <span class="tex-span">1 → 3 → 4</span>. After day five there is a two-tile gap between the first and the last tile, you can't jump over it.</p><p>In the second sample path <span class="tex-span">1 → 3 → 5</span> is available up to day five, inclusive. On day six the last tile is destroyed and the walk is thwarted.</p>
