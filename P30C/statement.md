## Description

<div><p>One warm and sunny day king Copa decided to visit the shooting gallery, located at the Central Park, and try to win the main prize — big pink plush panda. The king is not good at shooting, so he invited you to help him.</p><p>The shooting gallery is an infinite vertical plane with Cartesian coordinate system on it. The targets are points on this plane. Each target is described by it's coordinates <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, by the time of it's appearance <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and by the number <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, which gives the probability that Copa hits this target if he aims at it.</p><p>A target appears and disappears instantly, so Copa can hit the target only if at the moment <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> his gun sight aimed at <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>. Speed of movement of the gun sight on the plane is equal to 1. Copa knows all the information about the targets beforehand (remember, he is a king!). He wants to play in the optimal way, which maximizes the expected value of the amount of hit targets. He can aim at any target at the moment 0.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — amount of targets in the shooting gallery. Then <span class="tex-span"><i>n</i></span> lines follow, each describing one target. Each description consists of four numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> — integers, <span class="tex-span"> - 1000 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 1000, 0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, real number <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is given with no more than 6 digits after the decimal point, <span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>). No two targets may be at the same point.</p></div><div class="output-specification"><p>Output the maximum expected value of the amount of targets that was shot by the king. Your answer will be accepted if it differs from the correct answer by not more than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — amount of targets in the shooting gallery. Then <span class="tex-span"><i>n</i></span> lines follow, each describing one target. Each description consists of four numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> — integers, <span class="tex-span"> - 1000 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 1000, 0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, real number <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is given with no more than 6 digits after the decimal point, <span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>). No two targets may be at the same point.</p>

## Output

<p>Output the maximum expected value of the amount of targets that was shot by the king. Your answer will be accepted if it differs from the correct answer by not more than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
1
0 0 0 0.5

```




```input2
2
0 0 0 0.6
5 0 5 0.7

```




```output1
0.5000000000

```




```output2
1.3000000000

```


