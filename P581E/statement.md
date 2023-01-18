## Description

<div><p>Motorist Kojiro spent <span class="tex-span">10</span> years saving up for his favorite car brand, Furrari. Finally Kojiro's dream came true! Kojiro now wants to get to his girlfriend Johanna to show off his car to her.</p><p>Kojiro wants to get to his girlfriend, so he will go to her along a coordinate line. For simplicity, we can assume that Kojiro is at the point <span class="tex-span"><i>f</i></span> of a coordinate line, and Johanna is at point <span class="tex-span"><i>e</i></span>. Some points of the coordinate line have gas stations. Every gas station fills with only one type of fuel: <span class="tex-font-style-it">Regular-92</span>, <span class="tex-font-style-it">Premium-95</span> or <span class="tex-font-style-it">Super-98</span>. Thus, each gas station is characterized by a pair of integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> — the number of the gas type and its position.</p><p>One liter of fuel is enough to drive for exactly <span class="tex-span">1</span> km (this value does not depend on the type of fuel). Fuels of three types differ only in quality, according to the research, that affects the lifetime of the vehicle motor. A Furrari tank holds exactly <span class="tex-span"><i>s</i></span> liters of fuel (regardless of the type of fuel). At the moment of departure from point <span class="tex-span"><i>f</i></span> Kojiro's tank is completely filled with fuel <span class="tex-font-style-it">Super-98</span>. At each gas station Kojiro can fill the tank with any amount of fuel, but of course, at no point in time, the amount of fuel in the tank can be more than <span class="tex-span"><i>s</i></span> liters. Note that the tank <span class="tex-font-style-bf">can</span> simultaneously have different types of fuel. The car can moves both left and right.</p><p>To extend the lifetime of the engine Kojiro seeks primarily to minimize the amount of fuel of type <span class="tex-font-style-it">Regular-92</span>. If there are several strategies to go from <span class="tex-span"><i>f</i></span> to <span class="tex-span"><i>e</i></span>, using the minimum amount of fuel of type <span class="tex-font-style-it">Regular-92</span>, it is necessary to travel so as to minimize the amount of used fuel of type <span class="tex-font-style-it">Premium-95</span>.</p><p>Write a program that can for the <span class="tex-span"><i>m</i></span> possible positions of the start <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> minimize firstly, the amount of used fuel of type <span class="tex-font-style-it">Regular-92</span> and secondly, the amount of used fuel of type <span class="tex-font-style-it">Premium-95</span>.</p></div><div class="input-specification"><p>The first line of the input contains four positive integers <span class="tex-span"><i>e</i>, <i>s</i>, <i>n</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>e</i>, <i>s</i> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>n</i>, <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the coordinate of the point where Johanna is, the capacity of a Furrari tank, the number of gas stations and the number of starting points. </p><p>Next <span class="tex-span"><i>n</i></span> lines contain two integers each <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub>, <i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 3,  - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), representing the type of the <span class="tex-span"><i>i</i></span>-th gas station (<span class="tex-span">1</span> represents <span class="tex-font-style-it">Regular-92</span>, <span class="tex-span">2</span> — <span class="tex-font-style-it">Premium-95</span> and <span class="tex-span">3</span> — <span class="tex-font-style-it">Super-98</span>) and the position on a coordinate line of the <span class="tex-span"><i>i</i></span>-th gas station. Gas stations don't necessarily follow in order from left to right.</p><p>The last line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> &lt; <i>e</i></span>). Start positions don't necessarily follow in order from left to right.</p><p>No point of the coordinate line contains more than one gas station. It is possible that some of points <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> or point <span class="tex-span"><i>e</i></span> coincide with a gas station.</p></div><div class="output-specification"><p>Print exactly <span class="tex-span"><i>m</i></span> lines. The <span class="tex-span"><i>i</i></span>-th of them should contain two integers — the minimum amount of gas of type <span class="tex-font-style-it">Regular-92</span> and type <span class="tex-font-style-it">Premium-95</span>, if Kojiro starts at point <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span>. First you need to minimize the first value. If there are multiple ways to do it, you need to also minimize the second value.</p><p>If there is no way to get to Johanna from point <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span>, the <span class="tex-span"><i>i</i></span>-th line should look like that "<span class="tex-font-style-tt">-1 -1</span>" (two numbers minus one without the quotes).</p></div>

## Input

<p>The first line of the input contains four positive integers <span class="tex-span"><i>e</i>, <i>s</i>, <i>n</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>e</i>, <i>s</i> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>n</i>, <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the coordinate of the point where Johanna is, the capacity of a Furrari tank, the number of gas stations and the number of starting points. </p><p>Next <span class="tex-span"><i>n</i></span> lines contain two integers each <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub>, <i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 3,  - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), representing the type of the <span class="tex-span"><i>i</i></span>-th gas station (<span class="tex-span">1</span> represents <span class="tex-font-style-it">Regular-92</span>, <span class="tex-span">2</span> — <span class="tex-font-style-it">Premium-95</span> and <span class="tex-span">3</span> — <span class="tex-font-style-it">Super-98</span>) and the position on a coordinate line of the <span class="tex-span"><i>i</i></span>-th gas station. Gas stations don't necessarily follow in order from left to right.</p><p>The last line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> &lt; <i>e</i></span>). Start positions don't necessarily follow in order from left to right.</p><p>No point of the coordinate line contains more than one gas station. It is possible that some of points <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> or point <span class="tex-span"><i>e</i></span> coincide with a gas station.</p>

## Output

<p>Print exactly <span class="tex-span"><i>m</i></span> lines. The <span class="tex-span"><i>i</i></span>-th of them should contain two integers — the minimum amount of gas of type <span class="tex-font-style-it">Regular-92</span> and type <span class="tex-font-style-it">Premium-95</span>, if Kojiro starts at point <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span>. First you need to minimize the first value. If there are multiple ways to do it, you need to also minimize the second value.</p><p>If there is no way to get to Johanna from point <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span>, the <span class="tex-span"><i>i</i></span>-th line should look like that "<span class="tex-font-style-tt">-1 -1</span>" (two numbers minus one without the quotes).</p>





```input1
8 4 1 1
2 4
0

```




```input2
9 3 2 3
2 3
1 6
-1 0 1

```




```input3
20 9 2 4
1 5
2 10
-1 0 1 2

```




```output1
0 4

```




```output2
-1 -1
3 3
3 2

```




```output3
-1 -1
-1 -1
-1 -1
-1 -1

```


