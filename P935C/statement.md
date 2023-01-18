## Description

<div><p>Fifa and Fafa are sharing a flat. Fifa loves video games and wants to download a new soccer game. Unfortunately, Fafa heavily uses the internet which consumes the quota. Fifa can access the internet through his Wi-Fi access point. This access point can be accessed within a range of <span class="tex-span"><i>r</i></span> meters (this range can be chosen by Fifa) from its position. Fifa must put the access point inside the flat which has a circular shape of radius <span class="tex-span"><i>R</i></span>. Fifa wants to minimize the area that is not covered by the access point inside the flat without letting Fafa or anyone outside the flat to get access to the internet.</p><p>The world is represented as an infinite 2D plane. The flat is centered at <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> and has radius <span class="tex-span"><i>R</i></span> and Fafa's laptop is located at <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span>, not necessarily inside the flat. Find the position and the radius chosen by Fifa for his access point which minimizes the uncovered area.</p></div><div class="input-specification"><p>The single line of the input contains 5 space-separated integers <span class="tex-span"><i>R</i>, <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>R</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">|<i>x</i><sub class="lower-index">1</sub>|, |<i>y</i><sub class="lower-index">1</sub>|, |<i>x</i><sub class="lower-index">2</sub>|, |<i>y</i><sub class="lower-index">2</sub>| ≤ 10<sup class="upper-index">5</sup></span>).</p></div><div class="output-specification"><p>Print three space-separated numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>ap</i></sub>, <i>y</i><sub class="lower-index"><i>ap</i></sub>, <i>r</i></span> where <span class="tex-span">(<i>x</i><sub class="lower-index"><i>ap</i></sub>, <i>y</i><sub class="lower-index"><i>ap</i></sub>)</span> is the position which Fifa chose for the access point and <span class="tex-span"><i>r</i></span> is the radius of its range. </p><p>Your answer will be considered correct if the radius does not differ from optimal more than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span> absolutely or relatively, and also the radius you printed can be changed by no more than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span> (absolutely or relatively) in such a way that all points outside the flat and Fafa's laptop position are outside circle of the access point range.</p></div>

## Input

<p>The single line of the input contains 5 space-separated integers <span class="tex-span"><i>R</i>, <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>R</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">|<i>x</i><sub class="lower-index">1</sub>|, |<i>y</i><sub class="lower-index">1</sub>|, |<i>x</i><sub class="lower-index">2</sub>|, |<i>y</i><sub class="lower-index">2</sub>| ≤ 10<sup class="upper-index">5</sup></span>).</p>

## Output

<p>Print three space-separated numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>ap</i></sub>, <i>y</i><sub class="lower-index"><i>ap</i></sub>, <i>r</i></span> where <span class="tex-span">(<i>x</i><sub class="lower-index"><i>ap</i></sub>, <i>y</i><sub class="lower-index"><i>ap</i></sub>)</span> is the position which Fifa chose for the access point and <span class="tex-span"><i>r</i></span> is the radius of its range. </p><p>Your answer will be considered correct if the radius does not differ from optimal more than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span> absolutely or relatively, and also the radius you printed can be changed by no more than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span> (absolutely or relatively) in such a way that all points outside the flat and Fafa's laptop position are outside circle of the access point range.</p>





```input1
5 3 3 1 1

```




```input2
10 5 5 5 15

```




```output1
3.7677669529663684 3.7677669529663684 3.914213562373095

```




```output2
5.0 5.0 10.0

```


