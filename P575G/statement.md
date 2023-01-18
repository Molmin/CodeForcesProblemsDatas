## Description

<div><p>People in BubbleLand like to drink beer. Little do you know, beer here is so good and strong that every time you drink it your speed goes 10 times slower than before you drank it.</p><p>Birko lives in city Beergrade, but wants to go to city Beerburg. You are given a road map of BubbleLand and you need to find the fastest way for him. When he starts his journey in Beergrade his speed is 1. When he comes to a new city he always tries a glass of local beer, which divides his speed by 10. </p><p>The question here is what the minimal time for him to reach Beerburg is. If there are several paths with the same minimal time, pick the one that has least roads on it. If there is still more than one path, pick any.</p><p>It is guaranteed that there will be at least one path from Beergrade to Beerburg.</p></div><div class="input-specification"><p>The first line of input contains integer <span class="tex-span"><i>N</i></span> — the number of cities in Bubbleland and integer <span class="tex-span"><i>M</i></span> — the number of roads in this country. Cities are enumerated from 0 to <span class="tex-span"><i>N</i> - 1</span>, with city 0 being Beergrade, and city <span class="tex-span"><i>N</i> - 1</span> being Beerburg. Each of the following <span class="tex-span"><i>M</i></span> lines contains three integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> (<span class="tex-span"><i>a</i> ≠ <i>b</i></span>) and <span class="tex-span"><i>len</i></span>. These numbers indicate that there is a bidirectional road between cities <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> with length <span class="tex-span"><i>len</i></span>. </p><ul> <li> <span class="tex-span">2 ≤ <i>N</i> ≤ 10<sup class="upper-index">5</sup></span> </li><li> <span class="tex-span">1 ≤ <i>M</i> ≤ 10<sup class="upper-index">5</sup></span> </li><li> <span class="tex-span">0 ≤ <i>len</i> ≤ 9</span> </li><li> There is at most one road between two cities </li></ul></div><div class="output-specification"><p>The first line of output should contain minimal time needed to go from Beergrade to Beerburg.</p><p>The second line of the output should contain the number of cities on the path from Beergrade to Beerburg that takes minimal time. </p><p>The third line of output should contain the numbers of cities on this path in the order they are visited, separated by spaces.</p></div>

## Input

<p>The first line of input contains integer <span class="tex-span"><i>N</i></span> — the number of cities in Bubbleland and integer <span class="tex-span"><i>M</i></span> — the number of roads in this country. Cities are enumerated from 0 to <span class="tex-span"><i>N</i> - 1</span>, with city 0 being Beergrade, and city <span class="tex-span"><i>N</i> - 1</span> being Beerburg. Each of the following <span class="tex-span"><i>M</i></span> lines contains three integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> (<span class="tex-span"><i>a</i> ≠ <i>b</i></span>) and <span class="tex-span"><i>len</i></span>. These numbers indicate that there is a bidirectional road between cities <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> with length <span class="tex-span"><i>len</i></span>. </p><ul> <li> <span class="tex-span">2 ≤ <i>N</i> ≤ 10<sup class="upper-index">5</sup></span> </li><li> <span class="tex-span">1 ≤ <i>M</i> ≤ 10<sup class="upper-index">5</sup></span> </li><li> <span class="tex-span">0 ≤ <i>len</i> ≤ 9</span> </li><li> There is at most one road between two cities </li></ul>

## Output

<p>The first line of output should contain minimal time needed to go from Beergrade to Beerburg.</p><p>The second line of the output should contain the number of cities on the path from Beergrade to Beerburg that takes minimal time. </p><p>The third line of output should contain the numbers of cities on this path in the order they are visited, separated by spaces.</p>





```input1
8 10
0 1 1
1 2 5
2 7 6
0 3 2
3 7 3
0 4 0
4 5 0
5 7 2
0 6 0
6 7 7

```




```output1
32
3
0 3 7

```


