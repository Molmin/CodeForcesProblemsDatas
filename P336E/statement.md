## Description

<div><p>Vasily the bear has two favorite integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> and a pencil. Besides, he's got <span class="tex-span"><i>k</i></span> jars with different water color paints. All jars are numbered in some manner from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i></span>, inclusive. The jar number <span class="tex-span"><i>i</i></span> contains the paint of the <span class="tex-span"><i>i</i></span>-th color. </p><p>Initially the bear took a pencil and drew four segments on the coordinate plane. All of them end at point <span class="tex-span">(0, 0)</span>. They begin at: <span class="tex-span">(0, 2<sup class="upper-index"><i>n</i></sup>)</span>, <span class="tex-span">(0,  - 2<sup class="upper-index"><i>n</i></sup>)</span>, <span class="tex-span">(2<sup class="upper-index"><i>n</i></sup>, 0)</span>, <span class="tex-span">( - 2<sup class="upper-index"><i>n</i></sup>, 0)</span>. Then for each <span class="tex-span"><i>i</i> = 1, 2, ..., <i>n</i></span>, the bear drew two squares. The first square has the following vertex coordinates: <span class="tex-span">(2<sup class="upper-index"><i>i</i></sup>, 0)</span>, <span class="tex-span">( - 2<sup class="upper-index"><i>i</i></sup>, 0)</span>, <span class="tex-span">(0,  - 2<sup class="upper-index"><i>i</i></sup>)</span>, <span class="tex-span">(0, 2<sup class="upper-index"><i>i</i></sup>)</span>. The second square has the following vertex coordinates: <span class="tex-span">( - 2<sup class="upper-index"><i>i</i> - 1</sup>,  - 2<sup class="upper-index"><i>i</i> - 1</sup>)</span>, <span class="tex-span">( - 2<sup class="upper-index"><i>i</i> - 1</sup>, 2<sup class="upper-index"><i>i</i> - 1</sup>)</span>, <span class="tex-span">(2<sup class="upper-index"><i>i</i> - 1</sup>,  - 2<sup class="upper-index"><i>i</i> - 1</sup>)</span>, <span class="tex-span">(2<sup class="upper-index"><i>i</i> - 1</sup>, 2<sup class="upper-index"><i>i</i> - 1</sup>)</span>. After that, the bear drew another square: <span class="tex-span">(1, 0)</span>, <span class="tex-span">( - 1, 0)</span>, <span class="tex-span">(0,  - 1)</span>, <span class="tex-span">(0, 1)</span>. All points mentioned above form the set of points <span class="tex-span"><i>A</i></span>.</p><p><img class="tex-graphics" src="file://omHsRk13.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p><span class="tex-font-size-script">The sample of the final picture at <span class="tex-span"><i>n</i> = 0</span></span></p><p><img class="tex-graphics" src="file://6hkzRAHD.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p><span class="tex-font-size-script">The sample of the final picture at <span class="tex-span"><i>n</i> = 2</span></span></p><p>The bear decided to paint the resulting picture in <span class="tex-span"><i>k</i></span> moves. The <span class="tex-span"><i>i</i></span>-th move consists of the following stages: </p><ol> <li> The bear chooses 3 distinct points in set <span class="tex-span"><i>А</i></span> so that any pair of the chosen points has a segment on the picture between them. The chosen points and segments mark the area that mustn't contain any previously painted points. </li><li> The bear paints the area bounded by the chosen points and segments the <span class="tex-span"><i>i</i></span>-th color. </li></ol><p>Note that after the <span class="tex-span"><i>k</i></span>-th move some parts of the picture can stay unpainted.</p><p>The bear asked you to calculate, how many distinct ways there are to paint his picture. A way to paint the picture is a sequence of three-element sets of points he chose on each step. Two sequences are considered distinct if there is such number <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>k</i>)</span>, that the <span class="tex-span"><i>i</i></span>-th members of these sequences do not coincide as sets. As the sought number can be rather large, you only need to calculate the remainder after dividing it by number <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span>, separated by a space (<span class="tex-span">0 ≤ <i>n</i>, <i>k</i> ≤ 200</span>).</p></div><div class="output-specification"><p>Print exactly one integer — the answer to the problem modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span>, separated by a space (<span class="tex-span">0 ≤ <i>n</i>, <i>k</i> ≤ 200</span>).</p>

## Output

<p>Print exactly one integer — the answer to the problem modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p>





```input1
0 0

```




```input2
0 1

```




```input3
0 2

```




```input4
1 1

```




```output1
1

```




```output2
8

```




```output3
32

```




```output4
32

```


