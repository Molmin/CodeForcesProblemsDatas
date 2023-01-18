## Description

<div><p>The map of Berland is a rectangle of the size <span class="tex-span"><i>n</i> × <i>m</i></span>, which consists of cells of size <span class="tex-span">1 × 1</span>. Each cell is either land or water. The map is surrounded by the ocean. </p><p><span class="tex-font-style-it">Lakes</span> are the maximal regions of water cells, connected by sides, which are not connected with the ocean. Formally, lake is a set of water cells, such that it's possible to get from any cell of the set to any other without leaving the set and moving only to cells adjacent by the side, none of them is located on the border of the rectangle, and it's impossible to add one more water cell to the set such that it will be connected with any other cell.</p><p>You task is to fill up with the earth the minimum number of water cells so that there will be <span class="tex-font-style-bf">exactly</span> <span class="tex-span"><i>k</i></span> lakes in Berland. Note that the initial number of lakes on the map is <span class="tex-font-style-bf">not less</span> than <span class="tex-span"><i>k</i></span>. </p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 50</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 50</span>)&nbsp;— the sizes of the map and the number of lakes which should be left on the map.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> characters each — the description of the map. Each of the characters is either '<span class="tex-font-style-tt">.</span>' (it means that the corresponding cell is water) or '<span class="tex-font-style-tt">*</span>' (it means that the corresponding cell is land).</p><p>It is guaranteed that the map contain at least <span class="tex-span"><i>k</i></span> lakes.</p></div><div class="output-specification"><p>In the first line print the minimum number of cells which should be transformed from water to land. </p><p>In the next <span class="tex-span"><i>n</i></span> lines print <span class="tex-span"><i>m</i></span> symbols — the map after the changes. The format must strictly follow the format of the map in the input data (there is no need to print the size of the map). If there are several answers, print any of them. </p><p>It is guaranteed that the answer exists on the given data.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 50</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 50</span>)&nbsp;— the sizes of the map and the number of lakes which should be left on the map.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> characters each — the description of the map. Each of the characters is either '<span class="tex-font-style-tt">.</span>' (it means that the corresponding cell is water) or '<span class="tex-font-style-tt">*</span>' (it means that the corresponding cell is land).</p><p>It is guaranteed that the map contain at least <span class="tex-span"><i>k</i></span> lakes.</p>

## Output

<p>In the first line print the minimum number of cells which should be transformed from water to land. </p><p>In the next <span class="tex-span"><i>n</i></span> lines print <span class="tex-span"><i>m</i></span> symbols — the map after the changes. The format must strictly follow the format of the map in the input data (there is no need to print the size of the map). If there are several answers, print any of them. </p><p>It is guaranteed that the answer exists on the given data.</p>





```input1
5 4 1
****
*..*
****
**.*
..**

```




```input2
3 3 0
***
*.*
***

```




```output1
1
****
*..*
****
****
..**

```




```output2
1
***
***
***

```



## Note

<p>In the first example there are only two lakes — the first consists of the cells <span class="tex-span">(2, 2)</span> and <span class="tex-span">(2, 3)</span>, the second consists of the cell <span class="tex-span">(4, 3)</span>. It is profitable to cover the second lake because it is smaller. Pay attention that the area of water in the lower left corner is not a lake because this area share a border with the ocean. </p>
