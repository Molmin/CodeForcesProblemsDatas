## Description

<div><p>In the computer network of the Berland State University there are <span class="tex-span"><i>n</i></span> routers numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Some pairs of routers are connected by patch cords. Information can be transmitted over patch cords in both direction. The network is arranged in such a way that communication between any two routers (directly or through other routers) is possible. There are no cycles in the network, so there is only one path between each pair of routers over patch cords.</p><p>Unfortunately, the exact topology of the network was lost by administrators. In order to restore it, the following auxiliary information was collected.</p><p>For each patch cord <span class="tex-span"><i>p</i></span>, directly connected to the router <span class="tex-span"><i>i</i></span>, list of routers located behind the patch cord <span class="tex-span"><i>p</i></span> relatively <span class="tex-span"><i>i</i></span> is known. In other words, all routers path from which to the router <span class="tex-span"><i>i</i></span> goes through <span class="tex-span"><i>p</i></span> are known. So for each router <span class="tex-span"><i>i</i></span> there are <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> lists, where <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> is the number of patch cords connected to <span class="tex-span"><i>i</i></span>.</p><p>For example, let the network consists of three routers connected in chain <span class="tex-span">1 - 2 - 3</span>. Then:</p><ul> <li> the router <span class="tex-span">1</span>: for the single patch cord connected to the first router there is a single list containing two routers: <span class="tex-span">2</span> and <span class="tex-span">3</span>; </li><li> the router <span class="tex-span">2</span>: for each of the patch cords connected to the second router there is a list: one list contains the router <span class="tex-span">1</span> and the other — the router <span class="tex-span">3</span>; </li><li> the router <span class="tex-span">3</span>: for the single patch cord connected to the third router there is a single list containing two routers: <span class="tex-span">1</span> and <span class="tex-span">2</span>. </li></ul><p>Your task is to help administrators to restore the network topology, i. e. to identify all pairs of routers directly connected by a patch cord.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>) — the number of routers in the network.</p><p>The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>n</i></span> lines contains a description of the lists for the router <span class="tex-span"><i>i</i></span>.</p><p>The description of each list begins with the number of routers in it. Then the symbol '<span class="tex-font-style-tt">:</span>' follows, and after that the numbers of routers from the list are given. This numbers are separated by comma. Lists are separated by symbol '<span class="tex-font-style-tt">-</span>'.</p><p>It is guaranteed, that for each router <span class="tex-span"><i>i</i></span> the total number of routers in its lists equals to <span class="tex-span"><i>n</i> - 1</span> and all the numbers in lists of each router are distinct. For each router <span class="tex-span"><i>i</i></span> lists do not contain the number <span class="tex-span"><i>i</i></span>.</p></div><div class="output-specification"><p>Print <span class="tex-font-style-tt">-1</span> if no solution exists.</p><p>In the other case print to the first line <span class="tex-span"><i>n</i> - 1</span> — the total number of patch cords in the network. In each of the following <span class="tex-span"><i>n</i> - 1</span> lines print two integers — the routers which are directly connected by a patch cord. Information about each patch cord must be printed exactly once.</p><p>Patch cords and routers can be printed in arbitrary order.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>) — the number of routers in the network.</p><p>The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>n</i></span> lines contains a description of the lists for the router <span class="tex-span"><i>i</i></span>.</p><p>The description of each list begins with the number of routers in it. Then the symbol '<span class="tex-font-style-tt">:</span>' follows, and after that the numbers of routers from the list are given. This numbers are separated by comma. Lists are separated by symbol '<span class="tex-font-style-tt">-</span>'.</p><p>It is guaranteed, that for each router <span class="tex-span"><i>i</i></span> the total number of routers in its lists equals to <span class="tex-span"><i>n</i> - 1</span> and all the numbers in lists of each router are distinct. For each router <span class="tex-span"><i>i</i></span> lists do not contain the number <span class="tex-span"><i>i</i></span>.</p>

## Output

<p>Print <span class="tex-font-style-tt">-1</span> if no solution exists.</p><p>In the other case print to the first line <span class="tex-span"><i>n</i> - 1</span> — the total number of patch cords in the network. In each of the following <span class="tex-span"><i>n</i> - 1</span> lines print two integers — the routers which are directly connected by a patch cord. Information about each patch cord must be printed exactly once.</p><p>Patch cords and routers can be printed in arbitrary order.</p>





```input1
3
2:3,2
1:1-1:3
2:1,2

```




```input2
5
4:2,5,3,4
1:4-1:1-2:5,3
4:4,5,2,1
4:2,1,3,5
1:3-3:4,2,1

```




```input3
3
1:2-1:3
1:1-1:3
1:1-1:2

```




```output1
2
2 1
2 3

```




```output2
4
2 1
2 4
5 2
3 5

```




```output3
-1

```



## Note

<p>The first example is analyzed in the statement.</p><p>The answer to the second example is shown on the picture.</p><center> <img class="tex-graphics" src="file://yzCbjStH.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The first router has one list, which contains all other routers. The second router has three lists: the first — the single router <span class="tex-span">4</span>, the second — the single router <span class="tex-span">1</span>, the third — two routers <span class="tex-span">3</span> and <span class="tex-span">5</span>. The third router has one list, which contains all other routers. The fourth router also has one list, which contains all other routers. The fifth router has two lists: the first — the single router <span class="tex-span">3</span>, the second — three routers <span class="tex-span">1</span>, <span class="tex-span">2</span> and <span class="tex-span">4</span>.</p>
