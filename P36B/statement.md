## Description

<div><p>Ever since Kalevitch, a famous Berland abstractionist, heard of fractals, he made them the main topic of his canvases. Every morning the artist takes a piece of graph paper and starts with making a model of his future canvas. He takes a square as big as <span class="tex-span"><i>n</i> × <i>n</i></span> squares and paints some of them black. Then he takes a clean square piece of paper and paints the fractal using the following algorithm: </p><p>Step 1. The paper is divided into <span class="tex-span"><i>n</i><sup class="upper-index">2</sup></span> identical squares and some of them are painted black according to the model.</p><p>Step 2. Every square that remains white is divided into <span class="tex-span"><i>n</i><sup class="upper-index">2</sup></span> smaller squares and some of them are painted black according to the model.</p><p>Every following step repeats step 2.</p><center> <img class="tex-graphics" src="file://6cYL3Cy8.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Unfortunately, this tiresome work demands too much time from the painting genius. Kalevitch has been dreaming of making the process automatic to move to making 3D or even 4D fractals.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 3</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 5</span>), where <span class="tex-span"><i>k</i></span> is the amount of steps of the algorithm. Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>n</i></span> symbols that determine the model. Symbol «.» stands for a white square, whereas «*» stands for a black one. It is guaranteed that the model has at least one white square. </p></div><div class="output-specification"><p>Output a matrix <span class="tex-span"><i>n</i><sup class="upper-index"><i>k</i></sup> × <i>n</i><sup class="upper-index"><i>k</i></sup></span> which is what a picture should look like after <span class="tex-span"><i>k</i></span> steps of the algorithm.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 3</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 5</span>), where <span class="tex-span"><i>k</i></span> is the amount of steps of the algorithm. Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>n</i></span> symbols that determine the model. Symbol «.» stands for a white square, whereas «*» stands for a black one. It is guaranteed that the model has at least one white square. </p>

## Output

<p>Output a matrix <span class="tex-span"><i>n</i><sup class="upper-index"><i>k</i></sup> × <i>n</i><sup class="upper-index"><i>k</i></sup></span> which is what a picture should look like after <span class="tex-span"><i>k</i></span> steps of the algorithm.</p>





```input1
2 3
.*
..

```




```input2
3 2
.*.
***
.*.

```




```output1
.*******
..******
.*.*****
....****
.***.***
..**..**
.*.*.*.*
........

```




```output2
.*.***.*.
*********
.*.***.*.
*********
*********
*********
.*.***.*.
*********
.*.***.*.

```


