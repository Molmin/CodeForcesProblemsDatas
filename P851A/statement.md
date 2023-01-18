## Description

<div><p>Arpa is researching the Mexican wave.</p><p>There are <span class="tex-span"><i>n</i></span> spectators in the stadium, labeled from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. They start the Mexican wave at time <span class="tex-span">0</span>. </p><ul> <li> At time <span class="tex-span">1</span>, the first spectator stands. </li><li> At time <span class="tex-span">2</span>, the second spectator stands. </li><li> <span class="tex-span">...</span> </li><li> At time <span class="tex-span"><i>k</i></span>, the <span class="tex-span"><i>k</i></span>-th spectator stands. </li><li> At time <span class="tex-span"><i>k</i> + 1</span>, the <span class="tex-span">(<i>k</i> + 1)</span>-th spectator stands and the first spectator sits. </li><li> At time <span class="tex-span"><i>k</i> + 2</span>, the <span class="tex-span">(<i>k</i> + 2)</span>-th spectator stands and the second spectator sits. </li><li> <span class="tex-span">...</span> </li><li> At time <span class="tex-span"><i>n</i></span>, the <span class="tex-span"><i>n</i></span>-th spectator stands and the <span class="tex-span">(<i>n</i> - <i>k</i>)</span>-th spectator sits. </li><li> At time <span class="tex-span"><i>n</i> + 1</span>, the <span class="tex-span">(<i>n</i> + 1 - <i>k</i>)</span>-th spectator sits. </li><li> <span class="tex-span">...</span> </li><li> At time <span class="tex-span"><i>n</i> + <i>k</i></span>, the <span class="tex-span"><i>n</i></span>-th spectator sits. </li></ul><p>Arpa wants to know how many spectators are standing at time <span class="tex-span"><i>t</i></span>.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>t</i> &lt; <i>n</i> + <i>k</i></span>).</p></div><div class="output-specification"><p>Print single integer: how many spectators are standing at time <span class="tex-span"><i>t</i></span>.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>t</i> &lt; <i>n</i> + <i>k</i></span>).</p>

## Output

<p>Print single integer: how many spectators are standing at time <span class="tex-span"><i>t</i></span>.</p>





```input1
10 5 3

```




```input2
10 5 7

```




```input3
10 5 12

```




```output1
3

```




```output2
5

```




```output3
3

```



## Note

<p>In the following a sitting spectator is represented as <span class="tex-font-style-tt">-</span>, a standing spectator is represented as <span class="tex-font-style-tt">^</span>.</p><ul> <li> At <span class="tex-span"><i>t</i> = 0 </span> <span class="tex-font-style-tt">----------</span> <img align="middle" class="tex-formula" src="file://RmdNJ9JW.png" style="max-width: 100.0%;max-height: 100.0%;"> number of standing spectators = 0. </li><li> At <span class="tex-span"><i>t</i> = 1 </span> <span class="tex-font-style-tt">^---------</span> <img align="middle" class="tex-formula" src="file://Szc3WLT0.png" style="max-width: 100.0%;max-height: 100.0%;"> number of standing spectators = 1. </li><li> At <span class="tex-span"><i>t</i> = 2 </span> <span class="tex-font-style-tt">^^--------</span> <img align="middle" class="tex-formula" src="file://NnGrEpnh.png" style="max-width: 100.0%;max-height: 100.0%;"> number of standing spectators = 2. </li><li> At <span class="tex-span"><i>t</i> = 3 </span> <span class="tex-font-style-tt">^^^-------</span> <img align="middle" class="tex-formula" src="file://CL2r7ec4.png" style="max-width: 100.0%;max-height: 100.0%;"> number of standing spectators = 3. </li><li> At <span class="tex-span"><i>t</i> = 4 </span> <span class="tex-font-style-tt">^^^^------</span> <img align="middle" class="tex-formula" src="file://C0SZL3qu.png" style="max-width: 100.0%;max-height: 100.0%;"> number of standing spectators = 4. </li><li> At <span class="tex-span"><i>t</i> = 5 </span> <span class="tex-font-style-tt">^^^^^-----</span> <img align="middle" class="tex-formula" src="file://fyaXm1hr.png" style="max-width: 100.0%;max-height: 100.0%;"> number of standing spectators = 5. </li><li> At <span class="tex-span"><i>t</i> = 6 </span> <span class="tex-font-style-tt">-^^^^^----</span> <img align="middle" class="tex-formula" src="file://gx1MdKKN.png" style="max-width: 100.0%;max-height: 100.0%;"> number of standing spectators = 5. </li><li> At <span class="tex-span"><i>t</i> = 7 </span> <span class="tex-font-style-tt">--^^^^^---</span> <img align="middle" class="tex-formula" src="file://D67Fr4kG.png" style="max-width: 100.0%;max-height: 100.0%;"> number of standing spectators = 5. </li><li> At <span class="tex-span"><i>t</i> = 8 </span> <span class="tex-font-style-tt">---^^^^^--</span> <img align="middle" class="tex-formula" src="file://7H0RpFUs.png" style="max-width: 100.0%;max-height: 100.0%;"> number of standing spectators = 5. </li><li> At <span class="tex-span"><i>t</i> = 9 </span> <span class="tex-font-style-tt">----^^^^^-</span> <img align="middle" class="tex-formula" src="file://d4eGi2TD.png" style="max-width: 100.0%;max-height: 100.0%;"> number of standing spectators = 5. </li><li> At <span class="tex-span"><i>t</i> = 10</span> <span class="tex-font-style-tt">-----^^^^^</span> <img align="middle" class="tex-formula" src="file://vwaG5Hw6.png" style="max-width: 100.0%;max-height: 100.0%;"> number of standing spectators = 5. </li><li> At <span class="tex-span"><i>t</i> = 11</span> <span class="tex-font-style-tt">------^^^^</span> <img align="middle" class="tex-formula" src="file://mejeL9DH.png" style="max-width: 100.0%;max-height: 100.0%;"> number of standing spectators = 4. </li><li> At <span class="tex-span"><i>t</i> = 12</span> <span class="tex-font-style-tt">-------^^^</span> <img align="middle" class="tex-formula" src="file://XFs3rkVC.png" style="max-width: 100.0%;max-height: 100.0%;"> number of standing spectators = 3. </li><li> At <span class="tex-span"><i>t</i> = 13</span> <span class="tex-font-style-tt">--------^^</span> <img align="middle" class="tex-formula" src="file://kRmG4QwL.png" style="max-width: 100.0%;max-height: 100.0%;"> number of standing spectators = 2. </li><li> At <span class="tex-span"><i>t</i> = 14</span> <span class="tex-font-style-tt">---------^</span> <img align="middle" class="tex-formula" src="file://IJqq9jOQ.png" style="max-width: 100.0%;max-height: 100.0%;"> number of standing spectators = 1. </li><li> At <span class="tex-span"><i>t</i> = 15</span> <span class="tex-font-style-tt">----------</span> <img align="middle" class="tex-formula" src="file://sx8lrdyv.png" style="max-width: 100.0%;max-height: 100.0%;"> number of standing spectators = 0. </li></ul>
