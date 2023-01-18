## Description

<div><p>Paw the Spider is making a web. Web-making is a real art, Paw has been learning to do it his whole life. Let's consider the structure of the web.</p><center> <img class="tex-graphics" src="file://wQ1EiciM.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>There are <span class="tex-span"><i>n</i></span> <span class="tex-font-style-it">main</span> threads going from the center of the web. All main threads are located in one plane and divide it into <span class="tex-span"><i>n</i></span> equal infinite <span class="tex-font-style-it">sectors</span>. The sectors are indexed from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in the clockwise direction. Sectors <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>i</i> + 1</span> are <span class="tex-font-style-it">adjacent</span> for every <span class="tex-span"><i>i</i></span>, <span class="tex-span">1 ≤ <i>i</i> &lt; <i>n</i></span>. In addition, sectors <span class="tex-span">1</span> and <span class="tex-span"><i>n</i></span> are also adjacent.</p><p>Some sectors have <span class="tex-font-style-it">bridge threads</span>. Each bridge connects the two main threads that make up this sector. The points at which the bridge is attached to the main threads will be called <span class="tex-font-style-it">attachment points</span>. Both attachment points of a bridge are at the same distance from the center of the web. At each attachment point exactly one bridge is attached. The bridges are <span class="tex-font-style-it">adjacent</span> if they are in the same sector, and there are no other bridges between them.</p><p>A <span class="tex-font-style-it">cell</span> of the web is a trapezoid, which is located in one of the sectors and is bounded by two main threads and two adjacent bridges. You can see that the sides of the cell may have the attachment points of bridges from adjacent sectors. If the number of attachment points on one side of the cell is not equal to the number of attachment points on the other side, it creates an imbalance of pulling forces on this cell and this may eventually destroy the entire web. We'll call such a cell <span class="tex-font-style-it">unstable</span>. The perfect web does not contain unstable cells.</p><p>Unstable cells are marked red in the figure. Stable cells are marked green.</p><p>Paw the Spider isn't a skillful webmaker yet, he is only learning to make perfect webs. Help Paw to determine the number of unstable cells in the web he has just spun.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 1000</span>) — the number of main threads.</p><p>The <span class="tex-span"><i>i</i></span>-th of following <span class="tex-span"><i>n</i></span> lines describe the bridges located in the <span class="tex-span"><i>i</i></span>-th sector: first it contains integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) equal to the number of bridges in the given sector. Then follow <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> different integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>ij</i></sub> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>j</i> ≤ <i>k</i><sub class="lower-index"><i>i</i></sub></span>). Number <span class="tex-span"><i>p</i><sub class="lower-index"><i>ij</i></sub></span> equals the distance from the attachment points of the <span class="tex-span"><i>j</i></span>-th bridge of the <span class="tex-span"><i>i</i></span>-th sector to the center of the web.</p><p>It is guaranteed that any two bridges between adjacent sectors are attached at a different distance from the center of the web. It is guaranteed that the total number of the bridges doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p></div><div class="output-specification"><p>Print a single integer — the number of unstable cells in Paw the Spider's web.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 1000</span>) — the number of main threads.</p><p>The <span class="tex-span"><i>i</i></span>-th of following <span class="tex-span"><i>n</i></span> lines describe the bridges located in the <span class="tex-span"><i>i</i></span>-th sector: first it contains integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) equal to the number of bridges in the given sector. Then follow <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> different integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>ij</i></sub> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>j</i> ≤ <i>k</i><sub class="lower-index"><i>i</i></sub></span>). Number <span class="tex-span"><i>p</i><sub class="lower-index"><i>ij</i></sub></span> equals the distance from the attachment points of the <span class="tex-span"><i>j</i></span>-th bridge of the <span class="tex-span"><i>i</i></span>-th sector to the center of the web.</p><p>It is guaranteed that any two bridges between adjacent sectors are attached at a different distance from the center of the web. It is guaranteed that the total number of the bridges doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p>

## Output

<p>Print a single integer — the number of unstable cells in Paw the Spider's web.</p>





```input1
7
3 1 6 7
4 3 5 2 9
2 8 1
4 3 7 6 4
3 2 5 9
3 6 3 8
3 4 2 9

```




```output1
6
```


