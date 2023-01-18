## Description

<div><p>The Easter Rabbit laid <span class="tex-span"><i>n</i></span> eggs in a circle and is about to paint them. </p><p>Each egg should be painted one color out of 7: red, orange, yellow, green, blue, indigo or violet. Also, the following conditions should be satisfied:</p><ul> <li> Each of the seven colors should be used to paint at least one egg. </li><li> Any four eggs <span class="tex-font-style-bf">lying sequentially</span> should be painted different colors. </li></ul><p>Help the Easter Rabbit paint the eggs in the required manner. We know that it is always possible.</p></div><div class="input-specification"><p>The only line contains an integer <span class="tex-span"><i>n</i></span> — the amount of eggs (<span class="tex-span">7 ≤ <i>n</i> ≤ 100</span>).</p></div><div class="output-specification"><p>Print one line consisting of <span class="tex-span"><i>n</i></span> characters. The <span class="tex-span"><i>i</i></span>-th character should describe the color of the <span class="tex-span"><i>i</i></span>-th egg in the order they lie in the circle. The colors should be represented as follows: "<span class="tex-font-style-tt">R</span>" stands for red, "<span class="tex-font-style-tt">O</span>" stands for orange, "<span class="tex-font-style-tt">Y</span>" stands for yellow, "<span class="tex-font-style-tt">G</span>" stands for green, "<span class="tex-font-style-tt">B</span>" stands for blue, "<span class="tex-font-style-tt">I</span>" stands for indigo, "<span class="tex-font-style-tt">V</span>" stands for violet.</p><p>If there are several answers, print any of them.</p></div>

## Input

<p>The only line contains an integer <span class="tex-span"><i>n</i></span> — the amount of eggs (<span class="tex-span">7 ≤ <i>n</i> ≤ 100</span>).</p>

## Output

<p>Print one line consisting of <span class="tex-span"><i>n</i></span> characters. The <span class="tex-span"><i>i</i></span>-th character should describe the color of the <span class="tex-span"><i>i</i></span>-th egg in the order they lie in the circle. The colors should be represented as follows: "<span class="tex-font-style-tt">R</span>" stands for red, "<span class="tex-font-style-tt">O</span>" stands for orange, "<span class="tex-font-style-tt">Y</span>" stands for yellow, "<span class="tex-font-style-tt">G</span>" stands for green, "<span class="tex-font-style-tt">B</span>" stands for blue, "<span class="tex-font-style-tt">I</span>" stands for indigo, "<span class="tex-font-style-tt">V</span>" stands for violet.</p><p>If there are several answers, print any of them.</p>





```input1
8

```




```input2
13

```




```output1
ROYGRBIV

```




```output2
ROYGBIVGBIVYG

```



## Note

<p>The way the eggs will be painted in the first sample is shown on the picture: </p><center> <img class="tex-graphics" src="file://WDh7dyOD.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
