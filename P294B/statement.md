## Description

<div><p>Shaass has <span class="tex-span"><i>n</i></span> books. He wants to make a bookshelf for all his books. He wants the bookshelf's dimensions to be as small as possible. The thickness of the <span class="tex-span"><i>i</i></span>-th book is <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and its pages' width is equal to <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>. The thickness of each book is either <span class="tex-span">1</span> or <span class="tex-span">2</span>. All books have the same page heights.</p><center> <img class="tex-graphics" src="file://uvbMf8VD.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Shaass puts the books on the bookshelf in the following way. First he selects some of the books and put them vertically. Then he puts the rest of the books horizontally above the vertical books. The sum of the widths of the horizontal books must be no more than the total thickness of the vertical books. A sample arrangement of the books is depicted in the figure.</p><center> <img class="tex-graphics" src="file://2w9zqAFi.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Help Shaass to find the minimum total thickness of the vertical books that we can achieve.</p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span>, <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span>. Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> denoting the thickness and width of the <span class="tex-span"><i>i</i></span>-th book correspondingly, (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2, 1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>).</p></div><div class="output-specification"><p>On the only line of the output print the minimum total thickness of the vertical books that we can achieve.</p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span>, <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span>. Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> denoting the thickness and width of the <span class="tex-span"><i>i</i></span>-th book correspondingly, (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2, 1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>).</p>

## Output

<p>On the only line of the output print the minimum total thickness of the vertical books that we can achieve.</p>





```input1
5
1 12
1 3
2 15
2 5
2 1

```




```input2
3
1 10
2 1
2 4

```




```output1
5

```




```output2
3

```


