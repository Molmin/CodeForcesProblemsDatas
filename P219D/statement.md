## Description

<div><p>The country Treeland consists of <span class="tex-span"><i>n</i></span> cities, some pairs of them are connected with <span class="tex-font-style-it">unidirectional</span> roads. Overall there are <span class="tex-span"><i>n</i> - 1</span> roads in the country. We know that if we don't take the direction of the roads into consideration, we can get from any city to any other one.</p><p>The council of the elders has recently decided to choose the capital of Treeland. Of course it should be a city of this country. The council is supposed to meet in the capital and regularly move from the capital to other cities (at this stage nobody is thinking about getting back to the capital from these cities). For that reason if city <span class="tex-span"><i>a</i></span> is chosen a capital, then all roads must be oriented so that if we move along them, we can get from city <span class="tex-span"><i>a</i></span> to any other city. For that some roads may have to be inversed.</p><p>Help the elders to choose the capital so that they have to inverse the minimum number of roads in the country.</p></div><div class="input-specification"><p>The first input line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of cities in Treeland. Next <span class="tex-span"><i>n</i> - 1</span> lines contain the descriptions of the roads, one road per line. A road is described by a pair of integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>s</i><sub class="lower-index"><i>i</i></sub> ≠ <i>t</i><sub class="lower-index"><i>i</i></sub></span>) — the numbers of cities, connected by that road. The <span class="tex-span"><i>i</i></span>-th road is oriented from city <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> to city <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>. You can consider cities in Treeland indexed from 1 to <span class="tex-span"><i>n</i></span>.</p></div><div class="output-specification"><p>In the first line print the minimum number of roads to be inversed if the capital is chosen optimally. In the second line print all possible ways to choose the capital — a sequence of indexes of cities in the increasing order.</p></div>

## Input

<p>The first input line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of cities in Treeland. Next <span class="tex-span"><i>n</i> - 1</span> lines contain the descriptions of the roads, one road per line. A road is described by a pair of integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>s</i><sub class="lower-index"><i>i</i></sub> ≠ <i>t</i><sub class="lower-index"><i>i</i></sub></span>) — the numbers of cities, connected by that road. The <span class="tex-span"><i>i</i></span>-th road is oriented from city <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> to city <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>. You can consider cities in Treeland indexed from 1 to <span class="tex-span"><i>n</i></span>.</p>

## Output

<p>In the first line print the minimum number of roads to be inversed if the capital is chosen optimally. In the second line print all possible ways to choose the capital — a sequence of indexes of cities in the increasing order.</p>





```input1
3
2 1
2 3

```




```input2
4
1 4
2 4
3 4

```




```output1
0
2 

```




```output2
2
1 2 3 

```


