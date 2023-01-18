## Description

<div><p><span class="tex-font-style-it">Everything red frightens Nian the monster. So do red paper and... you, red on Codeforces, potential or real.</span></p><p>Big Banban has got a piece of paper with endless lattice points, where lattice points form squares with the same area. His most favorite closed shape is the circle because of its beauty and simplicity. Once he had obtained this piece of paper, he prepares it for paper-cutting.</p><center> <img class="tex-graphics" src="file://xUjP047k.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>He drew <span class="tex-span"><i>n</i></span> concentric circles on it and numbered these circles from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> such that the center of each circle is the same lattice point and the radius of the <span class="tex-span"><i>k</i></span>-th circle is <img align="middle" class="tex-formula" src="file://fcRDFRMp.png" style="max-width: 100.0%;max-height: 100.0%;"> times the length of a lattice edge.</p><p>Define the degree of beauty of a lattice point as the summation of the <span class="tex-font-style-bf">indices</span> of circles such that this lattice point is inside them, or on their bounds. Banban wanted to ask you the total degree of beauty of all the lattice points, but changed his mind.</p><p>Defining the total degree of beauty of all the lattice points on a piece of paper with <span class="tex-span"><i>n</i></span> circles as <span class="tex-span"><i>f</i>(<i>n</i>)</span>, you are asked to figure out <img align="middle" class="tex-formula" src="file://Za8TLc0Z.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">12</sup>)</span>.</p></div><div class="output-specification"><p>In the first line print one integer representing <img align="middle" class="tex-formula" src="file://rx0NqNaD.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">12</sup>)</span>.</p>

## Output

<p>In the first line print one integer representing <img align="middle" class="tex-formula" src="file://rx0NqNaD.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
5

```




```input2
233

```




```output1
387

```




```output2
788243189

```



## Note

<p>A piece of paper with <span class="tex-span">5</span> circles is shown in the following.</p><center> <img class="tex-graphics" src="file://G8MN52bl.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>There are <span class="tex-span">5</span> types of lattice points where the degree of beauty of each red point is <span class="tex-span">1 + 2 + 3 + 4 + 5 = 15</span>, the degree of beauty of each orange point is <span class="tex-span">2 + 3 + 4 + 5 = 14</span>, the degree of beauty of each green point is <span class="tex-span">4 + 5 = 9</span>, the degree of beauty of each blue point is <span class="tex-span">5</span> and the degree of beauty of each gray point is <span class="tex-span">0</span>. Therefore, <span class="tex-span"><i>f</i>(5) = 5·15 + 4·14 + 4·9 + 8·5 = 207</span>.</p><p>Similarly, <span class="tex-span"><i>f</i>(1) = 5, <i>f</i>(2) = 23, <i>f</i>(3) = 50, <i>f</i>(4) = 102</span> and consequently <img align="middle" class="tex-formula" src="file://uMaFrEKY.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
