## Description

<div><p>Gerald bought two very rare paintings at the Sotheby's auction and he now wants to hang them on the wall. For that he bought a special board to attach it to the wall and place the paintings on the board. The board has shape of an <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> × <i>b</i><sub class="lower-index">1</sub></span> rectangle, the paintings have shape of a <span class="tex-span"><i>a</i><sub class="lower-index">2</sub> × <i>b</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index">3</sub> × <i>b</i><sub class="lower-index">3</sub></span> rectangles.</p><p>Since the paintings are painted in the style of abstract art, it does not matter exactly how they will be rotated, but still, one side of both the board, and each of the paintings must be parallel to the floor. The paintings can touch each other and the edges of the board, but can not overlap or go beyond the edge of the board. Gerald asks whether it is possible to place the paintings on the board, or is the board he bought not large enough?</p></div><div class="input-specification"><p>The first line contains two space-separated numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span> — the sides of the board. Next two lines contain numbers <span class="tex-span"><i>a</i><sub class="lower-index">2</sub>, <i>b</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index">3</sub></span> — the sides of the paintings. All numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> in the input are integers and fit into the range from <span class="tex-span">1</span> to <span class="tex-span">1000</span>.</p></div><div class="output-specification"><p>If the paintings can be placed on the wall, print "<span class="tex-font-style-tt">YES</span>" (without the quotes), and if they cannot, print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p></div>

## Input

<p>The first line contains two space-separated numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span> — the sides of the board. Next two lines contain numbers <span class="tex-span"><i>a</i><sub class="lower-index">2</sub>, <i>b</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index">3</sub></span> — the sides of the paintings. All numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> in the input are integers and fit into the range from <span class="tex-span">1</span> to <span class="tex-span">1000</span>.</p>

## Output

<p>If the paintings can be placed on the wall, print "<span class="tex-font-style-tt">YES</span>" (without the quotes), and if they cannot, print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p>





```input1
3 2
1 3
2 1

```




```input2
5 5
3 3
3 3

```




```input3
4 2
2 3
1 2

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



## Note

<p>That's how we can place the pictures in the first test:</p><p><img class="tex-graphics" src="file://9c1gwj9i.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>And that's how we can do it in the third one.</p><p><img class="tex-graphics" src="file://Mqo418eK.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
