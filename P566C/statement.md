## Description

<div><p>Some country consists of <span class="tex-span"><i>n</i></span> cities, connected by a railroad network. The transport communication of the country is so advanced that the network consists of a minimum required number of <span class="tex-span">(<i>n</i> - 1)</span> bidirectional roads (in the other words, the graph of roads is a tree). The <span class="tex-span"><i>i</i></span>-th road that directly connects cities <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, has the length of <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> kilometers.</p><p>The transport network is served by a state transporting company FRR (Fabulous Rail Roads). In order to simplify the price policy, it offers a single ride fare on the train. In order to follow the route of length <span class="tex-span"><i>t</i></span> kilometers, you need to pay <img align="middle" class="tex-formula" src="file://t3IR9fzL.png" style="max-width: 100.0%;max-height: 100.0%;"> burles. Note that it is forbidden to split a long route into short segments and pay them separately (a special railroad police, or RRP, controls that the law doesn't get violated).</p><p>A Large Software Company decided to organize a programming tournament. Having conducted several online rounds, the company employees determined a list of finalists and sent it to the logistical department to find a place where to conduct finals. The Large Software Company can easily organize the tournament finals in any of the <span class="tex-span"><i>n</i></span> cities of the country, so the the main factor in choosing the city for the last stage of the tournament is the total cost of buying tickets for all the finalists. We know that the <span class="tex-span"><i>i</i></span>-th city of the country has <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> cup finalists living there.</p><p>Help the company employees find the city such that the total cost of travel of all the participants to it is minimum.</p></div><div class="input-specification"><p>The first line of the input contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>) — the number of cities in the country.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>w</i><sub class="lower-index">1</sub>, <i>w</i><sub class="lower-index">2</sub>, ..., <i>w</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>) — the number of finalists living in each city of the country.</p><p>Next <span class="tex-span">(<i>n</i> - 1)</span> lines contain the descriptions of the railroad, the <span class="tex-span"><i>i</i></span>-th line contains three integers, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>).</p></div><div class="output-specification"><p>Print two numbers — an integer <span class="tex-span"><i>f</i></span> that is the number of the optimal city to conduct the competition, and the real number <span class="tex-span"><i>c</i></span>, equal to the minimum total cost of transporting all the finalists to the competition. Your answer will be considered correct if two conditions are fulfilled at the same time: </p><ol> <li> The absolute or relative error of the printed number <span class="tex-span"><i>c</i></span> in comparison with the cost of setting up a final in city <span class="tex-span"><i>f</i></span> doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>; </li><li> Absolute or relative error of the printed number <span class="tex-span"><i>c</i></span> in comparison to the answer of the jury doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </li></ol><p>If there are multiple answers, you are allowed to print any of them.</p></div>

## Input

<p>The first line of the input contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>) — the number of cities in the country.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>w</i><sub class="lower-index">1</sub>, <i>w</i><sub class="lower-index">2</sub>, ..., <i>w</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>) — the number of finalists living in each city of the country.</p><p>Next <span class="tex-span">(<i>n</i> - 1)</span> lines contain the descriptions of the railroad, the <span class="tex-span"><i>i</i></span>-th line contains three integers, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>).</p>

## Output

<p>Print two numbers — an integer <span class="tex-span"><i>f</i></span> that is the number of the optimal city to conduct the competition, and the real number <span class="tex-span"><i>c</i></span>, equal to the minimum total cost of transporting all the finalists to the competition. Your answer will be considered correct if two conditions are fulfilled at the same time: </p><ol> <li> The absolute or relative error of the printed number <span class="tex-span"><i>c</i></span> in comparison with the cost of setting up a final in city <span class="tex-span"><i>f</i></span> doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>; </li><li> Absolute or relative error of the printed number <span class="tex-span"><i>c</i></span> in comparison to the answer of the jury doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </li></ol><p>If there are multiple answers, you are allowed to print any of them.</p>





```input1
5
3 1 2 6 5
1 2 3
2 3 1
4 3 9
5 3 1

```




```input2
2
5 5
1 2 2

```




```output1
3 192.0
```




```output2
1 14.142135623730951000

```



## Note

<p>In the sample test an optimal variant of choosing a city to conduct the finals of the competition is <span class="tex-span">3</span>. At such choice the cost of conducting is <img align="middle" class="tex-formula" src="file://VQ8KEvkx.png" style="max-width: 100.0%;max-height: 100.0%;"> burles.</p><p>In the second sample test, whatever city you would choose, you will need to pay for the transport for five participants, so you will need to pay <img align="middle" class="tex-formula" src="file://g4QMlz44.png" style="max-width: 100.0%;max-height: 100.0%;"> burles for each one of them.</p>
