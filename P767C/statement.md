## Description

<div><p>Once at New Year Dima had a dream in which he was presented a fairy garland. A garland is a set of lamps, some pairs of which are connected by wires. Dima remembered that each two lamps in the garland were connected directly or indirectly via some wires. Furthermore, the number of wires was exactly one less than the number of lamps.</p><p>There was something unusual about the garland. Each lamp had its own brightness which depended on the temperature of the lamp. Temperatures could be positive, negative or zero. Dima has two friends, so he decided to share the garland with them. He wants to cut two different wires so that the garland breaks up into three parts. Each part of the garland should shine equally, i.&nbsp;e. the sums of lamps' temperatures should be equal in each of the parts. Of course, each of the parts should be non-empty, i.&nbsp;e. each part should contain at least one lamp.</p><center> <img class="tex-graphics" height="265px" src="file://0Ipb18kU.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px"> </center><p>Help Dima to find a suitable way to cut the garland, or determine that this is impossible.</p><p>While examining the garland, Dima lifted it up holding by one of the lamps. Thus, each of the lamps, except the one he is holding by, is now hanging on some wire. So, you should print two lamp ids as the answer which denote that Dima should cut the wires these lamps are hanging on. Of course, the lamp Dima is holding the garland by can't be included in the answer.</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the number of lamps in the garland.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow. The <span class="tex-span"><i>i</i></span>-th of them contain the information about the <span class="tex-span"><i>i</i></span>-th lamp: the number lamp <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, it is hanging on (and <span class="tex-span">0</span>, if is there is no such lamp), and its temperature <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 100 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>). The lamps are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p></div><div class="output-specification"><p>If there is no solution, print <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise print two integers&nbsp;— the indexes of the lamps which mean Dima should cut the wires they are hanging on. If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the number of lamps in the garland.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow. The <span class="tex-span"><i>i</i></span>-th of them contain the information about the <span class="tex-span"><i>i</i></span>-th lamp: the number lamp <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, it is hanging on (and <span class="tex-span">0</span>, if is there is no such lamp), and its temperature <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 100 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>). The lamps are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p>

## Output

<p>If there is no solution, print <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise print two integers&nbsp;— the indexes of the lamps which mean Dima should cut the wires they are hanging on. If there are multiple answers, print any of them.</p>





```input1
6
2 4
0 5
4 2
2 1
1 1
4 2

```




```input2
6
2 4
0 6
4 2
2 1
1 1
4 2

```




```output1
1 4

```




```output2
-1

```



## Note

<p>The garland and cuts scheme for the first example:</p><center> <img class="tex-graphics" height="212px" src="file://aNNBnkAV.png" style="max-width: 100.0%;max-height: 100.0%;" width="291px"> </center>
