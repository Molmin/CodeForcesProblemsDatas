## Description

<div><p>Have you ever tasted Martian food? Well, you should.</p><p>Their signature dish is served on a completely black plate with the radius of <span class="tex-span"><i>R</i></span>, flat as a pancake.</p><p>First, they put a perfectly circular portion of the Golden Honduras on the plate. It has the radius of <span class="tex-span"><i>r</i></span> and is located as close to the edge of the plate as possible staying entirely within the plate. I. e. Golden Honduras touches the edge of the plate from the inside. It is believed that the proximity of the portion of the Golden Honduras to the edge of a plate demonstrates the neatness and exactness of the Martians.</p><p>Then a perfectly round portion of Pink Guadeloupe is put on the plate. The Guadeloupe should not overlap with Honduras, should not go beyond the border of the plate, but should have the maximum radius. I. e. Pink Guadeloupe should touch the edge of the plate from the inside, and touch Golden Honduras from the outside. For it is the size of the Rose Guadeloupe that shows the generosity and the hospitality of the Martians.</p><p>Further, the first portion (of the same perfectly round shape) of Green Bull Terrier is put on the plate. It should come in contact with Honduras and Guadeloupe, should not go beyond the border of the plate and should have maximum radius.</p><p>Each of the following portions of the Green Bull Terrier must necessarily touch the Golden Honduras, the previous portion of the Green Bull Terrier and touch the edge of a plate, but should not go beyond the border.</p><p>To determine whether a stranger is worthy to touch the food, the Martians ask him to find the radius of the <span class="tex-span"><i>k</i></span>-th portion of the Green Bull Terrier knowing the radii of a plate and a portion of the Golden Honduras. And are you worthy?</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 10<sup class="upper-index">4</sup></span>) — amount of testcases.</p><p>Each of the following <span class="tex-span"><i>t</i></span> lines contain three positive integers: the radii of the plate and a portion of the Golden Honduras <span class="tex-span"><i>R</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>r</i> &lt; <i>R</i> ≤ 10<sup class="upper-index">4</sup></span>) and the number <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">4</sup></span>).</p><p>In the pretests <span class="tex-span">1 ≤ <i>k</i> ≤ 2</span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>t</i></span> lines — the radius of the <span class="tex-span"><i>k</i></span>-th portion of the Green Bull Terrier for each test. The absolute or relative error of the answer should not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 10<sup class="upper-index">4</sup></span>) — amount of testcases.</p><p>Each of the following <span class="tex-span"><i>t</i></span> lines contain three positive integers: the radii of the plate and a portion of the Golden Honduras <span class="tex-span"><i>R</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>r</i> &lt; <i>R</i> ≤ 10<sup class="upper-index">4</sup></span>) and the number <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">4</sup></span>).</p><p>In the pretests <span class="tex-span">1 ≤ <i>k</i> ≤ 2</span>.</p>

## Output

<p>Print <span class="tex-span"><i>t</i></span> lines — the radius of the <span class="tex-span"><i>k</i></span>-th portion of the Green Bull Terrier for each test. The absolute or relative error of the answer should not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
2
4 3 1
4 2 2

```




```output1
0.9230769231
0.6666666667

```



## Note

<p>Dish from the first sample looks like this:</p><p><img class="tex-graphics" src="file://BxFwEuX9.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Dish from the second sample looks like this:</p><p><img class="tex-graphics" src="file://guwXHi3E.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
