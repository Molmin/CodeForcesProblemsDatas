## Description

<div><p><span class="tex-font-style-it">Princess Vlada enjoys springing in the meadows and walking in the forest. One day — wonderful, sunny day — during her walk Princess found out with astonishment that her shadow was missing! "Blimey!", — she thought and started her search of the shadow in the forest.</span></p><p><span class="tex-font-style-it">Normally the Shadow is too lazy and simply sleeps under the Princess. But at this terrifically hot summer day she got bored of such a dull life, so she decided to play with Vlada.</span></p><p>The forest, where our characters entertain themselves, may be represented as a set of integer cells in the plane, where the Shadow and the Princess can move only up, down, left and right by <span class="tex-span">1</span>. Some cells (as it happens in decent forests) are occupied by trees. The Shadow and the Princess are not allowed to enter a cell occupied by a tree. Unfortunately, these are the hard times for the forest, so there are very few trees growing here...</p><p>At first the Princess was walking within the cell (<span class="tex-span"><i>v</i><sub class="lower-index"><i>x</i></sub></span>,&nbsp;<span class="tex-span"><i>v</i><sub class="lower-index"><i>y</i></sub></span>), while the Shadow hid from the Princess in the cell (<span class="tex-span"><i>s</i><sub class="lower-index"><i>x</i></sub></span>,&nbsp;<span class="tex-span"><i>s</i><sub class="lower-index"><i>y</i></sub></span>). The Princess, The Shadow and the trees are located in the different cells.</p><p>The Shadow is playing with the Princess. As soon as the Princess moves by <span class="tex-span">1</span> in some direction, the Shadow simultaneously flies by <span class="tex-span">1</span> in the same direction, if it is possible (if the cell to fly to is not occupied by some tree); otherwise, the Shadow doesn't move. The Shadow is very shadowy, so our characters do not interfere with each other.</p><p>We say that the Shadow is caught by the Princess if after some move both of them are located in the same cell. Vlada managed to catch her Shadow! Can you?</p></div><div class="input-specification"><p>First line of the input contains the coordinates of the characters <span class="tex-span"><i>v</i><sub class="lower-index"><i>x</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>y</i></sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index"><i>x</i></sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index"><i>y</i></sub></span> and the number of trees <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>m</i> ≤ 400</span>). The following <span class="tex-span"><i>m</i></span> lines contain the coordinates of the trees.</p><p>All the coordinates are integers between -100 and 100, inclusive. The Princess, The Shadow and the trees are located in the different cells.</p></div><div class="output-specification"><p>If it is impossible for the Princess to catch the Shadow, print "<span class="tex-font-style-tt">-1</span>" (without quotes).</p><p>Otherwise print a sequence of characters "<span class="tex-font-style-tt">L</span>", "<span class="tex-font-style-tt">R</span>", "<span class="tex-font-style-tt">D</span>", "<span class="tex-font-style-tt">U</span>", corresponding to the Princess's moves, following which she will be able to catch the Shadow at some turn (<span class="tex-font-style-tt">L</span> — move to the left, <span class="tex-font-style-tt">R</span> — to the right, <span class="tex-font-style-tt">U</span> — up, <span class="tex-font-style-tt">D</span> — down; axis <span class="tex-span"><i>x</i></span> is directed to the right, <span class="tex-span"><i>y</i></span> — up).</p><p>The number of characters (that is, the number of moves) must not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>. All the Princess's moves should be correct, that is must not lead to the cell where a tree grows. It is allowed for the Princess and the Shadow to occupy the same cell before the last turn.</p></div>

## Input

<p>First line of the input contains the coordinates of the characters <span class="tex-span"><i>v</i><sub class="lower-index"><i>x</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>y</i></sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index"><i>x</i></sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index"><i>y</i></sub></span> and the number of trees <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>m</i> ≤ 400</span>). The following <span class="tex-span"><i>m</i></span> lines contain the coordinates of the trees.</p><p>All the coordinates are integers between -100 and 100, inclusive. The Princess, The Shadow and the trees are located in the different cells.</p>

## Output

<p>If it is impossible for the Princess to catch the Shadow, print "<span class="tex-font-style-tt">-1</span>" (without quotes).</p><p>Otherwise print a sequence of characters "<span class="tex-font-style-tt">L</span>", "<span class="tex-font-style-tt">R</span>", "<span class="tex-font-style-tt">D</span>", "<span class="tex-font-style-tt">U</span>", corresponding to the Princess's moves, following which she will be able to catch the Shadow at some turn (<span class="tex-font-style-tt">L</span> — move to the left, <span class="tex-font-style-tt">R</span> — to the right, <span class="tex-font-style-tt">U</span> — up, <span class="tex-font-style-tt">D</span> — down; axis <span class="tex-span"><i>x</i></span> is directed to the right, <span class="tex-span"><i>y</i></span> — up).</p><p>The number of characters (that is, the number of moves) must not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>. All the Princess's moves should be correct, that is must not lead to the cell where a tree grows. It is allowed for the Princess and the Shadow to occupy the same cell before the last turn.</p>





```input1
0 0 1 0 1
0 1

```




```input2
5 0 3 0 8
2 -1
2 0
2 1
3 -1
4 1
4 0
3 1
4 -1

```




```input3
3 2 1 1 3
0 1
1 0
0 0

```




```output1
LLUR

```




```output2
-1

```




```output3
DLL
```



## Note

<p>Below the pictures for the samples are given (Princess, Shadow and the trees are colored in pink, gray and black correspondingly; the blue dot marks the lattice center).</p><p>In the first case the Princess may make two left steps, one step upwards and one right step: <img class="tex-graphics" src="file://O6F2MP42.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>In the following case the Princess cannot catch the Shadow: <img class="tex-graphics" src="file://cH6Jki8b.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>In the last sample the Princess may make two left steps and one down step (in any order): <img class="tex-graphics" src="file://QM2k5sgD.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
