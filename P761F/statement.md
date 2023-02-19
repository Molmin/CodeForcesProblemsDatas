## Description

<div><p>Dasha decided to have a rest after solving the problem <span class="tex-span"><i>D</i></span> and began to look photos from previous competitions.</p><p>Let's call photos as the matrix with the size <span class="tex-span"><i>n</i> × <i>m</i></span>, which consists of lowercase English letters.</p><p>Some <span class="tex-span"><i>k</i></span> photos especially interested her, because they can be received from photo-template by painting a rectangular area in a certain color. Let's call such photos special. </p><center> <img class="tex-graphics" src="file://VaPWfCmZ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>More formally the <span class="tex-span"><i>i</i></span>-th special photo is received from the photo-template by replacing all characters on some rectangle with upper left corner of the cell with coordinates <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> and lower right corner in the cell with coordinates <span class="tex-span">(<i>c</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub>)</span> to the symbol <span class="tex-span"><i>e</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Dasha asks you to find the special photo so that the total distance from it to all other special photos is minimum. And calculate this distance.</p><p>Determine the distance between two photos as the sum of distances between all corresponding letters. The distance between two letters is the difference module of their positions in the alphabet. For example, the distance between letters '<span class="tex-font-style-tt">h</span>' and '<span class="tex-font-style-tt">m</span>' equals <span class="tex-span">|8 - 13| = 5</span>, because the letter '<span class="tex-font-style-tt">h</span>' is the 8-th in the alphabet, the letter '<span class="tex-font-style-tt">m</span>' is the 13-th.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">3</sup>, 1 ≤ <i>k</i> ≤ 3·10<sup class="upper-index">5</sup>)</span> — the number of strings in the photo-template, the number of columns and the number of special photos which are interesting for Dasha. </p><p>The next <span class="tex-span"><i>n</i></span> lines contains the string with <span class="tex-span"><i>m</i></span> length which consists of little Latin characters — the description of the photo-template.</p><p>Each of the next <span class="tex-span"><i>k</i></span> lines contains the description of the special photo in the following format, "<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>e</i><sub class="lower-index"><i>i</i></sub></span>" <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i>)</span>, where <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> — is the coordinate of the upper left corner of the rectangle, <span class="tex-span">(<i>c</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub>)</span> — is the description of the lower right corner, and <span class="tex-span"><i>e</i><sub class="lower-index"><i>i</i></sub></span> — is the little Latin letter which replaces the photo-template in the described rectangle. </p></div><div class="output-specification"><p>In the only line print the minimum total distance from the found special photo to all other special photos.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">3</sup>, 1 ≤ <i>k</i> ≤ 3·10<sup class="upper-index">5</sup>)</span> — the number of strings in the photo-template, the number of columns and the number of special photos which are interesting for Dasha. </p><p>The next <span class="tex-span"><i>n</i></span> lines contains the string with <span class="tex-span"><i>m</i></span> length which consists of little Latin characters — the description of the photo-template.</p><p>Each of the next <span class="tex-span"><i>k</i></span> lines contains the description of the special photo in the following format, "<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>e</i><sub class="lower-index"><i>i</i></sub></span>" <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i>)</span>, where <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> — is the coordinate of the upper left corner of the rectangle, <span class="tex-span">(<i>c</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub>)</span> — is the description of the lower right corner, and <span class="tex-span"><i>e</i><sub class="lower-index"><i>i</i></sub></span> — is the little Latin letter which replaces the photo-template in the described rectangle. </p>

## Output

<p>In the only line print the minimum total distance from the found special photo to all other special photos.</p>





```input1
3 3 2
aaa
aaa
aaa
1 1 2 2 b
2 2 3 3 c

```




```input2
5 5 3
abcde
eabcd
deabc
cdeab
bcdea
1 1 3 4 f
1 2 3 3 e
1 3 3 4 i

```




```output1
10

```




```output2
59

```



## Note

<p>In the first example the photos are following: </p><pre class="verbatim"><br>bba    aaa<br>bba    acc<br>aaa    acc<br></pre><p>The distance between them is <span class="tex-span">10</span>.</p>
