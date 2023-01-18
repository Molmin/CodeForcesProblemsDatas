## Description

<div><p>During the winter holidays, the demand for Christmas balls is exceptionally high. Since it's already <span class="tex-span">2018</span>, the advances in alchemy allow easy and efficient ball creation by utilizing magic crystals.</p><p>Grisha needs to obtain some yellow, green and blue balls. It's known that to produce a <span class="tex-font-style-bf">yellow</span> ball one needs two yellow crystals, <span class="tex-font-style-bf">green</span>&nbsp;— one yellow and one blue, and for a <span class="tex-font-style-bf">blue</span> ball, three blue crystals are enough.</p><p>Right now there are <span class="tex-span"><i>A</i></span> yellow and <span class="tex-span"><i>B</i></span> blue crystals in Grisha's disposal. Find out how many additional crystals he should acquire in order to produce the required number of balls.</p></div><div class="input-specification"><p>The first line features two integers <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> (<span class="tex-span">0 ≤ <i>A</i>, <i>B</i> ≤ 10<sup class="upper-index">9</sup></span>), denoting the number of yellow and blue crystals respectively at Grisha's disposal.</p><p>The next line contains three integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>z</i></span> (<span class="tex-span">0 ≤ <i>x</i>, <i>y</i>, <i>z</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the respective amounts of yellow, green and blue balls to be obtained.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the minimum number of crystals that Grisha should acquire in addition.</p></div>

## Input

<p>The first line features two integers <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> (<span class="tex-span">0 ≤ <i>A</i>, <i>B</i> ≤ 10<sup class="upper-index">9</sup></span>), denoting the number of yellow and blue crystals respectively at Grisha's disposal.</p><p>The next line contains three integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>z</i></span> (<span class="tex-span">0 ≤ <i>x</i>, <i>y</i>, <i>z</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the respective amounts of yellow, green and blue balls to be obtained.</p>

## Output

<p>Print a single integer&nbsp;— the minimum number of crystals that Grisha should acquire in addition.</p>





```input1
4 3
2 1 1

```




```input2
3 9
1 1 3

```




```input3
12345678 87654321
43043751 1000000000 53798715

```




```output1
2

```




```output2
1

```




```output3
2147483648

```



## Note

<p>In the first sample case, Grisha needs five yellow and four blue crystals to create two yellow balls, one green ball, and one blue ball. To do that, Grisha needs to obtain two additional crystals: one yellow and one blue.</p>
