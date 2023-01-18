## Description

<div><p>Sereja painted <span class="tex-span"><i>n</i></span> points on the plane, point number <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i>)</span> has coordinates <span class="tex-span">(<i>i</i>, 0)</span>. Then Sereja marked each point with a small or large English letter. Sereja don't like letter "<span class="tex-font-style-tt">x</span>", so he didn't use it to mark points. Sereja thinks that the points are marked beautifully if the following conditions holds:</p><ul> <li> all points can be divided into pairs so that each point will belong to exactly one pair; </li><li> in each pair the point with the lesser abscissa will be marked with a small English letter and the point with the larger abscissa will be marked with the same large English letter; </li><li> if we built a square on each pair, the pair's points will be the square's opposite points and the segment between them will be the square's diagonal, then among the resulting squares there won't be any intersecting or touching ones. </li></ul><p>Little Petya erased some small and all large letters marking the points. Now Sereja wonders how many ways are there to return the removed letters so that the points were marked beautifully.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> the number of points <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains a sequence consisting of <span class="tex-span"><i>n</i></span> small English letters and question marks — the sequence of letters, that mark points, in order of increasing <span class="tex-span"><i>x</i></span>-coordinate of points. Question marks denote the points without letters (Petya erased them). It is guaranteed that the input string doesn't contain letter "<span class="tex-font-style-tt">x</span>".</p></div><div class="output-specification"><p>In a single line print the answer to the problem modulo <span class="tex-span">4294967296</span>. If there is no way to return the removed letters, print number <span class="tex-span">0</span>.</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> the number of points <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains a sequence consisting of <span class="tex-span"><i>n</i></span> small English letters and question marks — the sequence of letters, that mark points, in order of increasing <span class="tex-span"><i>x</i></span>-coordinate of points. Question marks denote the points without letters (Petya erased them). It is guaranteed that the input string doesn't contain letter "<span class="tex-font-style-tt">x</span>".</p>

## Output

<p>In a single line print the answer to the problem modulo <span class="tex-span">4294967296</span>. If there is no way to return the removed letters, print number <span class="tex-span">0</span>.</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
4
a???

```




```input2
4
abc?

```




```input3
6
abc???

```




```output1
50

```




```output2
0

```




```output3
1

```


