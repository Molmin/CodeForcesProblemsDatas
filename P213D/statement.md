## Description

<div><p>Furik loves painting stars. A star is a shape that results if we take a regular pentagon and paint all diagonals in it. </p><center> <img class="tex-graphics" src="file://wJWe80WC.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Recently he decided to teach Rubik to paint stars. After many years of training Rubik could paint stars easily. But now Furik decided to test Rubik and complicated the task. Rubik must paint <span class="tex-span"><i>n</i></span> stars, observing the following rules:</p><ul> <li> all stars must be painted in a single move (i.e. it is forbidden to take the pen away from the paper); </li><li> it is forbidden to paint the same segment of non-zero length more than once; </li><li> the stars can intersect only in their vertexes; </li><li> the length of a side of the regular pentagon, in which Rubik paints each star, must equal 10. </li></ul><p>Help Rubik to cope with this hard task.</p></div><div class="input-specification"><p>A single line contains an integer <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span> — the number of stars to paint.</p></div><div class="output-specification"><p>On the first line print an integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 5·<i>n</i>)</span>. On the next <span class="tex-span"><i>m</i></span> lines print coordinates of <span class="tex-span"><i>m</i></span> distinct points with accuracy of at least <span class="tex-span">9</span> and at most <span class="tex-span">100</span> digits after decimal point. All coordinates should not exceed <span class="tex-span">5000</span> in their absolute value. On each of the next <span class="tex-span"><i>n</i></span> lines print <span class="tex-span">5</span> integers — the indexes of the points that form the given star in the clockwise or counterclockwise order. On the next line print <span class="tex-span">5·<i>n</i> + 1</span> integers — the numbers of points in the order, in which Rubik paints stars. That is, if number with index <span class="tex-span"><i>i</i></span> is <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, and number with index <span class="tex-span"><i>i</i> + 1</span> is <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i> + 1</sub></span>, then points with indexes <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i> + 1</sub></span> will have a segment painted between them. </p><p>You can consider all <span class="tex-span"><i>m</i></span> printed points indexed from 1 to <span class="tex-span"><i>m</i></span> in the order, in which they occur in the output. Separate the numbers on the lines with whitespaces.</p><p>Note that the answer has an imprecise validation. Try to obtain as accurate a solution as possible. The validator performs all calculations considering that the absolute error of a participant's answer is not more than <span class="tex-span">10<sup class="upper-index"> - 8</sup></span>.</p></div>

## Input

<p>A single line contains an integer <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span> — the number of stars to paint.</p>

## Output

<p>On the first line print an integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 5·<i>n</i>)</span>. On the next <span class="tex-span"><i>m</i></span> lines print coordinates of <span class="tex-span"><i>m</i></span> distinct points with accuracy of at least <span class="tex-span">9</span> and at most <span class="tex-span">100</span> digits after decimal point. All coordinates should not exceed <span class="tex-span">5000</span> in their absolute value. On each of the next <span class="tex-span"><i>n</i></span> lines print <span class="tex-span">5</span> integers — the indexes of the points that form the given star in the clockwise or counterclockwise order. On the next line print <span class="tex-span">5·<i>n</i> + 1</span> integers — the numbers of points in the order, in which Rubik paints stars. That is, if number with index <span class="tex-span"><i>i</i></span> is <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, and number with index <span class="tex-span"><i>i</i> + 1</span> is <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i> + 1</sub></span>, then points with indexes <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i> + 1</sub></span> will have a segment painted between them. </p><p>You can consider all <span class="tex-span"><i>m</i></span> printed points indexed from 1 to <span class="tex-span"><i>m</i></span> in the order, in which they occur in the output. Separate the numbers on the lines with whitespaces.</p><p>Note that the answer has an imprecise validation. Try to obtain as accurate a solution as possible. The validator performs all calculations considering that the absolute error of a participant's answer is not more than <span class="tex-span">10<sup class="upper-index"> - 8</sup></span>.</p>





```input1
1

```




```output1
5
3.830127018922193 3.366025403784439
-3.601321235851749 10.057331467373021
0.466045194906253 19.192786043799030
10.411264148588986 18.147501411122495
12.490381056766580 8.366025403784439
1 2 3 4 5
1 3 5 2 4 1

```



## Note

<p>The initial position of points in the sample is:</p><center> <img class="tex-graphics" src="file://5iT8WTmI.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The order in which Rubik can paint segments is:</p><center> <img class="tex-graphics" src="file://xByj0F7j.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
