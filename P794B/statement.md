## Description

<div><p>Igor the analyst has adopted <span class="tex-span"><i>n</i></span> little bunnies. As we all know, bunnies love carrots. Thus, Igor has bought a carrot to be shared between his bunnies. Igor wants to treat all the bunnies equally, and thus he wants to cut the carrot into <span class="tex-span"><i>n</i></span> pieces of equal area. </p><p>Formally, the carrot can be viewed as an isosceles triangle with base length equal to <span class="tex-span">1</span> and height equal to <span class="tex-span"><i>h</i></span>. Igor wants to make <span class="tex-span"><i>n</i> - 1</span> cuts <span class="tex-font-style-bf">parallel to the base</span> to cut the carrot into <span class="tex-span"><i>n</i></span> pieces. He wants to make sure that all <span class="tex-span"><i>n</i></span> pieces have the same area. Can you help Igor determine where to cut the carrot so that each piece have equal area?</p><center> <img class="tex-graphics" height="454px" src="file://lk7FfCeN.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px"> <span class="tex-font-size-small">Illustration to the first example.</span> </center></div><div class="input-specification"><p>The first and only line of input contains two space-separated integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>h</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>h</i> ≤ 10<sup class="upper-index">5</sup></span>).</p></div><div class="output-specification"><p>The output should contain <span class="tex-span"><i>n</i> - 1</span> real numbers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i> - 1</sub></span>. The number <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> denotes that the <span class="tex-span"><i>i</i></span>-th cut must be made <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> units away from the apex of the carrot. In addition, <span class="tex-span">0 &lt; <i>x</i><sub class="lower-index">1</sub> &lt; <i>x</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>x</i><sub class="lower-index"><i>n</i> - 1</sub> &lt; <i>h</i></span> must hold. </p><p>Your output will be considered correct if absolute or relative error of every number in your output doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p><p>Formally, let your answer be <span class="tex-span"><i>a</i></span>, and the jury's answer be <span class="tex-span"><i>b</i></span>. Your answer is considered correct if <img align="middle" class="tex-formula" src="file://UPFceGms.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first and only line of input contains two space-separated integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>h</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>h</i> ≤ 10<sup class="upper-index">5</sup></span>).</p>

## Output

<p>The output should contain <span class="tex-span"><i>n</i> - 1</span> real numbers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i> - 1</sub></span>. The number <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> denotes that the <span class="tex-span"><i>i</i></span>-th cut must be made <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> units away from the apex of the carrot. In addition, <span class="tex-span">0 &lt; <i>x</i><sub class="lower-index">1</sub> &lt; <i>x</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>x</i><sub class="lower-index"><i>n</i> - 1</sub> &lt; <i>h</i></span> must hold. </p><p>Your output will be considered correct if absolute or relative error of every number in your output doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p><p>Formally, let your answer be <span class="tex-span"><i>a</i></span>, and the jury's answer be <span class="tex-span"><i>b</i></span>. Your answer is considered correct if <img align="middle" class="tex-formula" src="file://UPFceGms.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
3 2

```




```input2
2 100000

```




```output1
1.154700538379 1.632993161855

```




```output2
70710.678118654752

```



## Note

<p>Definition of isosceles triangle: <a href="https://en.wikipedia.org/wiki/Isosceles_triangle">https://en.wikipedia.org/wiki/Isosceles_triangle</a>.</p>
