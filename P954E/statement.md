## Description

<div><p>Consider a system of <span class="tex-span"><i>n</i></span> water taps all pouring water into the same container. The <span class="tex-span"><i>i</i></span>-th water tap can be set to deliver any amount of water from <span class="tex-span">0</span> to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> ml per second (this amount may be a real number). The water delivered by <span class="tex-span"><i>i</i></span>-th tap has temperature <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>If for every <img align="middle" class="tex-formula" src="file://areu6JjS.png" style="max-width: 100.0%;max-height: 100.0%;"> you set <span class="tex-span"><i>i</i></span>-th tap to deliver exactly <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> ml of water per second, then the resulting temperature of water will be <img align="middle" class="tex-formula" src="file://DPZNmaQ5.png" style="max-width: 100.0%;max-height: 100.0%;"> (if <img align="middle" class="tex-formula" src="file://6zKYoHbl.png" style="max-width: 100.0%;max-height: 100.0%;">, then to avoid division by zero we state that the resulting water temperature is <span class="tex-span">0</span>).</p><p>You have to set all the water taps in such a way that the resulting temperature is exactly <span class="tex-span"><i>T</i></span>. What is the maximum amount of water you may get per second if its temperature has to be <span class="tex-span"><i>T</i></span>?</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200000</span>, <span class="tex-span">1 ≤ <i>T</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of water taps and the desired temperature of water, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the maximum amount of water <span class="tex-span"><i>i</i></span>-th tap can deliver per second.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the temperature of water each tap delivers.</p></div><div class="output-specification"><p>Print the maximum possible amount of water with temperature exactly <span class="tex-span"><i>T</i></span> you can get per second (if it is impossible to obtain water with such temperature, then the answer is considered to be <span class="tex-span">0</span>).</p><p>Your answer is considered correct if its absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200000</span>, <span class="tex-span">1 ≤ <i>T</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of water taps and the desired temperature of water, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the maximum amount of water <span class="tex-span"><i>i</i></span>-th tap can deliver per second.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the temperature of water each tap delivers.</p>

## Output

<p>Print the maximum possible amount of water with temperature exactly <span class="tex-span"><i>T</i></span> you can get per second (if it is impossible to obtain water with such temperature, then the answer is considered to be <span class="tex-span">0</span>).</p><p>Your answer is considered correct if its absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
2 100
3 10
50 150

```




```input2
3 9
5 5 30
6 6 10

```




```input3
2 12
1 3
10 15

```




```output1
6.000000000000000

```




```output2
40.000000000000000

```




```output3
1.666666666666667

```


