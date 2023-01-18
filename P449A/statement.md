## Description

<div><p>Jzzhu has a big rectangular chocolate bar that consists of <span class="tex-span"><i>n</i> × <i>m</i></span> unit squares. He wants to cut this bar exactly <span class="tex-span"><i>k</i></span> times. Each cut must meet the following requirements:</p><ul> <li> each cut should be straight (horizontal or vertical); </li><li> each cut should go along edges of unit squares (it is prohibited to divide any unit chocolate square with cut); </li><li> each cut should go inside the whole chocolate bar, and all cuts must be distinct. </li></ul><p>The picture below shows a possible way to cut a <span class="tex-span">5 × 6</span> chocolate for <span class="tex-span">5</span> times.</p><center> <img class="tex-graphics" src="file://5otVxEWW.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Imagine Jzzhu have made <span class="tex-span"><i>k</i></span> cuts and the big chocolate is splitted into several pieces. Consider the smallest (by area) piece of the chocolate, Jzzhu wants this piece to be as large as possible. What is the maximum possible area of smallest piece he can get with exactly <span class="tex-span"><i>k</i></span> cuts? The area of a chocolate piece is the number of unit squares in it.</p></div><div class="input-specification"><p>A single line contains three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">9</sup>;&nbsp;1 ≤ <i>k</i> ≤ 2·10<sup class="upper-index">9</sup>)</span>.</p></div><div class="output-specification"><p>Output a single integer representing the answer. If it is impossible to cut the big chocolate <span class="tex-span"><i>k</i></span> times, print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>A single line contains three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">9</sup>;&nbsp;1 ≤ <i>k</i> ≤ 2·10<sup class="upper-index">9</sup>)</span>.</p>

## Output

<p>Output a single integer representing the answer. If it is impossible to cut the big chocolate <span class="tex-span"><i>k</i></span> times, print <span class="tex-font-style-tt">-1</span>.</p>





```input1
3 4 1

```




```input2
6 4 2

```




```input3
2 3 4

```




```output1
6

```




```output2
8

```




```output3
-1

```



## Note

<p>In the first sample, Jzzhu can cut the chocolate following the picture below:</p><center> <img class="tex-graphics" src="file://kGbugk4G.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second sample the optimal division looks like this:</p><center> <img class="tex-graphics" src="file://0jmWuT5V.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the third sample, it's impossible to cut a <span class="tex-span">2 × 3</span> chocolate <span class="tex-span">4</span> times.</p>
