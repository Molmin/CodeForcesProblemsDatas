## Description

<div><p>Even polar bears feel cold when lying on the ice. Therefore, a polar bear Alice is going to make a carpet. The carpet can be viewed as a grid with height <span class="tex-span"><i>h</i></span> and width <span class="tex-span"><i>w</i></span>. Then the grid is divided into <span class="tex-span"><i>h</i> × <i>w</i></span> squares. Alice is going to assign one of <span class="tex-span"><i>k</i></span> different colors to each square. The colors are numbered from 1 to <span class="tex-span"><i>k</i></span>. She may choose not to use all of the colors.</p><p>However, there are some restrictions. For every two adjacent squares (squares that shares an edge) <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>, there is a <span class="tex-font-style-it">color constraint</span> in one of the forms: </p><ul> <li> <span class="tex-span"><i>color</i>(<i>x</i>) = <i>color</i>(<i>y</i>)</span>, or </li><li> <span class="tex-span"><i>color</i>(<i>x</i>) ≠ <i>color</i>(<i>y</i>)</span>. </li></ul><p>Example of the color constraints:</p><center> <img class="tex-graphics" src="file://ComeEQeL.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Ideally, Alice wants to satisfy all color constraints. But again, life in the Arctic is hard. It is not always possible to satisfy all color constraints. Fortunately, she will still be happy if at least <img align="middle" class="tex-formula" src="file://ERVjzQem.png" style="max-width: 100.0%;max-height: 100.0%;"> of the color constraints are satisfied. </p><p>If she has <span class="tex-span">4</span> colors she can color the carpet in the following way:</p><center> <img class="tex-graphics" src="file://acr6OIKs.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>And she is happy because <img align="middle" class="tex-formula" src="file://QctiMZgv.png" style="max-width: 100.0%;max-height: 100.0%;"> of the color constraints are satisfied, and <img align="middle" class="tex-formula" src="file://wcuzB8ez.png" style="max-width: 100.0%;max-height: 100.0%;">. Your task is to help her color the carpet.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>h</i>, <i>w</i>, <i>k</i></span> <span class="tex-span">(2 ≤ <i>h</i>, <i>w</i> ≤ 1000, 1 ≤ <i>k</i> ≤ <i>w</i>·<i>h</i>)</span>.</p><p>The next <span class="tex-span">2<i>h</i> - 1</span> lines describe the color constraints from top to bottom, left to right. They contain <span class="tex-span"><i>w</i> - 1, <i>w</i>, <i>w</i> - 1, <i>w</i>, ..., <i>w</i> - 1</span> characters respectively. Each color constraint is represented by a character "<span class="tex-font-style-tt">E</span>" or "<span class="tex-font-style-tt">N</span>", where "<span class="tex-font-style-tt">E</span>" means "<span class="tex-span"> = </span>" and "<span class="tex-font-style-tt">N</span>" means "<span class="tex-span"> ≠ </span>".</p><p>The color constraints listed in the order they are depicted on the picture.</p></div><div class="output-specification"><p>If there is a coloring that satisfies at least <img align="middle" class="tex-formula" src="file://tNNnNGuQ.png" style="max-width: 100.0%;max-height: 100.0%;"> of the color constraints, print "<span class="tex-font-style-tt">YES</span>" (without quotes) in the first line. In each of the next <span class="tex-span"><i>h</i></span> lines, print <span class="tex-span"><i>w</i></span> integers describing the coloring.</p><p>Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>h</i>, <i>w</i>, <i>k</i></span> <span class="tex-span">(2 ≤ <i>h</i>, <i>w</i> ≤ 1000, 1 ≤ <i>k</i> ≤ <i>w</i>·<i>h</i>)</span>.</p><p>The next <span class="tex-span">2<i>h</i> - 1</span> lines describe the color constraints from top to bottom, left to right. They contain <span class="tex-span"><i>w</i> - 1, <i>w</i>, <i>w</i> - 1, <i>w</i>, ..., <i>w</i> - 1</span> characters respectively. Each color constraint is represented by a character "<span class="tex-font-style-tt">E</span>" or "<span class="tex-font-style-tt">N</span>", where "<span class="tex-font-style-tt">E</span>" means "<span class="tex-span"> = </span>" and "<span class="tex-font-style-tt">N</span>" means "<span class="tex-span"> ≠ </span>".</p><p>The color constraints listed in the order they are depicted on the picture.</p>

## Output

<p>If there is a coloring that satisfies at least <img align="middle" class="tex-formula" src="file://tNNnNGuQ.png" style="max-width: 100.0%;max-height: 100.0%;"> of the color constraints, print "<span class="tex-font-style-tt">YES</span>" (without quotes) in the first line. In each of the next <span class="tex-span"><i>h</i></span> lines, print <span class="tex-span"><i>w</i></span> integers describing the coloring.</p><p>Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p>





```input1
3 4 4
ENE
NNEE
NEE
ENEN
ENN

```




```output1
YES
1 1 2 2
3 4 1 1
3 3 2 4
```


