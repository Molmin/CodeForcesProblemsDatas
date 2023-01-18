## Description

<div><p>In some game by Playrix it takes <span class="tex-span"><i>t</i></span> minutes for an oven to bake <span class="tex-span"><i>k</i></span> carrot cakes, all cakes are ready at the same moment <span class="tex-span"><i>t</i></span> minutes after they started baking. Arkady needs at least <span class="tex-span"><i>n</i></span> cakes to complete a task, but he currently don't have any. However, he has infinitely many ingredients and one oven. Moreover, Arkady can build one more similar oven to make the process faster, it would take <span class="tex-span"><i>d</i></span> minutes to build the oven. While the new oven is being built, only old one can bake cakes, after the new oven is built, both ovens bake simultaneously. Arkady can't build more than one oven.</p><p>Determine if it is reasonable to build the second oven, i.e. will it decrease the minimum time needed to get <span class="tex-span"><i>n</i></span> cakes or not. If the time needed with the second oven is the same as with one oven, then it is unreasonable.</p></div><div class="input-specification"><p>The only line contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>t</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>t</i>, <i>k</i>, <i>d</i> ≤ 1 000</span>)&nbsp;— the number of cakes needed, the time needed for one oven to bake <span class="tex-span"><i>k</i></span> cakes, the number of cakes baked at the same time, the time needed to build the second oven. </p></div><div class="output-specification"><p>If it is reasonable to build the second oven, print "<span class="tex-font-style-tt">YES</span>". Otherwise print "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>The only line contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>t</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>t</i>, <i>k</i>, <i>d</i> ≤ 1 000</span>)&nbsp;— the number of cakes needed, the time needed for one oven to bake <span class="tex-span"><i>k</i></span> cakes, the number of cakes baked at the same time, the time needed to build the second oven. </p>

## Output

<p>If it is reasonable to build the second oven, print "<span class="tex-font-style-tt">YES</span>". Otherwise print "<span class="tex-font-style-tt">NO</span>".</p>





```input1
8 6 4 5

```




```input2
8 6 4 6

```




```input3
10 3 11 4

```




```input4
4 2 1 4

```




```output1
YES

```




```output2
NO

```




```output3
NO

```




```output4
YES

```



## Note

<p>In the first example it is possible to get <span class="tex-span">8</span> cakes in <span class="tex-span">12</span> minutes using one oven. The second oven can be built in <span class="tex-span">5</span> minutes, so after <span class="tex-span">6</span> minutes the first oven bakes <span class="tex-span">4</span> cakes, the second oven bakes <span class="tex-span">4</span> more ovens after <span class="tex-span">11</span> minutes. Thus, it is reasonable to build the second oven. </p><p>In the second example it doesn't matter whether we build the second oven or not, thus it takes <span class="tex-span">12</span> minutes to bake <span class="tex-span">8</span> cakes in both cases. Thus, it is unreasonable to build the second oven.</p><p>In the third example the first oven bakes <span class="tex-span">11</span> cakes in <span class="tex-span">3</span> minutes, that is more than needed <span class="tex-span">10</span>. It is unreasonable to build the second oven, because its building takes more time that baking the needed number of cakes using the only oven.</p>
