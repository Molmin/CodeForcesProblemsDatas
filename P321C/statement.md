## Description

<div><p>Now Fox Ciel becomes a commander of Tree Land. Tree Land, like its name said, has <span class="tex-span"><i>n</i></span> cities connected by <span class="tex-span"><i>n</i> - 1</span> undirected roads, and for any two cities there always exists a path between them.</p><p>Fox Ciel needs to assign an officer to each city. Each officer has a rank — a letter from '<span class="tex-font-style-tt">A</span>' to '<span class="tex-font-style-tt">Z</span>'. So there will be 26 different ranks, and '<span class="tex-font-style-tt">A</span>' is the topmost, so '<span class="tex-font-style-tt">Z</span>' is the bottommost.</p><p>There are enough officers of each rank. But there is a special rule must obey: if <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> are two distinct cities and their officers have the same rank, then on the simple path between <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> there must be a city <span class="tex-span"><i>z</i></span> that has an officer with higher rank. The rule guarantee that a communications between same rank officers will be monitored by higher rank officer.</p><p>Help Ciel to make a valid plan, and if it's impossible, output "<span class="tex-font-style-tt">Impossible!</span>".</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of cities in Tree Land.</p><p>Each of the following <span class="tex-span"><i>n</i> - 1</span> lines contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i>, <i>a</i> ≠ <i>b</i></span>) — they mean that there will be an undirected road between <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. Consider all the cities are numbered from 1 to <span class="tex-span"><i>n</i></span>.</p><p>It guaranteed that the given graph will be a tree.</p></div><div class="output-specification"><p>If there is a valid plane, output <span class="tex-span"><i>n</i></span> space-separated characters in a line — <span class="tex-span"><i>i</i></span>-th character is the rank of officer in the city with number <span class="tex-span"><i>i</i></span>. </p><p>Otherwise output "<span class="tex-font-style-tt">Impossible!</span>".</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of cities in Tree Land.</p><p>Each of the following <span class="tex-span"><i>n</i> - 1</span> lines contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i>, <i>a</i> ≠ <i>b</i></span>) — they mean that there will be an undirected road between <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. Consider all the cities are numbered from 1 to <span class="tex-span"><i>n</i></span>.</p><p>It guaranteed that the given graph will be a tree.</p>

## Output

<p>If there is a valid plane, output <span class="tex-span"><i>n</i></span> space-separated characters in a line — <span class="tex-span"><i>i</i></span>-th character is the rank of officer in the city with number <span class="tex-span"><i>i</i></span>. </p><p>Otherwise output "<span class="tex-font-style-tt">Impossible!</span>".</p>





```input1
4
1 2
1 3
1 4

```




```input2
10
1 2
2 3
3 4
4 5
5 6
6 7
7 8
8 9
9 10

```




```output1
A B B B

```




```output2
D C B A D C B D C D

```



## Note

<p>In the first example, for any two officers of rank '<span class="tex-font-style-tt">B</span>', an officer with rank '<span class="tex-font-style-tt">A</span>' will be on the path between them. So it is a valid solution.</p>
