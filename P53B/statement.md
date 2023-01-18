## Description

<div><p>One popular blog site edits the uploaded photos like this. It cuts a rectangular area out of them so that the ratio of height to width (i.e. the <span class="tex-span"><i>height</i> / <i>width</i></span> quotient) can vary from 0.8 to 1.25 inclusively. Besides, at least one side of the cut area should have a size, equal to some power of number 2 (<span class="tex-span">2<sup class="upper-index"><i>x</i></sup></span> for some integer <span class="tex-span"><i>x</i></span>). If those rules don't indicate the size of the cut are clearly, then the way with which the cut part possesses the largest area is chosen. Of course, both sides of the cut area should be integer. If there are several answers to this problem, you should choose the answer with the maximal height.</p></div><div class="input-specification"><p>The first line contains a pair of integers <span class="tex-span"><i>h</i></span> and <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>h</i>, <i>w</i> ≤ 10<sup class="upper-index">9</sup></span>) which are the height and width of the uploaded photo in pixels.</p></div><div class="output-specification"><p>Print two integers which are the height and width of the cut area.</p></div>

## Input

<p>The first line contains a pair of integers <span class="tex-span"><i>h</i></span> and <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>h</i>, <i>w</i> ≤ 10<sup class="upper-index">9</sup></span>) which are the height and width of the uploaded photo in pixels.</p>

## Output

<p>Print two integers which are the height and width of the cut area.</p>





```input1
2 1

```




```input2
2 2

```




```input3
5 5

```




```output1
1 1

```




```output2
2 2

```




```output3
5 4

```


