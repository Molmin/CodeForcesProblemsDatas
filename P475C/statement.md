## Description

<div><p>Rumors say that one of Kamal-ol-molk's paintings has been altered. A rectangular brush has been moved right and down on the painting.</p><p>Consider the painting as a <span class="tex-span"><i>n</i> × <i>m</i></span> rectangular grid. At the beginning an <span class="tex-span"><i>x</i> × <i>y</i></span> rectangular brush is placed somewhere in the frame, with edges parallel to the frame, (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i>, 1 ≤ <i>y</i> ≤ <i>m</i></span>). Then the brush is moved several times. Each time the brush is moved one unit right or down. The brush has been strictly inside the frame during the painting. The brush alters every cell it has covered at some moment.</p><p>You have found one of the old Kamal-ol-molk's paintings. You want to know if it's possible that it has been altered in described manner. If yes, you also want to know minimum possible area of the brush. </p></div><div class="input-specification"><p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>, (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>), denoting the height and width of the painting.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the painting. Each line has <span class="tex-span"><i>m</i></span> characters. Character '<span class="tex-font-style-tt">X</span>' denotes an altered cell, otherwise it's showed by '<span class="tex-font-style-tt">.</span>'. There will be at least one altered cell in the painting.</p></div><div class="output-specification"><p>Print the minimum area of the brush in a line, if the painting is possibly altered, otherwise print <span class="tex-span"> - 1</span>.</p></div>

## Input

<p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>, (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>), denoting the height and width of the painting.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the painting. Each line has <span class="tex-span"><i>m</i></span> characters. Character '<span class="tex-font-style-tt">X</span>' denotes an altered cell, otherwise it's showed by '<span class="tex-font-style-tt">.</span>'. There will be at least one altered cell in the painting.</p>

## Output

<p>Print the minimum area of the brush in a line, if the painting is possibly altered, otherwise print <span class="tex-span"> - 1</span>.</p>





```input1
4 4
XX..
XX..
XXXX
XXXX

```




```input2
4 4
....
.XXX
.XXX
....

```




```input3
4 5
XXXX.
XXXX.
.XX..
.XX..

```




```output1
4

```




```output2
2

```




```output3
-1

```


