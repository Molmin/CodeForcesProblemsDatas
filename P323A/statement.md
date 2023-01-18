## Description

<div><p>You are given a cube of size <span class="tex-span"><i>k</i> × <i>k</i> × <i>k</i></span>, which consists of unit cubes. Two unit cubes are considered neighbouring, if they have common face.</p><p>Your task is to paint each of <span class="tex-span"><i>k</i><sup class="upper-index">3</sup></span> unit cubes one of two colours (black or white), so that the following conditions must be satisfied:</p><ul> <li> each white cube has exactly 2 neighbouring cubes of white color; </li><li> each black cube has exactly 2 neighbouring cubes of black color. </li></ul></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ 100)</span>, which is size of the cube.</p></div><div class="output-specification"><p>Print -1 if there is no solution. Otherwise, print the required painting of the cube consequently by layers. Print a <span class="tex-span"><i>k</i> × <i>k</i></span> matrix in the first <span class="tex-span"><i>k</i></span> lines, showing how the first layer of the cube should be painted. In the following <span class="tex-span"><i>k</i></span> lines print a <span class="tex-span"><i>k</i> × <i>k</i></span> matrix — the way the second layer should be painted. And so on to the last <span class="tex-span"><i>k</i></span>-th layer. Note that orientation of the cube in the space does not matter.</p><p>Mark a white unit cube with symbol "<span class="tex-font-style-tt">w</span>" and a black one with "<span class="tex-font-style-tt">b</span>". Use the format of output data, given in the test samples. You may print extra empty lines, they will be ignored.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ 100)</span>, which is size of the cube.</p>

## Output

<p>Print -1 if there is no solution. Otherwise, print the required painting of the cube consequently by layers. Print a <span class="tex-span"><i>k</i> × <i>k</i></span> matrix in the first <span class="tex-span"><i>k</i></span> lines, showing how the first layer of the cube should be painted. In the following <span class="tex-span"><i>k</i></span> lines print a <span class="tex-span"><i>k</i> × <i>k</i></span> matrix — the way the second layer should be painted. And so on to the last <span class="tex-span"><i>k</i></span>-th layer. Note that orientation of the cube in the space does not matter.</p><p>Mark a white unit cube with symbol "<span class="tex-font-style-tt">w</span>" and a black one with "<span class="tex-font-style-tt">b</span>". Use the format of output data, given in the test samples. You may print extra empty lines, they will be ignored.</p>





```input1
1

```




```input2
2

```




```output1
-1

```




```output2
bb
ww

bb
ww

```


