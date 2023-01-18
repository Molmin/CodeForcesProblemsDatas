## Description

<div><p>A camera you have accidentally left in a desert has taken an interesting photo. The photo has a resolution of <span class="tex-span"><i>n</i></span> pixels width, and each column of this photo is all white or all black. Thus, we can represent the photo as a sequence of <span class="tex-span"><i>n</i></span> zeros and ones, where <span class="tex-span">0</span> means that the corresponding column is all white, and <span class="tex-span">1</span> means that the corresponding column is black.</p><p>You think that this photo can contain a zebra. In this case the whole photo should consist of several (possibly, only one) alternating black and white stripes of equal width. For example, the photo <span class="tex-span">[0, 0, 0, 1, 1, 1, 0, 0, 0]</span> can be a photo of zebra, while the photo <span class="tex-span">[0, 0, 0, 1, 1, 1, 1]</span> can not, because the width of the black stripe is <span class="tex-span">3</span>, while the width of the white stripe is <span class="tex-span">4</span>. Can the given photo be a photo of zebra or not?</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>) — the width of the photo.</p><p>The second line contains a sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>) — the description of the photo. If <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is zero, the <span class="tex-span"><i>i</i></span>-th column is all black. If <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is one, then the <span class="tex-span"><i>i</i></span>-th column is all white.</p></div><div class="output-specification"><p>If the photo can be a photo of zebra, print "<span class="tex-font-style-tt">YES</span>" (without quotes). Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p><p>You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>) — the width of the photo.</p><p>The second line contains a sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>) — the description of the photo. If <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is zero, the <span class="tex-span"><i>i</i></span>-th column is all black. If <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is one, then the <span class="tex-span"><i>i</i></span>-th column is all white.</p>

## Output

<p>If the photo can be a photo of zebra, print "<span class="tex-font-style-tt">YES</span>" (without quotes). Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p><p>You can print each letter in any case (upper or lower).</p>





```input1
9
0 0 0 1 1 1 0 0 0

```




```input2
7
0 0 0 1 1 1 1

```




```input3
5
1 1 1 1 1

```




```input4
8
1 1 1 0 0 0 1 1

```




```input5
9
1 1 0 1 1 0 1 1 0

```




```output1
YES

```




```output2
NO

```




```output3
YES

```




```output4
NO

```




```output5
NO

```



## Note

<p>The first two examples are described in the statements.</p><p>In the third example all pixels are white, so the photo can be a photo of zebra.</p><p>In the fourth example the width of the first stripe is equal to three (white color), the width of the second stripe is equal to three (black), and the width of the third stripe is equal to two (white). Thus, not all stripes have equal length, so this photo is not a photo of zebra.</p>
