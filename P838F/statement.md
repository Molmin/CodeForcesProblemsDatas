## Description

<div><p>You are playing a game with a bag of red and black balls. Initially, you are told that the bag has <span class="tex-span"><i>n</i></span> balls total. In addition, you are also told that the bag has probability <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> / 10<sup class="upper-index">6</sup></span> of containing exactly <span class="tex-span"><i>i</i></span> red balls.</p><p>You now would like to buy balls from this bag. You really like the color red, so red balls are worth a unit of <span class="tex-span">1</span>, while black balls are worth nothing. To buy a ball, if there are still balls in the bag, you pay a cost <span class="tex-span"><i>c</i></span> with <span class="tex-span">0 ≤ <i>c</i> ≤ 1</span>, and draw a ball randomly from the bag. You can choose to stop buying at any point (and you can even choose to not buy anything at all).</p><p>Given that you buy optimally to maximize the expected profit (i.e. # red balls - cost needed to obtain them), print the maximum expected profit.</p></div><div class="input-specification"><p>The first line of input will contain two integers <span class="tex-span"><i>n</i>, <i>X</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10 000</span>, <span class="tex-span">0 ≤ <i>X</i> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>The next line of input will contain <span class="tex-span"><i>n</i> + 1</span> integers <span class="tex-span"><i>p</i><sub class="lower-index">0</sub>, <i>p</i><sub class="lower-index">1</sub>, ... <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>, <img align="middle" class="tex-formula" src="file://IKzuDsnV.png" style="max-width: 100.0%;max-height: 100.0%;">)</p><p>The value of <span class="tex-span"><i>c</i></span> can be computed as <img align="middle" class="tex-formula" src="file://8EkZCqdi.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="output-specification"><p>Print a single floating point number representing the optimal expected value.</p><p>Your answer will be accepted if it has absolute or relative error at most <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>. More specifically, if your answer is <span class="tex-span"><i>a</i></span> and the jury answer is <span class="tex-span"><i>b</i></span>, your answer will be accepted if <img align="middle" class="tex-formula" src="file://kx8xMHr1.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line of input will contain two integers <span class="tex-span"><i>n</i>, <i>X</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10 000</span>, <span class="tex-span">0 ≤ <i>X</i> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>The next line of input will contain <span class="tex-span"><i>n</i> + 1</span> integers <span class="tex-span"><i>p</i><sub class="lower-index">0</sub>, <i>p</i><sub class="lower-index">1</sub>, ... <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>, <img align="middle" class="tex-formula" src="file://IKzuDsnV.png" style="max-width: 100.0%;max-height: 100.0%;">)</p><p>The value of <span class="tex-span"><i>c</i></span> can be computed as <img align="middle" class="tex-formula" src="file://8EkZCqdi.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>

## Output

<p>Print a single floating point number representing the optimal expected value.</p><p>Your answer will be accepted if it has absolute or relative error at most <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>. More specifically, if your answer is <span class="tex-span"><i>a</i></span> and the jury answer is <span class="tex-span"><i>b</i></span>, your answer will be accepted if <img align="middle" class="tex-formula" src="file://kx8xMHr1.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
3 200000
250000 250000 250000 250000

```




```output1
0.9000000000

```



## Note

<p>Here, there is equal probability for the bag to contain 0,1,2,3 red balls. Also, it costs 0.2 to draw a ball from the bag.</p>
