## Description

<div><p>Genos has been given <span class="tex-span"><i>n</i></span> distinct lines on the Cartesian plane. Let <img align="middle" class="tex-formula" src="file://QFdpCMg4.png" style="max-width: 100.0%;max-height: 100.0%;"> be a list of intersection points of these lines. A single point might appear multiple times in this list if it is the intersection of multiple pairs of lines. The order of the list does not matter.</p><p>Given a query point <span class="tex-span">(<i>p</i>, <i>q</i>)</span>, let <img align="middle" class="tex-formula" src="file://SYjs0whe.png" style="max-width: 100.0%;max-height: 100.0%;"> be the corresponding list of distances of all points in <img align="middle" class="tex-formula" src="file://dl5PGRtb.png" style="max-width: 100.0%;max-height: 100.0%;"> to the query point. Distance here refers to euclidean distance. As a refresher, the euclidean distance between two points <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> and <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span> is <img align="middle" class="tex-formula" src="file://bnIxrQJh.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Genos is given a point <span class="tex-span">(<i>p</i>, <i>q</i>)</span> and a positive integer <span class="tex-span"><i>m</i></span>. He is asked to find the sum of the <span class="tex-span"><i>m</i></span> smallest elements in <img align="middle" class="tex-formula" src="file://ylgdIAPX.png" style="max-width: 100.0%;max-height: 100.0%;">. Duplicate elements in <img align="middle" class="tex-formula" src="file://GqKHIDt5.png" style="max-width: 100.0%;max-height: 100.0%;"> are treated as separate elements. Genos is intimidated by Div1 E problems so he asked for your help.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 50 000</span>)&nbsp;— the number of lines.</p><p>The second line contains three integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">|<i>x</i>|, |<i>y</i>| ≤ 1 000 000</span>, <img align="middle" class="tex-formula" src="file://WHf3yBhv.png" style="max-width: 100.0%;max-height: 100.0%;">)&nbsp;— the encoded coordinates of the query point and the integer <span class="tex-span"><i>m</i></span> from the statement above. The query point <span class="tex-span">(<i>p</i>, <i>q</i>)</span> is obtained as <img align="middle" class="tex-formula" src="file://jJ7zxOlI.png" style="max-width: 100.0%;max-height: 100.0%;">. In other words, divide <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> by <span class="tex-span">1000</span> to get the actual query point. <img align="middle" class="tex-formula" src="file://AVOtcUrG.png" style="max-width: 100.0%;max-height: 100.0%;"> denotes the length of the list <img align="middle" class="tex-formula" src="file://gaVSWPn8.png" style="max-width: 100.0%;max-height: 100.0%;"> and it is guaranteed that <img align="middle" class="tex-formula" src="file://o8hfXSzh.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>|, |<i>b</i><sub class="lower-index"><i>i</i></sub>| ≤ 1 000 000</span>)&nbsp;— the parameters for a line of the form: <img align="middle" class="tex-formula" src="file://QduVqHLR.png" style="max-width: 100.0%;max-height: 100.0%;">. It is guaranteed that no two lines are the same, that is <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>) ≠ (<i>a</i><sub class="lower-index"><i>j</i></sub>, <i>b</i><sub class="lower-index"><i>j</i></sub>)</span> if <span class="tex-span"><i>i</i> ≠ <i>j</i></span>.</p></div><div class="output-specification"><p>Print a single real number, the sum of <span class="tex-span"><i>m</i></span> smallest elements of <img align="middle" class="tex-formula" src="file://ISl6YJHv.png" style="max-width: 100.0%;max-height: 100.0%;">. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p><p>To clarify, let's assume that your answer is <span class="tex-span"><i>a</i></span> and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct if <img align="middle" class="tex-formula" src="file://o09w04uh.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 50 000</span>)&nbsp;— the number of lines.</p><p>The second line contains three integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">|<i>x</i>|, |<i>y</i>| ≤ 1 000 000</span>, <img align="middle" class="tex-formula" src="file://WHf3yBhv.png" style="max-width: 100.0%;max-height: 100.0%;">)&nbsp;— the encoded coordinates of the query point and the integer <span class="tex-span"><i>m</i></span> from the statement above. The query point <span class="tex-span">(<i>p</i>, <i>q</i>)</span> is obtained as <img align="middle" class="tex-formula" src="file://jJ7zxOlI.png" style="max-width: 100.0%;max-height: 100.0%;">. In other words, divide <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> by <span class="tex-span">1000</span> to get the actual query point. <img align="middle" class="tex-formula" src="file://AVOtcUrG.png" style="max-width: 100.0%;max-height: 100.0%;"> denotes the length of the list <img align="middle" class="tex-formula" src="file://gaVSWPn8.png" style="max-width: 100.0%;max-height: 100.0%;"> and it is guaranteed that <img align="middle" class="tex-formula" src="file://o8hfXSzh.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>|, |<i>b</i><sub class="lower-index"><i>i</i></sub>| ≤ 1 000 000</span>)&nbsp;— the parameters for a line of the form: <img align="middle" class="tex-formula" src="file://QduVqHLR.png" style="max-width: 100.0%;max-height: 100.0%;">. It is guaranteed that no two lines are the same, that is <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>) ≠ (<i>a</i><sub class="lower-index"><i>j</i></sub>, <i>b</i><sub class="lower-index"><i>j</i></sub>)</span> if <span class="tex-span"><i>i</i> ≠ <i>j</i></span>.</p>

## Output

<p>Print a single real number, the sum of <span class="tex-span"><i>m</i></span> smallest elements of <img align="middle" class="tex-formula" src="file://ISl6YJHv.png" style="max-width: 100.0%;max-height: 100.0%;">. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p><p>To clarify, let's assume that your answer is <span class="tex-span"><i>a</i></span> and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct if <img align="middle" class="tex-formula" src="file://o09w04uh.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
4
1000 1000 3
1000 0
-1000 0
0 5000
0 -5000

```




```input2
2
-1000000 -1000000 1
1000000 -1000000
999999 1000000

```




```input3
3
-1000 1000 3
1000 0
-1000 2000
2000 -1000

```




```input4
5
-303667 189976 10
-638 116487
-581 44337
1231 -756844
1427 -44097
8271 -838417

```




```output1
14.282170363

```




```output2
2000001000.999999500

```




```output3
6.000000000

```




```output4
12953.274911829

```



## Note

<p>In the first sample, the three closest points have distances <img align="middle" class="tex-formula" src="file://j3hZbiuY.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="file://XPt2XDZV.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>In the second sample, the two lines <span class="tex-span"><i>y</i> = 1000<i>x</i> - 1000</span> and <img align="middle" class="tex-formula" src="file://H7M6Qo9Y.png" style="max-width: 100.0%;max-height: 100.0%;"> intersect at <span class="tex-span">(2000000, 1999999000)</span>. This point has a distance of <img align="middle" class="tex-formula" src="file://RhaBc2yu.png" style="max-width: 100.0%;max-height: 100.0%;"> from <span class="tex-span">( - 1000,  - 1000)</span>.</p><p>In the third sample, the three lines all intersect at the point <span class="tex-span">(1, 1)</span>. This intersection point is present three times in <img align="middle" class="tex-formula" src="file://Qy6ZqWIP.png" style="max-width: 100.0%;max-height: 100.0%;"> since it is the intersection of three pairs of lines. Since the distance between the intersection point and the query point is <span class="tex-span">2</span>, the answer is three times that or <span class="tex-span">6</span>.</p>
