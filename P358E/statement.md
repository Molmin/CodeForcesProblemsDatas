## Description

<div><p>Dima is a good person. In fact, he's great. But all good things come to an end...</p><p>Seryozha is going to kick Dima just few times.. For this reason he divides the room into unit squares. Now the room is a rectangle <span class="tex-span"><i>n</i> × <i>m</i></span> consisting of unit squares.</p><p>For the beginning, Seryozha put Dima in a center of some square. Then he started to kick Dima (it is known, that he kicks Dima at least once). Each time when Dima is kicked he flyes up and moves into one of four directions (up, left, right, down). On each move Dima passes <span class="tex-span"><i>k</i></span> <span class="tex-span">(<i>k</i> &gt; 1)</span> unit of the length in the corresponding direction. Seryozha is really kind, so he kicks Dima in such way that Dima never meets the walls (in other words, Dima never leave the room's space). Seryozha is also dynamic character so Dima never flies above the same segment, connecting a pair of adjacent squares, twice.</p><p>Seryozha kicks Dima for a long time, but Dima is not vindictive — Dima writes. Dima marked all squares in which he was staying or above which he was flying. Thanks to kicks, Dima does not remember the <span class="tex-span"><i>k</i></span> value, so he asks you to find all possible values which matches to the Dima's records.</p></div><div class="input-specification"><p>The first line contains <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">3</sup>)</span> — size of the room.</p><p>Next <span class="tex-span"><i>n</i></span> lines goes, each contains <span class="tex-span"><i>m</i></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> — Dima's notes: <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub> = 1</span>, if Dima was staying in the square <span class="tex-span">(<i>i</i>, <i>j</i>)</span> or was flying above it. Otherwise <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub> = 0</span>.</p><p>At least one <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> equals <span class="tex-span">1</span>.</p></div><div class="output-specification"><p>In a single line in accending order print all <span class="tex-span"><i>k</i></span> <span class="tex-span">(<i>k</i> &gt; 1)</span>, which matches the Dima's notes. If there are no such <span class="tex-span"><i>k</i></span> and Dima invented this story with kicks, print -<span class="tex-span">1</span>.</p></div>

## Input

<p>The first line contains <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">3</sup>)</span> — size of the room.</p><p>Next <span class="tex-span"><i>n</i></span> lines goes, each contains <span class="tex-span"><i>m</i></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> — Dima's notes: <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub> = 1</span>, if Dima was staying in the square <span class="tex-span">(<i>i</i>, <i>j</i>)</span> or was flying above it. Otherwise <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub> = 0</span>.</p><p>At least one <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> equals <span class="tex-span">1</span>.</p>

## Output

<p>In a single line in accending order print all <span class="tex-span"><i>k</i></span> <span class="tex-span">(<i>k</i> &gt; 1)</span>, which matches the Dima's notes. If there are no such <span class="tex-span"><i>k</i></span> and Dima invented this story with kicks, print -<span class="tex-span">1</span>.</p>





```input1
5 5
1 1 1 1 1
1 0 0 0 1
1 0 0 0 1
1 0 0 0 1
1 1 1 1 1

```




```input2
7 7
0 0 1 1 1 0 0
0 0 1 0 1 0 0
1 1 1 1 1 1 1
1 0 1 0 1 0 1
1 1 1 1 1 1 1
0 0 1 0 1 0 0
0 0 1 1 1 0 0

```




```input3
3 3
1 1 1
1 1 1
1 1 1

```




```input4
4 4
1 1 1 1
0 0 0 0
0 0 0 0
0 0 0 0

```




```input5
5 5
0 0 1 0 0
0 0 1 0 0
1 1 1 1 1
0 0 1 0 0
0 0 1 0 0

```




```output1
2 4

```




```output2
2

```




```output3
-1

```




```output4
3

```




```output5
-1

```


