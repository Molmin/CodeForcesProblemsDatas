## Description

<div><p>Chubby Yang is studying linear equations right now. He came up with a nice problem. In the problem you are given an <span class="tex-span"><i>n</i> × <i>n</i></span> matrix <span class="tex-span"><i>W</i></span>, consisting of integers, and you should find two <span class="tex-span"><i>n</i> × <i>n</i></span> matrices <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span>, all the following conditions must hold: </p><ul> <li> <span class="tex-span"><i>A</i><sub class="lower-index"><i>ij</i></sub> = <i>A</i><sub class="lower-index"><i>ji</i></sub></span>, for all <span class="tex-span"><i>i</i>, <i>j</i></span> <span class="tex-span">(1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i>)</span>; </li><li> <span class="tex-span"><i>B</i><sub class="lower-index"><i>ij</i></sub> =  - <i>B</i><sub class="lower-index"><i>ji</i></sub></span>, for all <span class="tex-span"><i>i</i>, <i>j</i></span> <span class="tex-span">(1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i>)</span>; </li><li> <span class="tex-span"><i>W</i><sub class="lower-index"><i>ij</i></sub> = <i>A</i><sub class="lower-index"><i>ij</i></sub> + <i>B</i><sub class="lower-index"><i>ij</i></sub></span>, for all <span class="tex-span"><i>i</i>, <i>j</i></span> <span class="tex-span">(1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i>)</span>. </li></ul><p>Can you solve the problem?</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 170)</span>. Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>n</i></span> integers. The <span class="tex-span"><i>j</i></span>-th integer in the <span class="tex-span"><i>i</i></span>-th line is <span class="tex-span"><i>W</i><sub class="lower-index"><i>ij</i></sub></span> <span class="tex-span">(0 ≤ |<i>W</i><sub class="lower-index"><i>ij</i></sub>| &lt; 1717)</span>.</p></div><div class="output-specification"><p>The first <span class="tex-span"><i>n</i></span> lines must contain matrix <span class="tex-span"><i>A</i></span>. The next <span class="tex-span"><i>n</i></span> lines must contain matrix <span class="tex-span"><i>B</i></span>. Print the matrices in the format equal to format of matrix <span class="tex-span"><i>W</i></span> in input. It is guaranteed that the answer exists. If there are multiple answers, you are allowed to print any of them.</p><p>The answer will be considered correct if the absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 170)</span>. Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>n</i></span> integers. The <span class="tex-span"><i>j</i></span>-th integer in the <span class="tex-span"><i>i</i></span>-th line is <span class="tex-span"><i>W</i><sub class="lower-index"><i>ij</i></sub></span> <span class="tex-span">(0 ≤ |<i>W</i><sub class="lower-index"><i>ij</i></sub>| &lt; 1717)</span>.</p>

## Output

<p>The first <span class="tex-span"><i>n</i></span> lines must contain matrix <span class="tex-span"><i>A</i></span>. The next <span class="tex-span"><i>n</i></span> lines must contain matrix <span class="tex-span"><i>B</i></span>. Print the matrices in the format equal to format of matrix <span class="tex-span"><i>W</i></span> in input. It is guaranteed that the answer exists. If there are multiple answers, you are allowed to print any of them.</p><p>The answer will be considered correct if the absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p>





```input1
2
1 4
3 2

```




```input2
3
1 2 3
4 5 6
7 8 9

```




```output1
1.00000000 3.50000000
3.50000000 2.00000000
0.00000000 0.50000000
-0.50000000 0.00000000

```




```output2
1.00000000 3.00000000 5.00000000
3.00000000 5.00000000 7.00000000
5.00000000 7.00000000 9.00000000
0.00000000 -1.00000000 -2.00000000
1.00000000 0.00000000 -1.00000000
2.00000000 1.00000000 0.00000000

```


