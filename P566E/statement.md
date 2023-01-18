## Description

<div><p>Archaeologists found some information about an ancient land of Treeland. We know for sure that the Treeland consisted of <span class="tex-span"><i>n</i></span> cities connected by the <span class="tex-span"><i>n</i> - 1</span> road, such that you can get from each city to any other one along the roads. However, the information about the specific design of roads in Treeland has been lost. The only thing that the archaeologists can use is the preserved information about <span class="tex-font-style-it">near</span> cities.</p><p>Two cities of Treeland were called <span class="tex-font-style-it">near</span>, if it were possible to move from one city to the other one by moving through at most two roads. Also, a city is considered <span class="tex-font-style-it">near</span> to itself. During the recent excavations archaeologists found a set of <span class="tex-span"><i>n</i></span> notes, each of them represents a list of cities, <span class="tex-font-style-it">near</span> to some of the <span class="tex-span"><i>n</i></span> cities of the country. However, unfortunately, none of the found records lets you understand in what order the cities go in the list and for which city in the list the <span class="tex-font-style-it">near</span> to it cities were listed. </p><p>Help the archaeologists and restore any variant of the map of Treeland that meets the found information.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>) — the number of cities in the country. </p><p>Next <span class="tex-span"><i>n</i></span> lines describe the found lists of <span class="tex-font-style-it">near</span> cities. Each list starts from number <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>), representing the number of cities in the list followed by <span class="tex-span"><i>k</i></span> city numbers. All numbers in each list are distinct.</p><p>It is guaranteed that the given information determines at least one possible road map.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i> - 1</span> pairs of numbers representing the roads of the country. The <span class="tex-span"><i>i</i></span>-th line must contain two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>), showing that there is a road between cities <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>The answer you print must satisfy the description of close cities from the input. You may print the roads of the countries in any order. The cities that are connected by a road may also be printed in any order.</p><p>If there are multiple good answers, you may print any of them.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>) — the number of cities in the country. </p><p>Next <span class="tex-span"><i>n</i></span> lines describe the found lists of <span class="tex-font-style-it">near</span> cities. Each list starts from number <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>), representing the number of cities in the list followed by <span class="tex-span"><i>k</i></span> city numbers. All numbers in each list are distinct.</p><p>It is guaranteed that the given information determines at least one possible road map.</p>

## Output

<p>Print <span class="tex-span"><i>n</i> - 1</span> pairs of numbers representing the roads of the country. The <span class="tex-span"><i>i</i></span>-th line must contain two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>), showing that there is a road between cities <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>The answer you print must satisfy the description of close cities from the input. You may print the roads of the countries in any order. The cities that are connected by a road may also be printed in any order.</p><p>If there are multiple good answers, you may print any of them.</p>





```input1
5
4 3 2 4 1
5 5 3 2 4 1
5 4 2 1 5 3
4 2 1 4 3
3 1 4 5

```




```input2
6
5 6 1 3 4 2
5 2 1 3 4 6
6 3 6 2 5 4 1
6 6 1 2 5 3 4
3 5 2 4
5 3 1 2 4 6

```




```output1
1 4
1 2
1 3
4 5

```




```output2
2 4
1 2
2 3
2 6
4 5

```


