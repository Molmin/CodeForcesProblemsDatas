## Description

<div><p>There is a white sheet of paper lying on a rectangle table. The sheet is a rectangle with its sides parallel to the sides of the table. If you will take a look from above and assume that the bottom left corner of the table has coordinates $(0, 0)$, and coordinate axes are left and bottom sides of the table, then the bottom left corner of the white sheet has coordinates $(x_1, y_1)$, and the top right — $(x_2, y_2)$.</p><p>After that two black sheets of paper are placed on the table. Sides of both black sheets are also parallel to the sides of the table. Coordinates of the bottom left corner of the first black sheet are $(x_3, y_3)$, and the top right — $(x_4, y_4)$. Coordinates of the bottom left corner of the second black sheet are $(x_5, y_5)$, and the top right — $(x_6, y_6)$. </p><center> <img class="tex-graphics" src="file://YFrt7Snb.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">Example of three rectangles.</span> </center><p>Determine if some part of the white sheet can be seen from the above after the two black sheets are placed. The part of the white sheet can be seen if there is at least one point lying <span class="tex-font-style-bf">not strictly inside</span> the white sheet and <span class="tex-font-style-bf">strictly outside</span> of both black sheets.</p></div><div class="input-specification"><p>The first line of the input contains four integers $x_1, y_1, x_2, y_2$ $(0 \le x_1 &lt; x_2 \le 10^{6}, 0 \le y_1 &lt; y_2 \le 10^{6})$ — coordinates of the bottom left and the top right corners of the white sheet.</p><p>The second line of the input contains four integers $x_3, y_3, x_4, y_4$ $(0 \le x_3 &lt; x_4 \le 10^{6}, 0 \le y_3 &lt; y_4 \le 10^{6})$ — coordinates of the bottom left and the top right corners of the first black sheet.</p><p>The third line of the input contains four integers $x_5, y_5, x_6, y_6$ $(0 \le x_5 &lt; x_6 \le 10^{6}, 0 \le y_5 &lt; y_6 \le 10^{6})$ — coordinates of the bottom left and the top right corners of the second black sheet.</p><p><span class="tex-font-style-bf">The sides of each sheet of paper are parallel (perpendicular) to the coordinate axes.</span></p></div><div class="output-specification"><p>If some part of the white sheet can be seen from the above after the two black sheets are placed, print "<span class="tex-font-style-tt">YES</span>" (without quotes). Otherwise print "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>The first line of the input contains four integers $x_1, y_1, x_2, y_2$ $(0 \le x_1 &lt; x_2 \le 10^{6}, 0 \le y_1 &lt; y_2 \le 10^{6})$ — coordinates of the bottom left and the top right corners of the white sheet.</p><p>The second line of the input contains four integers $x_3, y_3, x_4, y_4$ $(0 \le x_3 &lt; x_4 \le 10^{6}, 0 \le y_3 &lt; y_4 \le 10^{6})$ — coordinates of the bottom left and the top right corners of the first black sheet.</p><p>The third line of the input contains four integers $x_5, y_5, x_6, y_6$ $(0 \le x_5 &lt; x_6 \le 10^{6}, 0 \le y_5 &lt; y_6 \le 10^{6})$ — coordinates of the bottom left and the top right corners of the second black sheet.</p><p><span class="tex-font-style-bf">The sides of each sheet of paper are parallel (perpendicular) to the coordinate axes.</span></p>

## Output

<p>If some part of the white sheet can be seen from the above after the two black sheets are placed, print "<span class="tex-font-style-tt">YES</span>" (without quotes). Otherwise print "<span class="tex-font-style-tt">NO</span>".</p>





```input1
2 2 4 4
1 1 3 5
3 1 5 5
```




```input2
3 3 7 5
0 0 4 6
0 0 7 4
```




```input3
5 2 10 5
3 1 7 6
8 1 11 7
```




```input4
0 0 1000000 1000000
0 0 499999 1000000
500000 0 1000000 1000000
```




```output1
NO
```




```output2
YES
```




```output3
YES
```




```output4
YES
```



## Note

<p>In the first example the white sheet is fully covered by black sheets.</p><p>In the second example the part of the white sheet can be seen after two black sheets are placed. For example, the point $(6.5, 4.5)$ lies not strictly inside the white sheet and lies strictly outside of both black sheets.</p>
