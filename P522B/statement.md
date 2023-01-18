## Description

<div><p>One day <span class="tex-span"><i>n</i></span> friends met at a party, they hadn't seen each other for a long time and so they decided to make a group photo together. </p><p>Simply speaking, the process of taking photos can be described as follows. On the photo, each photographed friend occupies a rectangle of pixels: the <span class="tex-span"><i>i</i></span>-th of them occupies the rectangle of width <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> pixels and height <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> pixels. On the group photo everybody stands in a line, thus the minimum pixel size of the photo including all the photographed friends, is <span class="tex-span"><i>W</i> × <i>H</i></span>, where <span class="tex-span"><i>W</i></span> is the total sum of all widths and <span class="tex-span"><i>H</i></span> is the maximum height of all the photographed friends.</p><p>As is usually the case, the friends made <span class="tex-span"><i>n</i></span> photos — the <span class="tex-span"><i>j</i></span>-th (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>n</i></span>) photo had everybody except for the <span class="tex-span"><i>j</i></span>-th friend as he was the photographer.</p><p>Print the minimum size of each made photo in pixels. </p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200 000</span>) — the number of friends. </p><p>Then <span class="tex-span"><i>n</i></span> lines follow: the <span class="tex-span"><i>i</i></span>-th line contains information about the <span class="tex-span"><i>i</i></span>-th friend. The line contains a pair of integers <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub>, <i>h</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10, 1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — the width and height in pixels of the corresponding rectangle.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> space-separated numbers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> — the total number of pixels on the minimum photo containing all friends expect for the <span class="tex-span"><i>i</i></span>-th one.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200 000</span>) — the number of friends. </p><p>Then <span class="tex-span"><i>n</i></span> lines follow: the <span class="tex-span"><i>i</i></span>-th line contains information about the <span class="tex-span"><i>i</i></span>-th friend. The line contains a pair of integers <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub>, <i>h</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10, 1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — the width and height in pixels of the corresponding rectangle.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> space-separated numbers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> — the total number of pixels on the minimum photo containing all friends expect for the <span class="tex-span"><i>i</i></span>-th one.</p>





```input1
3
1 10
5 5
10 1

```




```input2
3
2 1
1 2
2 1

```




```output1
75 110 60
```




```output2
6 4 6
```


