## Description

<div><p>The tram in Berland goes along a straight line from the point <span class="tex-span">0</span> to the point <span class="tex-span"><i>s</i></span> and back, passing <span class="tex-span">1</span> meter per <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span> seconds in both directions. It means that the tram is always in the state of uniform rectilinear motion, instantly turning around at points <span class="tex-span"><i>x</i> = 0</span> and <span class="tex-span"><i>x</i> = <i>s</i></span>.</p><p>Igor is at the point <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>. He should reach the point <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>. Igor passes <span class="tex-span">1</span> meter per <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span> seconds. </p><p>Your task is to determine the minimum time Igor needs to get from the point <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> to the point <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, if it is known where the tram is and in what direction it goes at the moment Igor comes to the point <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>.</p><p>Igor can enter the tram unlimited number of times at any moment when his and the tram's positions coincide. It is <span class="tex-font-style-bf">not obligatory</span> that points in which Igor enter and exit the tram are integers. Assume that any boarding and unboarding happens instantly. Igor can move arbitrary along the line (but not faster than <span class="tex-span">1</span> meter per <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span> seconds). He can also stand at some point for some time.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>s</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> (<span class="tex-span">2 ≤ <i>s</i> ≤ 1000</span>, <span class="tex-span">0 ≤ <i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub> ≤ <i>s</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> ≠ <i>x</i><sub class="lower-index">2</sub></span>)&nbsp;— the maximum coordinate of the point to which the tram goes, the point Igor is at, and the point he should come to.</p><p>The second line contains two integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub> ≤ 1000</span>)&nbsp;— the time in seconds in which the tram passes <span class="tex-span">1</span> meter and the time in seconds in which Igor passes <span class="tex-span">1</span> meter.</p><p>The third line contains two integers <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>p</i> ≤ <i>s</i> - 1</span>, <span class="tex-span"><i>d</i></span> is either <span class="tex-span">1</span> or <img align="middle" class="tex-formula" src="file://uuGb0OYT.png" style="max-width: 100.0%;max-height: 100.0%;">)&nbsp;— the position of the tram in the moment Igor came to the point <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> and the direction of the tram at this moment. If <img align="middle" class="tex-formula" src="file://k9BIUSsR.png" style="max-width: 100.0%;max-height: 100.0%;">, the tram goes in the direction from the point <span class="tex-span"><i>s</i></span> to the point <span class="tex-span">0</span>. If <span class="tex-span"><i>d</i> = 1</span>, the tram goes in the direction from the point <span class="tex-span">0</span> to the point <span class="tex-span"><i>s</i></span>.</p></div><div class="output-specification"><p>Print the minimum time in seconds which Igor needs to get from the point <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> to the point <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>s</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> (<span class="tex-span">2 ≤ <i>s</i> ≤ 1000</span>, <span class="tex-span">0 ≤ <i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub> ≤ <i>s</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> ≠ <i>x</i><sub class="lower-index">2</sub></span>)&nbsp;— the maximum coordinate of the point to which the tram goes, the point Igor is at, and the point he should come to.</p><p>The second line contains two integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub> ≤ 1000</span>)&nbsp;— the time in seconds in which the tram passes <span class="tex-span">1</span> meter and the time in seconds in which Igor passes <span class="tex-span">1</span> meter.</p><p>The third line contains two integers <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>p</i> ≤ <i>s</i> - 1</span>, <span class="tex-span"><i>d</i></span> is either <span class="tex-span">1</span> or <img align="middle" class="tex-formula" src="file://uuGb0OYT.png" style="max-width: 100.0%;max-height: 100.0%;">)&nbsp;— the position of the tram in the moment Igor came to the point <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> and the direction of the tram at this moment. If <img align="middle" class="tex-formula" src="file://k9BIUSsR.png" style="max-width: 100.0%;max-height: 100.0%;">, the tram goes in the direction from the point <span class="tex-span"><i>s</i></span> to the point <span class="tex-span">0</span>. If <span class="tex-span"><i>d</i> = 1</span>, the tram goes in the direction from the point <span class="tex-span">0</span> to the point <span class="tex-span"><i>s</i></span>.</p>

## Output

<p>Print the minimum time in seconds which Igor needs to get from the point <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> to the point <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>.</p>





```input1
4 2 4
3 4
1 1

```




```input2
5 4 0
1 2
3 1

```




```output1
8

```




```output2
7

```



## Note

<p>In the first example it is profitable for Igor to go by foot and not to wait the tram. Thus, he has to pass <span class="tex-span">2</span> meters and it takes <span class="tex-span">8</span> seconds in total, because he passes <span class="tex-span">1</span> meter per <span class="tex-span">4</span> seconds. </p><p>In the second example Igor can, for example, go towards the point <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> and get to the point <span class="tex-span">1</span> in <span class="tex-span">6</span> seconds (because he has to pass <span class="tex-span">3</span> meters, but he passes <span class="tex-span">1</span> meters per <span class="tex-span">2</span> seconds). At that moment the tram will be at the point <span class="tex-span">1</span>, so Igor can enter the tram and pass <span class="tex-span">1</span> meter in <span class="tex-span">1</span> second. Thus, Igor will reach the point <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> in <span class="tex-span">7</span> seconds in total.</p>
