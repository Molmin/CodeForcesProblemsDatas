## Description

<div><p>Autumn came late to the kingdom of Far Far Away. The harvest was exuberant and it is now time to get ready for the winter. As most people celebrate the Harvest festival, Simon the Caretaker tries to solve a very non-trivial task of how to find place for the agricultural equipment in the warehouse.</p><p>He's got problems with some particularly large piece of equipment, which is, of course, turboplows. The problem is that when a turboplow is stored, it takes up not some simply rectangular space. It takes up a T-shaped space like on one of the four pictures below (here character "<span class="tex-font-style-tt">#</span>" stands for the space occupied by the turboplow and character "<span class="tex-font-style-tt">.</span>" stands for the free space):</p><center> <span class="tex-font-style-tt"> <span> <pre class="verbatim">###      ..#      .#.      #..<br>.#.      ###      .#.      ###<br>.#.      ..#      ###      #..<br></pre> </span> </span> </center><p>Simon faced a quite natural challenge: placing in the given <span class="tex-span"><i>n</i> × <i>m</i></span> cells warehouse the maximum number of turboplows. As one stores the turboplows, he can rotate them in any manner (so that they take up the space like on one of the four pictures above). However, two turboplows cannot "overlap", that is, they cannot share the same cell in the warehouse.</p><p>Simon feels that he alone cannot find the optimal way of positioning the plugs in the warehouse that would maximize their quantity. Can you help him?</p></div><div class="input-specification"><p>The only line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> — the sizes of the warehouse (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 9</span>).</p></div><div class="output-specification"><p>In the first line print the maximum number of turboplows that can be positioned in the warehouse. In each of the next <span class="tex-span"><i>n</i></span> lines print <span class="tex-span"><i>m</i></span> characters. Use "<span class="tex-font-style-tt">.</span>" (dot) to mark empty space and use successive capital Latin letters ("<span class="tex-font-style-tt">A</span>" for the first turboplow, "<span class="tex-font-style-tt">B</span>" for the second one and so on until you reach the number of turboplows in your scheme) to mark place for the corresponding turboplows considering that they are positioned in the optimal manner in the warehouse. The order in which you number places for the turboplows does not matter. If there are several optimal solutions for a warehouse of the given size, print any of them.</p></div>

## Input

<p>The only line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> — the sizes of the warehouse (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 9</span>).</p>

## Output

<p>In the first line print the maximum number of turboplows that can be positioned in the warehouse. In each of the next <span class="tex-span"><i>n</i></span> lines print <span class="tex-span"><i>m</i></span> characters. Use "<span class="tex-font-style-tt">.</span>" (dot) to mark empty space and use successive capital Latin letters ("<span class="tex-font-style-tt">A</span>" for the first turboplow, "<span class="tex-font-style-tt">B</span>" for the second one and so on until you reach the number of turboplows in your scheme) to mark place for the corresponding turboplows considering that they are positioned in the optimal manner in the warehouse. The order in which you number places for the turboplows does not matter. If there are several optimal solutions for a warehouse of the given size, print any of them.</p>





```input1
3 3

```




```input2
5 6

```




```input3
2 2

```




```output1
1
AAA
.A.
.A.

```




```output2
4
A..C..
AAAC..
ABCCCD
.B.DDD
BBB..D

```




```output3
0
..
..

```


