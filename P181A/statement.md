## Description

<div><p>The Berland capital is shaken with three bold crimes committed by the Pihsters, a notorious criminal gang.</p><p>The Berland capital's map is represented by an <span class="tex-span"><i>n</i> × <i>m</i></span> rectangular table. Each cell of the table on the map represents some districts of the capital. </p><p>The capital's main detective Polycarpus took a map and marked there the districts where the first three robberies had been committed as asterisks. Deduction tells Polycarpus that the fourth robbery will be committed in such district, that all four robbed districts will form the vertices of some rectangle, parallel to the sides of the map. </p><p>Polycarpus is good at deduction but he's hopeless at math. So he asked you to find the district where the fourth robbery will be committed.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 100</span>) — the number of rows and columns in the table, correspondingly.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters — the description of the capital's map. Each character can either be a "<span class="tex-font-style-tt">.</span>" (dot), or an "<span class="tex-font-style-tt">*</span>" (asterisk). A character equals "<span class="tex-font-style-tt">*</span>" if the corresponding district has been robbed. Otherwise, it equals "<span class="tex-font-style-tt">.</span>".</p><p>It is guaranteed that the map has exactly three characters "<span class="tex-font-style-tt">*</span>" and we can always find the fourth district that meets the problem requirements. </p></div><div class="output-specification"><p>Print two integers — the number of the row and the number of the column of the city district that is the fourth one to be robbed. The rows are numbered starting from one from top to bottom and the columns are numbered starting from one from left to right.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 100</span>) — the number of rows and columns in the table, correspondingly.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters — the description of the capital's map. Each character can either be a "<span class="tex-font-style-tt">.</span>" (dot), or an "<span class="tex-font-style-tt">*</span>" (asterisk). A character equals "<span class="tex-font-style-tt">*</span>" if the corresponding district has been robbed. Otherwise, it equals "<span class="tex-font-style-tt">.</span>".</p><p>It is guaranteed that the map has exactly three characters "<span class="tex-font-style-tt">*</span>" and we can always find the fourth district that meets the problem requirements. </p>

## Output

<p>Print two integers — the number of the row and the number of the column of the city district that is the fourth one to be robbed. The rows are numbered starting from one from top to bottom and the columns are numbered starting from one from left to right.</p>





```input1
3 2
.*
..
**

```




```input2
3 3
*.*
*..
...

```




```output1
1 1

```




```output2
2 3

```


