## Description

<div><p>Nanami is an expert at playing games. This day, Nanami's good friend Hajime invited her to watch a game of baseball. Unwilling as she was, she followed him to the stadium. But Nanami had no interest in the game, so she looked around to see if there was something that might interest her. That's when she saw the digital board at one end of the stadium.</p><p>The digital board is <span class="tex-span"><i>n</i></span> pixels in height and <span class="tex-span"><i>m</i></span> pixels in width, every pixel is either light or dark. The pixels are described by its coordinate. The <span class="tex-span"><i>j</i></span>-th pixel of the <span class="tex-span"><i>i</i></span>-th line is pixel <span class="tex-span">(<i>i</i>, <i>j</i>)</span>. The board displays messages by switching a combination of pixels to light, and the rest to dark. Nanami notices that the state of the pixels on the board changes from time to time. At certain times, certain pixels on the board may switch from light to dark, or from dark to light.</p><p>Nanami wonders, what is the area of the biggest light block such that a specific pixel is on its side. A light block is a sub-rectangle of the board, in which all pixels are light. Pixel <span class="tex-span">(<i>i</i>, <i>j</i>)</span> belongs to a side of sub-rectangle with <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> and <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span> as its upper-left and lower-right vertex if and only if it satisfies the logical condition: </p><center>((<span class="tex-span"><i>i</i> = <i>x</i><sub class="lower-index">1</sub></span> or <span class="tex-span"><i>i</i> = <i>x</i><sub class="lower-index">2</sub></span>) and (<span class="tex-span"><i>y</i><sub class="lower-index">1</sub> ≤ <i>j</i> ≤ <i>y</i><sub class="lower-index">2</sub></span>)) or ((<span class="tex-span"><i>j</i> = <i>y</i><sub class="lower-index">1</sub></span> or <span class="tex-span"><i>j</i> = <i>y</i><sub class="lower-index">2</sub></span>) and (<span class="tex-span"><i>x</i><sub class="lower-index">1</sub> ≤ <i>i</i> ≤ <i>x</i><sub class="lower-index">2</sub></span>)).</center><p>Nanami has all the history of changing pixels, also she has some questions of the described type, can you answer them?</p></div><div class="input-specification"><p>The first line contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>q</i>&nbsp;(1 ≤ <i>n</i>, <i>m</i>, <i>q</i> ≤ 1000)</span> — the height and width of the digital board, and the number of operations.</p><p>Then follow <span class="tex-span"><i>n</i></span> lines, each line containing <span class="tex-span"><i>m</i></span> space-separated integers. The <span class="tex-span"><i>j</i></span>-th integer of the <span class="tex-span"><i>i</i></span>-th line is <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> — the initial state of pixel <span class="tex-span">(<i>i</i>, <i>j</i>)</span>.</p><ul> <li> If <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = 0</span>, pixel <span class="tex-span">(<i>i</i>, <i>j</i>)</span> is initially dark. </li><li> If <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = 1</span>, pixel <span class="tex-span">(<i>i</i>, <i>j</i>)</span> is initially light. </li></ul><p>Then follow <span class="tex-span"><i>q</i></span> lines, each line containing three space-separated integers <span class="tex-span"><i>op</i></span>, <span class="tex-span"><i>x</i></span>, and <span class="tex-span"><i>y</i>&nbsp;(1 ≤ <i>op</i> ≤ 2;&nbsp;1 ≤ <i>x</i> ≤ <i>n</i>;&nbsp;1 ≤ <i>y</i> ≤ <i>m</i>)</span>, describing an operation.</p><ul> <li> If <span class="tex-span"><i>op</i> = 1</span>, the pixel at <span class="tex-span">(<i>x</i>, <i>y</i>)</span> changes its state (from light to dark or from dark to light). </li><li> If <span class="tex-span"><i>op</i> = 2</span>, Nanami queries the biggest light block with pixel <span class="tex-span">(<i>x</i>, <i>y</i>)</span> on its side. </li></ul></div><div class="output-specification"><p>For each query, print a single line containing one integer — the answer to Nanami's query.</p></div>

## Input

<p>The first line contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>q</i>&nbsp;(1 ≤ <i>n</i>, <i>m</i>, <i>q</i> ≤ 1000)</span> — the height and width of the digital board, and the number of operations.</p><p>Then follow <span class="tex-span"><i>n</i></span> lines, each line containing <span class="tex-span"><i>m</i></span> space-separated integers. The <span class="tex-span"><i>j</i></span>-th integer of the <span class="tex-span"><i>i</i></span>-th line is <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> — the initial state of pixel <span class="tex-span">(<i>i</i>, <i>j</i>)</span>.</p><ul> <li> If <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = 0</span>, pixel <span class="tex-span">(<i>i</i>, <i>j</i>)</span> is initially dark. </li><li> If <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = 1</span>, pixel <span class="tex-span">(<i>i</i>, <i>j</i>)</span> is initially light. </li></ul><p>Then follow <span class="tex-span"><i>q</i></span> lines, each line containing three space-separated integers <span class="tex-span"><i>op</i></span>, <span class="tex-span"><i>x</i></span>, and <span class="tex-span"><i>y</i>&nbsp;(1 ≤ <i>op</i> ≤ 2;&nbsp;1 ≤ <i>x</i> ≤ <i>n</i>;&nbsp;1 ≤ <i>y</i> ≤ <i>m</i>)</span>, describing an operation.</p><ul> <li> If <span class="tex-span"><i>op</i> = 1</span>, the pixel at <span class="tex-span">(<i>x</i>, <i>y</i>)</span> changes its state (from light to dark or from dark to light). </li><li> If <span class="tex-span"><i>op</i> = 2</span>, Nanami queries the biggest light block with pixel <span class="tex-span">(<i>x</i>, <i>y</i>)</span> on its side. </li></ul>

## Output

<p>For each query, print a single line containing one integer — the answer to Nanami's query.</p>





```input1
3 4 5
0 1 1 0
1 0 0 1
0 1 1 0
2 2 2
2 1 2
1 2 2
1 2 3
2 2 2

```




```input2
3 3 4
1 1 1
1 1 1
1 1 1
2 2 2
1 2 2
2 1 1
2 2 1

```




```output1
0
2
6

```




```output2
6
3
3

```



## Note

<p>Consider the first sample.</p><p>The first query specifies pixel <span class="tex-span">(2, 2)</span>, which is dark itself, so there are no valid light blocks, thus the answer is 0.</p><p>The second query specifies pixel <span class="tex-span">(1, 2)</span>. The biggest light block is the block with <span class="tex-span">(1, 2)</span> as its upper-left vertex and <span class="tex-span">(1, 3)</span> as its lower-right vertex.</p><p>The last query specifies pixel <span class="tex-span">(2, 2)</span>, which became light in the third operation. The biggest light block is the block with <span class="tex-span">(1, 2)</span> as its upper-left vertex and <span class="tex-span">(3, 3)</span> as its lower-right vertex.</p>
