## Description

<div><p>Julia is going to cook a chicken in the kitchen of her dormitory. To save energy, the stove in the kitchen automatically turns off after <span class="tex-span"><i>k</i></span> minutes after turning on.</p><p>During cooking, Julia goes to the kitchen every <span class="tex-span"><i>d</i></span> minutes and turns on the stove if it is turned off. While the cooker is turned off, it stays warm. The stove switches on and off instantly.</p><p>It is known that the chicken needs <span class="tex-span"><i>t</i></span> minutes to be cooked on the stove, if it is turned on, and <span class="tex-span">2<i>t</i></span> minutes, if it is turned off. You need to find out, how much time will Julia have to cook the chicken, if it is considered that the chicken is cooked evenly, with constant speed when the stove is turned on and at a constant speed when it is turned off.</p></div><div class="input-specification"><p>The single line contains three integers <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>d</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>k</i>, <i>d</i>, <i>t</i> ≤ 10<sup class="upper-index">18</sup></span>).</p></div><div class="output-specification"><p>Print a single number, the total time of cooking in minutes. The relative or absolute error must not exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p><p>Namely, let's assume that your answer is <span class="tex-span"><i>x</i></span> and the answer of the jury is <span class="tex-span"><i>y</i></span>. The checker program will consider your answer correct if <img align="middle" class="tex-formula" src="file://iqQxSmkd.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The single line contains three integers <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>d</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>k</i>, <i>d</i>, <i>t</i> ≤ 10<sup class="upper-index">18</sup></span>).</p>

## Output

<p>Print a single number, the total time of cooking in minutes. The relative or absolute error must not exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p><p>Namely, let's assume that your answer is <span class="tex-span"><i>x</i></span> and the answer of the jury is <span class="tex-span"><i>y</i></span>. The checker program will consider your answer correct if <img align="middle" class="tex-formula" src="file://iqQxSmkd.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
3 2 6

```




```input2
4 2 20

```




```output1
6.5

```




```output2
20.0

```



## Note

<p>In the first example, the chicken will be cooked for 3 minutes on the turned on stove, after this it will be cooked for <img align="middle" class="tex-formula" src="file://MQKLo8ej.png" style="max-width: 100.0%;max-height: 100.0%;">. Then the chicken will be cooked for one minute on a turned off stove, it will be cooked for <img align="middle" class="tex-formula" src="file://HFOgcgKX.png" style="max-width: 100.0%;max-height: 100.0%;">. Thus, after four minutes the chicken will be cooked for <img align="middle" class="tex-formula" src="file://IZGsZdAs.png" style="max-width: 100.0%;max-height: 100.0%;">. Before the fifth minute Julia will turn on the stove and after <span class="tex-span">2.5</span> minutes the chicken will be ready <img align="middle" class="tex-formula" src="file://5t4VCrxZ.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>In the second example, when the stove is turned off, Julia will immediately turn it on, so the stove will always be turned on and the chicken will be cooked in 20 minutes.</p>
