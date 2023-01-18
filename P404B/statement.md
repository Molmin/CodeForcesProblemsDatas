## Description

<div><p>Valera takes part in the Berland Marathon. The marathon race starts at the stadium that can be represented on the plane as a square whose lower left corner is located at point with coordinates <span class="tex-span">(0, 0)</span> and the length of the side equals <span class="tex-span"><i>a</i></span> meters. The sides of the square are parallel to coordinate axes.</p><p>As the length of the marathon race is very long, Valera needs to have extra drink during the race. The coach gives Valera a bottle of drink each <span class="tex-span"><i>d</i></span> meters of the path. We know that Valera starts at the point with coordinates <span class="tex-span">(0, 0)</span> and runs counter-clockwise. That is, when Valera covers <span class="tex-span"><i>a</i></span> meters, he reaches the point with coordinates <span class="tex-span">(<i>a</i>, 0)</span>. We also know that the length of the marathon race equals <span class="tex-span"><i>nd</i> + 0.5</span> meters. </p><p>Help Valera's coach determine where he should be located to help Valera. Specifically, determine the coordinates of Valera's positions when he covers <span class="tex-span"><i>d</i>, 2·<i>d</i>, ..., <i>n</i>·<i>d</i></span> meters.</p></div><div class="input-specification"><p>The first line contains two space-separated real numbers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>d</i></span> <span class="tex-span">(1 ≤ <i>a</i>, <i>d</i> ≤ 10<sup class="upper-index">5</sup>)</span>, given with precision till <span class="tex-span">4</span> decimal digits after the decimal point. Number <span class="tex-span"><i>a</i></span> denotes the length of the square's side that describes the stadium. Number <span class="tex-span"><i>d</i></span> shows that after each <span class="tex-span"><i>d</i></span> meters Valera gets an extra drink.</p><p>The second line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> showing that Valera needs an extra drink <span class="tex-span"><i>n</i></span> times.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> lines, each line should contain two real numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, separated by a space. Numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> in the <span class="tex-span"><i>i</i></span>-th line mean that Valera is at point with coordinates <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> after he covers <span class="tex-span"><i>i</i>·<i>d</i></span> meters. Your solution will be considered correct if the absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p><p>Note, that this problem have huge amount of output data. Please, do not use cout stream for output in this problem.</p></div>

## Input

<p>The first line contains two space-separated real numbers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>d</i></span> <span class="tex-span">(1 ≤ <i>a</i>, <i>d</i> ≤ 10<sup class="upper-index">5</sup>)</span>, given with precision till <span class="tex-span">4</span> decimal digits after the decimal point. Number <span class="tex-span"><i>a</i></span> denotes the length of the square's side that describes the stadium. Number <span class="tex-span"><i>d</i></span> shows that after each <span class="tex-span"><i>d</i></span> meters Valera gets an extra drink.</p><p>The second line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> showing that Valera needs an extra drink <span class="tex-span"><i>n</i></span> times.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> lines, each line should contain two real numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, separated by a space. Numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> in the <span class="tex-span"><i>i</i></span>-th line mean that Valera is at point with coordinates <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> after he covers <span class="tex-span"><i>i</i>·<i>d</i></span> meters. Your solution will be considered correct if the absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p><p>Note, that this problem have huge amount of output data. Please, do not use cout stream for output in this problem.</p>





```input1
2 5
2

```




```input2
4.147 2.8819
6

```




```output1
1.0000000000 2.0000000000
2.0000000000 0.0000000000

```




```output2
2.8819000000 0.0000000000
4.1470000000 1.6168000000
3.7953000000 4.1470000000
0.9134000000 4.1470000000
0.0000000000 2.1785000000
0.7034000000 0.0000000000

```


