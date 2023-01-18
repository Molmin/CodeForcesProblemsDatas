## Description

<div><p>Vasya plays FreeDiv. In this game he manages a huge state, which has <span class="tex-span"><i>n</i></span> cities and <span class="tex-span"><i>m</i></span> two-way roads between them. Unfortunately, not from every city you can reach any other one moving along these roads. Therefore Vasya decided to divide the state into provinces so that in every province, one could reach from every city all the cities of the province, but there are no roads between provinces. </p><p>Unlike other turn-based strategies, in FreeDiv a player has the opportunity to build tunnels between cities. The tunnels are two-way roads along which one can move armies undetected by the enemy. However, no more than one tunnel can be connected to each city. As for Vasya, he wants to build a network of tunnels so that any pair of cities in his state were reachable by some path consisting of roads and a tunnels. But at that no more than <span class="tex-span"><i>k</i></span> tunnels are connected to each province (otherwise, the province will be difficult to keep in case other provinces are captured by enemy armies).</p><p>Vasya discovered that maybe he will not be able to build such a network for the current condition of the state. Maybe he'll have first to build several roads between cities in different provinces to merge the provinces. Your task is to determine the minimum number of roads Vasya needs to build so that it was possible to build the required network of tunnels in the resulting state.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 10<sup class="upper-index">6</sup>, 0 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>). Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers. They are the numbers of cities connected by a corresponding road. No road connects city to itself and there is at most one road between each pair of cities.</p></div><div class="output-specification"><p>Print a single number, the minimum number of additional roads.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 10<sup class="upper-index">6</sup>, 0 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>). Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers. They are the numbers of cities connected by a corresponding road. No road connects city to itself and there is at most one road between each pair of cities.</p>

## Output

<p>Print a single number, the minimum number of additional roads.</p>





```input1
3 3 2
1 2
2 3
3 1

```




```input2
4 2 2
1 2
3 4

```




```input3
4 0 2

```




```output1
0
```




```output2
0
```




```output3
1
```



## Note

<p>In the first example only one province exists, so it is not necessary to build any tunnels or roads.</p><p>In the second example two provinces exist. It is possible to merge the provinces by building a tunnel between cities 1 and 3.</p><p>In the third example at least one additional road is necessary. For example it is possible to build additional road between cities 1 and 2 and build two tunnels between cities 1 and 3, 2 and 4 after that.</p>
