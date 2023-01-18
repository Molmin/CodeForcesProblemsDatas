## Description

<div><p>Tony Stark is playing a game with his suits (they have auto-pilot now). He lives in Malibu. Malibu has <span class="tex-span"><i>n</i></span> junctions numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, connected with <span class="tex-span"><i>n</i> - 1</span> roads. One can get from a junction to any other junction using these roads (graph of Malibu forms a tree).</p><p>Tony has <span class="tex-span"><i>m</i></span> suits. There's a special plan for each suit. The <span class="tex-span"><i>i</i></span>-th suit will appear at the moment of time <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> in the junction <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, and will move to junction <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> using the shortest path between <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> with the speed <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> roads per second (passing a junctions takes no time), and vanishing immediately when arriving at <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> (if it reaches <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> in time <span class="tex-span"><i>q</i></span>, it's available there at moment <span class="tex-span"><i>q</i></span>, but not in further moments). Also, suits move continuously (for example if <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub> ≠ <i>u</i><sub class="lower-index"><i>i</i></sub></span>, at time <img align="middle" class="tex-formula" src="file://b3PFAvaX.png" style="max-width: 100.0%;max-height: 100.0%;"> it's in the middle of a road. Please note that if <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub> = <i>u</i><sub class="lower-index"><i>i</i></sub></span> it means the suit will be at junction number <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> only at moment <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and then it vanishes. </p><p>An explosion happens if at any moment of time two suits share the same exact location (it may be in a junction or somewhere on a road; while appearing, vanishing or moving).</p><p>Your task is to tell Tony the moment of the the first explosion (if there will be any).</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100 000</span>)&nbsp;— the number of junctions and the number of suits respectively.</p><p>The next <span class="tex-span"><i>n</i> - 1</span> lines contain the roads descriptions. Each line contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— endpoints of the <span class="tex-span"><i>i</i></span>-th road (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>).</p><p>The next <span class="tex-span"><i>m</i></span> lines contain the suit descriptions. The <span class="tex-span"><i>i</i></span>-th of them contains four integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10 000, 1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10 000</span>, <span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), meaning the <span class="tex-span"><i>i</i></span>-th suit will appear at moment of time <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> at the junction <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and will move to the junction <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> with a speed <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> roads per second.</p></div><div class="output-specification"><p>If there would be no explosions at all, print <span class="tex-font-style-tt">-1</span> in the first and only line of output.</p><p>Otherwise print the moment of the first explosion.</p><p>Your answer will be considered correct if its relative or absolute error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100 000</span>)&nbsp;— the number of junctions and the number of suits respectively.</p><p>The next <span class="tex-span"><i>n</i> - 1</span> lines contain the roads descriptions. Each line contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— endpoints of the <span class="tex-span"><i>i</i></span>-th road (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>).</p><p>The next <span class="tex-span"><i>m</i></span> lines contain the suit descriptions. The <span class="tex-span"><i>i</i></span>-th of them contains four integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10 000, 1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10 000</span>, <span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), meaning the <span class="tex-span"><i>i</i></span>-th suit will appear at moment of time <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> at the junction <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and will move to the junction <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> with a speed <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> roads per second.</p>

## Output

<p>If there would be no explosions at all, print <span class="tex-font-style-tt">-1</span> in the first and only line of output.</p><p>Otherwise print the moment of the first explosion.</p><p>Your answer will be considered correct if its relative or absolute error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
6 4
2 5
6 5
3 6
4 6
4 1
27 6 1 3
9 5 1 6
27 4 3 4
11 29 2 6

```




```input2
6 4
3 1
4 5
6 4
6 1
2 6
16 4 4 5
13 20 6 2
3 16 4 5
28 5 3 5

```




```output1
27.3

```




```output2
-1

```


