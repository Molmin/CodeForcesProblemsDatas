## Description

<div><p>Many years have passed, and <span class="tex-span"><i>n</i></span> friends met at a party again. Technologies have leaped forward since the last meeting, cameras with timer appeared and now it is not obligatory for one of the friends to stand with a camera, and, thus, being absent on the photo.</p><p>Simply speaking, the process of photographing can be described as follows. Each friend occupies a rectangle of pixels on the photo: the <span class="tex-span"><i>i</i></span>-th of them in a standing state occupies a <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> pixels wide and a <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> pixels high rectangle. But also, each person can lie down for the photo, and then he will occupy a <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> pixels wide and a <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> pixels high rectangle.</p><p>The total photo will have size <span class="tex-span"><i>W</i> × <i>H</i></span>, where <span class="tex-span"><i>W</i></span> is the total width of all the people rectangles, and <span class="tex-span"><i>H</i></span> is the maximum of the heights. The friends want to determine what minimum area the group photo can they obtain if no more than <span class="tex-span"><i>n</i> / 2</span> of them can lie on the ground (it would be strange if more than <span class="tex-span"><i>n</i> / 2</span> gentlemen lie on the ground together, isn't it?..)</p><p>Help them to achieve this goal.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — the number of friends.</p><p>The next <span class="tex-span"><i>n</i></span> lines have two integers <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub>, <i>h</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub>, <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) each, representing the size of the rectangle, corresponding to the <span class="tex-span"><i>i</i></span>-th friend.</p></div><div class="output-specification"><p>Print a single integer equal to the minimum possible area of the photo containing all friends if no more than <span class="tex-span"><i>n</i> / 2</span> of them can lie on the ground.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — the number of friends.</p><p>The next <span class="tex-span"><i>n</i></span> lines have two integers <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub>, <i>h</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub>, <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) each, representing the size of the rectangle, corresponding to the <span class="tex-span"><i>i</i></span>-th friend.</p>

## Output

<p>Print a single integer equal to the minimum possible area of the photo containing all friends if no more than <span class="tex-span"><i>n</i> / 2</span> of them can lie on the ground.</p>





```input1
3
10 1
20 2
30 3

```




```input2
3
3 1
2 2
4 3

```




```input3
1
5 10

```




```output1
180

```




```output2
21

```




```output3
50

```


