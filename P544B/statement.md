## Description

<div><p>A map of some object is a rectangular field consisting of <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>n</i></span> columns. Each cell is initially occupied by the sea but you can cover some some cells of the map with sand so that exactly <span class="tex-span"><i>k</i></span> islands appear on the map. We will call a set of sand cells to be <span class="tex-font-style-bf">island</span> if it is possible to get from each of them to each of them by moving only through sand cells and by moving from a cell only to a side-adjacent cell. The cells are called to be side-adjacent if they share a vertical or horizontal side. It is easy to see that islands do not share cells (otherwise they together form a bigger island).</p><p>Find a way to cover some cells with sand so that exactly <span class="tex-span"><i>k</i></span> islands appear on the <span class="tex-span"><i>n</i> × <i>n</i></span> map, or determine that no such way exists. </p></div><div class="input-specification"><p>The single line contains two positive integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ <i>n</i><sup class="upper-index">2</sup></span>) — the size of the map and the number of islands you should form.</p></div><div class="output-specification"><p>If the answer doesn't exist, print "NO" (without the quotes) in a single line.</p><p>Otherwise, print "YES" in the first line. In the next <span class="tex-span"><i>n</i></span> lines print the description of the map. Each of the lines of the description must consist only of characters <span class="tex-font-style-tt">'S'</span> and <span class="tex-font-style-tt">'L'</span>, where <span class="tex-font-style-tt">'S'</span> is a cell that is occupied by the sea and <span class="tex-font-style-tt">'L'</span> is the cell covered with sand. The length of each line of the description must equal <span class="tex-span"><i>n</i></span>.</p><p>If there are multiple answers, you may print any of them.</p><p>You <span class="tex-font-style-bf">should not</span> maximize the sizes of islands.</p></div>

## Input

<p>The single line contains two positive integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ <i>n</i><sup class="upper-index">2</sup></span>) — the size of the map and the number of islands you should form.</p>

## Output

<p>If the answer doesn't exist, print "NO" (without the quotes) in a single line.</p><p>Otherwise, print "YES" in the first line. In the next <span class="tex-span"><i>n</i></span> lines print the description of the map. Each of the lines of the description must consist only of characters <span class="tex-font-style-tt">'S'</span> and <span class="tex-font-style-tt">'L'</span>, where <span class="tex-font-style-tt">'S'</span> is a cell that is occupied by the sea and <span class="tex-font-style-tt">'L'</span> is the cell covered with sand. The length of each line of the description must equal <span class="tex-span"><i>n</i></span>.</p><p>If there are multiple answers, you may print any of them.</p><p>You <span class="tex-font-style-bf">should not</span> maximize the sizes of islands.</p>





```input1
5 2

```




```input2
5 25

```




```output1
YES
SSSSS
LLLLL
SSSSS
LLLLL
SSSSS

```




```output2
NO

```


