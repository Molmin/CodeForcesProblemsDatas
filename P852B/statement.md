## Description

<div><p>Due to the recent popularity of the Deep learning new countries are starting to look like Neural Networks. That is, the countries are being built deep with many layers, each layer possibly having many cities. They also have one entry, and one exit point.</p><p>There are exactly <span class="tex-span"><i>L</i></span> layers, each having <span class="tex-span"><i>N</i></span> cities. Let us look at the two adjacent layers <span class="tex-span"><i>L</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>L</i><sub class="lower-index">2</sub></span>. Each city from the layer <span class="tex-span"><i>L</i><sub class="lower-index">1</sub></span> is connected to each city from the layer <span class="tex-span"><i>L</i><sub class="lower-index">2</sub></span> with the traveling cost <span class="tex-span"><i>c</i><sub class="lower-index"><i>ij</i></sub></span> for <img align="middle" class="tex-formula" src="file://XgdlIZNf.png" style="max-width: 100.0%;max-height: 100.0%;">, and each pair of adjacent layers has the same cost in between their cities as any other pair (they just stacked the same layers, as usual). Also, the traveling costs to each city from the layer <span class="tex-span"><i>L</i><sub class="lower-index">2</sub></span> are same for all cities in the <span class="tex-span"><i>L</i><sub class="lower-index">1</sub></span>, that is <span class="tex-span"><i>c</i><sub class="lower-index"><i>ij</i></sub></span> is the same for <img align="middle" class="tex-formula" src="file://oGSBtndK.png" style="max-width: 100.0%;max-height: 100.0%;">, and fixed <span class="tex-span"><i>j</i></span>.</p><p>Doctor G. needs to speed up his computations for this country so he asks you to find the number of paths he can take from entry to exit point such that his traveling cost is divisible by given number <span class="tex-span"><i>M</i></span>.</p></div><div class="input-specification"><p>The first line of input contains <span class="tex-span"><i>N</i> (1 ≤ <i>N</i> ≤ 10<sup class="upper-index">6</sup>)</span>, <span class="tex-span"><i>L</i> (2 ≤ <i>L</i> ≤ 10<sup class="upper-index">5</sup>)</span> and <span class="tex-span"><i>M</i> (2 ≤ <i>M</i> ≤ 100)</span>, the number of cities in each layer, the number of layers and the number that travelling cost should be divisible by, respectively.</p><p>Second, third and fourth line contain <span class="tex-span"><i>N</i></span> integers each denoting costs <span class="tex-span">0 ≤ <i>cost</i> ≤ <i>M</i></span> from entry point to the first layer, costs between adjacent layers as described above, and costs from the last layer to the exit point.</p></div><div class="output-specification"><p>Output a single integer, the number of paths Doctor G. can take which have total cost divisible by <span class="tex-span"><i>M</i></span>, modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line of input contains <span class="tex-span"><i>N</i> (1 ≤ <i>N</i> ≤ 10<sup class="upper-index">6</sup>)</span>, <span class="tex-span"><i>L</i> (2 ≤ <i>L</i> ≤ 10<sup class="upper-index">5</sup>)</span> and <span class="tex-span"><i>M</i> (2 ≤ <i>M</i> ≤ 100)</span>, the number of cities in each layer, the number of layers and the number that travelling cost should be divisible by, respectively.</p><p>Second, third and fourth line contain <span class="tex-span"><i>N</i></span> integers each denoting costs <span class="tex-span">0 ≤ <i>cost</i> ≤ <i>M</i></span> from entry point to the first layer, costs between adjacent layers as described above, and costs from the last layer to the exit point.</p>

## Output

<p>Output a single integer, the number of paths Doctor G. can take which have total cost divisible by <span class="tex-span"><i>M</i></span>, modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
2 3 13
4 6
2 1
3 4

```




```output1
2
```



## Note

<p><img class="tex-graphics" src="file://5537jZ2r.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>This is a country with <span class="tex-span">3</span> layers, each layer having <span class="tex-span">2</span> cities. Paths <img align="middle" class="tex-formula" src="file://vsxuRnrB.png" style="max-width: 100.0%;max-height: 100.0%;">, and <img align="middle" class="tex-formula" src="file://wRJNGimQ.png" style="max-width: 100.0%;max-height: 100.0%;"> are the only paths having total cost divisible by <span class="tex-span">13</span>. Notice that input edges for layer cities have the same cost, and that they are same for all layers.</p>
