## Description

<div><p>Qwerty the Ranger arrived to the Diatar system with a very important task. He should deliver a special carcinogen for scientific research to planet Persephone. This is urgent, so Qwerty has to get to the planet as soon as possible. A lost day may fail negotiations as nobody is going to pay for an overdue carcinogen.</p><p>You can consider Qwerty's ship, the planet Persephone and the star Diatar points on a plane. Diatar is located in the origin of coordinate axes — at point <span class="tex-span">(0, 0)</span>. Persephone goes round Diatar along a circular orbit with radius <span class="tex-span"><i>R</i></span> in the counter-clockwise direction at constant linear speed <span class="tex-span"><i>v</i><sub class="lower-index"><i>p</i></sub></span> (thus, for instance, a full circle around the star takes <img align="middle" class="tex-formula" src="file://lYXHmCj7.png" style="max-width: 100.0%;max-height: 100.0%;"> of time). At the initial moment of time Persephone is located at point <span class="tex-span">(<i>x</i><sub class="lower-index"><i>p</i></sub>, <i>y</i><sub class="lower-index"><i>p</i></sub>)</span>.</p><p>At the initial moment of time Qwerty's ship is at point <span class="tex-span">(<i>x</i>, <i>y</i>)</span>. Qwerty can move in any direction at speed of at most <span class="tex-span"><i>v</i></span> (<span class="tex-span"><i>v</i> &gt; <i>v</i><sub class="lower-index"><i>p</i></sub></span>). The star Diatar is hot (as all stars), so Qwerty can't get too close to it. The ship's metal sheathing melts at distance <span class="tex-span"><i>r</i></span> (<span class="tex-span"><i>r</i> &lt; <i>R</i></span>) from the star.</p><p>Find the minimum time Qwerty needs to get the carcinogen to planet Persephone.</p></div><div class="input-specification"><p>The first line contains space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>p</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>p</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>p</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">4</sup> ≤ <i>x</i><sub class="lower-index"><i>p</i></sub>, <i>y</i><sub class="lower-index"><i>p</i></sub> ≤ 10<sup class="upper-index">4</sup></span>, <span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>p</i></sub> &lt; 10<sup class="upper-index">4</sup></span>) — Persephone's initial position and the speed at which it goes round Diatar.</p><p>The second line contains space-separated integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span"> - 10<sup class="upper-index">4</sup> ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">4</sup></span>, <span class="tex-span">1 &lt; <i>v</i> ≤ 10<sup class="upper-index">4</sup></span>, <span class="tex-span">1 ≤ <i>r</i> ≤ 10<sup class="upper-index">4</sup></span>) — The intial position of Qwerty's ship, its maximum speed and the minimum safe distance to star Diatar.</p><p>It is guaranteed that <span class="tex-span"><i>r</i><sup class="upper-index">2</sup> &lt; <i>x</i><sup class="upper-index">2</sup> + <i>y</i><sup class="upper-index">2</sup></span>, <span class="tex-span"><i>r</i><sup class="upper-index">2</sup> &lt; <i>x</i><sub class="lower-index"><i>p</i></sub><sup class="upper-index">2</sup> + <i>y</i><sub class="lower-index"><i>p</i></sub><sup class="upper-index">2</sup></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>p</i></sub> &lt; <i>v</i></span>.</p></div><div class="output-specification"><p>Print a single real number — the minimum possible delivery time. The answer will be considered valid if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>p</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>p</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>p</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">4</sup> ≤ <i>x</i><sub class="lower-index"><i>p</i></sub>, <i>y</i><sub class="lower-index"><i>p</i></sub> ≤ 10<sup class="upper-index">4</sup></span>, <span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>p</i></sub> &lt; 10<sup class="upper-index">4</sup></span>) — Persephone's initial position and the speed at which it goes round Diatar.</p><p>The second line contains space-separated integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span"> - 10<sup class="upper-index">4</sup> ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">4</sup></span>, <span class="tex-span">1 &lt; <i>v</i> ≤ 10<sup class="upper-index">4</sup></span>, <span class="tex-span">1 ≤ <i>r</i> ≤ 10<sup class="upper-index">4</sup></span>) — The intial position of Qwerty's ship, its maximum speed and the minimum safe distance to star Diatar.</p><p>It is guaranteed that <span class="tex-span"><i>r</i><sup class="upper-index">2</sup> &lt; <i>x</i><sup class="upper-index">2</sup> + <i>y</i><sup class="upper-index">2</sup></span>, <span class="tex-span"><i>r</i><sup class="upper-index">2</sup> &lt; <i>x</i><sub class="lower-index"><i>p</i></sub><sup class="upper-index">2</sup> + <i>y</i><sub class="lower-index"><i>p</i></sub><sup class="upper-index">2</sup></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>p</i></sub> &lt; <i>v</i></span>.</p>

## Output

<p>Print a single real number — the minimum possible delivery time. The answer will be considered valid if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
10 0 1
-10 0 2 8

```




```input2
50 60 10
50 60 20 40

```




```output1
9.584544103
```




```output2
0.000000000
```


