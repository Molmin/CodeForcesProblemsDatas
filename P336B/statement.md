## Description

<div><p>One beautiful day Vasily the bear painted <span class="tex-span">2<i>m</i></span> circles of the same radius <span class="tex-span"><i>R</i></span> on a coordinate plane. Circles with numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> had centers at points <span class="tex-span">(2<i>R</i> - <i>R</i>, 0)</span>, <span class="tex-span">(4<i>R</i> - <i>R</i>, 0)</span>, <span class="tex-span">...</span>, <span class="tex-span">(2<i>Rm</i> - <i>R</i>, 0)</span>, respectively. Circles with numbers from <span class="tex-span"><i>m</i> + 1</span> to <span class="tex-span">2<i>m</i></span> had centers at points <span class="tex-span">(2<i>R</i> - <i>R</i>, 2<i>R</i>)</span>, <span class="tex-span">(4<i>R</i> - <i>R</i>, 2<i>R</i>)</span>, <span class="tex-span">...</span>, <span class="tex-span">(2<i>Rm</i> - <i>R</i>, 2<i>R</i>)</span>, respectively. </p><p>Naturally, the bear painted the circles for a simple experiment with a fly. The experiment continued for <span class="tex-span"><i>m</i><sup class="upper-index">2</sup></span> days. Each day of the experiment got its own unique number from <span class="tex-span">0</span> to <span class="tex-span"><i>m</i><sup class="upper-index">2</sup> - 1</span>, inclusive. </p><p>On the day number <span class="tex-span"><i>i</i></span> the following things happened: </p><ol> <li> The fly arrived at the coordinate plane at the center of the circle with number <img align="middle" class="tex-formula" src="file://Ue9eGhrK.png" style="max-width: 100.0%;max-height: 100.0%;"> (<img align="middle" class="tex-formula" src="file://zs6bsM90.png" style="max-width: 100.0%;max-height: 100.0%;"> is the result of dividing number <span class="tex-span"><i>x</i></span> by number <span class="tex-span"><i>y</i></span>, rounded down to an integer). </li><li> The fly went along the coordinate plane to the center of the circle number <img align="middle" class="tex-formula" src="file://SXWCx0sF.png" style="max-width: 100.0%;max-height: 100.0%;"> (<img align="middle" class="tex-formula" src="file://kZQjIsW9.png" style="max-width: 100.0%;max-height: 100.0%;"> is the remainder after dividing number <span class="tex-span"><i>x</i></span> by number <span class="tex-span"><i>y</i></span>). The bear noticed that the fly went from the center of circle <span class="tex-span"><i>v</i></span> to the center of circle <span class="tex-span"><i>u</i></span> along the shortest path with all points lying on the border or inside at least one of the <span class="tex-span">2<i>m</i></span> circles. After the fly reached the center of circle <span class="tex-span"><i>u</i></span>, it flew away in an unknown direction. </li></ol><p>Help Vasily, count the average distance the fly went along the coordinate plane during each of these <span class="tex-span"><i>m</i><sup class="upper-index">2</sup></span> days.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>m</i>, <i>R</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>R</i> ≤ 10</span>).</p></div><div class="output-specification"><p>In a single line print a single real number — the answer to the problem. The answer will be considered correct if its absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>m</i>, <i>R</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>R</i> ≤ 10</span>).</p>

## Output

<p>In a single line print a single real number — the answer to the problem. The answer will be considered correct if its absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
1 1

```




```input2
2 2

```




```output1
2.0000000000

```




```output2
5.4142135624

```



## Note

<p><img class="tex-graphics" src="file://7CuTKS23.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p><span class="tex-font-size-script">Figure to the second sample</span></p>
