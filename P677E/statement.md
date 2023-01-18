## Description

<div><p>Vanya plays a game of balloons on the field of size <span class="tex-span"><i>n</i> × <i>n</i></span>, where each cell contains a balloon with one of the values <span class="tex-span">0</span>, <span class="tex-span">1</span>, <span class="tex-span">2</span> or <span class="tex-span">3</span>. The goal is to destroy a cross, such that the product of all values of balloons in the cross is maximum possible. There are two types of crosses: normal and rotated. For example:</p><pre class="verbatim"><br>**o**<br>**o**<br>ooooo<br>**o**<br>**o**<br></pre><p>or</p><pre class="verbatim"><br>o***o<br>*o*o*<br>**o**<br>*o*o*<br>o***o<br></pre><p>Formally, the cross is given by three integers <span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>c</i></span> and <span class="tex-span"><i>d</i></span>, such that <span class="tex-span"><i>d</i> ≤ <i>r</i>, <i>c</i> ≤ <i>n</i> - <i>d</i> + 1</span>. The normal cross consists of balloons located in cells <span class="tex-span">(<i>x</i>, <i>y</i>)</span> (where <span class="tex-span"><i>x</i></span> stay for the number of the row and <span class="tex-span"><i>y</i></span> for the number of the column), such that <span class="tex-span">|<i>x</i> - <i>r</i>|·|<i>y</i> - <i>c</i>| = 0</span> and <span class="tex-span">|<i>x</i> - <i>r</i>| + |<i>y</i> - <i>c</i>| &lt; <i>d</i></span>. Rotated cross consists of balloons located in cells <span class="tex-span">(<i>x</i>, <i>y</i>)</span>, such that <span class="tex-span">|<i>x</i> - <i>r</i>| = |<i>y</i> - <i>c</i>|</span> and <span class="tex-span">|<i>x</i> - <i>r</i>| &lt; <i>d</i></span>.</p><p>Vanya wants to know the maximum possible product of the values of balls forming one cross. As this value can be large, output it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the number of rows and columns in the table with balloons.</p><p>The each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>n</i></span> characters '<span class="tex-font-style-tt">0</span>', '<span class="tex-font-style-tt">1</span>', '<span class="tex-font-style-tt">2</span>' or '<span class="tex-font-style-tt">3</span>'&nbsp;— the description of the values in balloons.</p></div><div class="output-specification"><p>Print the maximum possible product modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. Note, that you are not asked to maximize the remainder modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>, but to find the maximum value and print it this modulo.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the number of rows and columns in the table with balloons.</p><p>The each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>n</i></span> characters '<span class="tex-font-style-tt">0</span>', '<span class="tex-font-style-tt">1</span>', '<span class="tex-font-style-tt">2</span>' or '<span class="tex-font-style-tt">3</span>'&nbsp;— the description of the values in balloons.</p>

## Output

<p>Print the maximum possible product modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. Note, that you are not asked to maximize the remainder modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>, but to find the maximum value and print it this modulo.</p>





```input1
4
1233
0213
2020
0303

```




```input2
5
00300
00300
33333
00300
00300

```




```input3
5
00003
02030
00300
03020
30000

```




```input4
5
21312
10003
10002
10003
23231

```




```input5
5
12131
12111
12112
21311
21212

```




```output1
108

```




```output2
19683

```




```output3
108

```




```output4
3

```




```output5
24

```



## Note

<p>In the first sample, the maximum product is achieved for a rotated cross with a center in the cell <span class="tex-span">(3, 3)</span> and radius <span class="tex-span">1</span>: <span class="tex-span">2·2·3·3·3 = 108</span>.</p>
