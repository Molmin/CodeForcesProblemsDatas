## Description

<div><p>You must have heard all about the Foolland on your Geography lessons. Specifically, you must know that federal structure of this country has been the same for many centuries. The country consists of <span class="tex-span"><i>n</i></span> cities, some pairs of cities are connected by bidirectional roads, each road is described by its length <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>The fools lived in their land joyfully, but a recent revolution changed the king. Now the king is Vasily the Bear. Vasily divided the country cities into regions, so that any two cities of the same region have a path along the roads between them and any two cities of different regions don't have such path. Then Vasily decided to upgrade the road network and construct exactly <span class="tex-span"><i>p</i></span> new roads in the country. Constructing a road goes like this:</p><ol> <li> We choose a pair of <span class="tex-font-style-bf">distinct</span> cities <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>v</i></span> that will be connected by a new road (at that, it is possible that there already is a road between these cities). </li><li> We define the length of the new road: if cities <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>v</i></span> belong to distinct regions, then the length is calculated as <span class="tex-span"><i>min</i>(10<sup class="upper-index">9</sup>, <i>S</i> + 1)</span> (<span class="tex-span"><i>S</i></span> — the total length of all roads that exist in the linked regions), otherwise we assume that the length equals <span class="tex-span">1000</span>. </li><li> We build a road of the specified length between the chosen cities. If the new road connects two distinct regions, after construction of the road these regions are combined into one new region. </li></ol><p>Vasily wants the road constructing process to result in the country that consists exactly of <span class="tex-span"><i>q</i></span> regions. Your task is to come up with such road constructing plan for Vasily that it meets the requirement and minimizes the total length of the built roads.</p></div><div class="input-specification"><p>The first line contains four integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>), <span class="tex-span"><i>p</i></span> (<span class="tex-span">0 ≤ <i>p</i> ≤ 10<sup class="upper-index">5</sup></span>), <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ <i>n</i></span>) — the number of cities in the Foolland, the number of existing roads, the number of roads that are planned to construct and the required number of regions.</p><p>Next <span class="tex-span"><i>m</i></span> lines describe the roads that exist by the moment upgrading of the roads begun. Each of these lines contains three integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>: <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> — the numbers of the cities connected by this road (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub></span>), <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> — length of the road (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>. Note that one pair of cities can be connected with multiple roads.</p></div><div class="output-specification"><p>If constructing the roads in the required way is impossible, print a single string "<span class="tex-font-style-tt">NO</span>" (without the quotes). Otherwise, in the first line print word "<span class="tex-font-style-tt">YES</span>" (without the quotes), and in the next <span class="tex-span"><i>p</i></span> lines print the road construction plan. Each line of the plan must consist of two distinct integers, giving the numbers of the cities connected by a road. The road must occur in the plan in the order they need to be constructed. If there are multiple optimal solutions, you can print any of them.</p></div>

## Input

<p>The first line contains four integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>), <span class="tex-span"><i>p</i></span> (<span class="tex-span">0 ≤ <i>p</i> ≤ 10<sup class="upper-index">5</sup></span>), <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ <i>n</i></span>) — the number of cities in the Foolland, the number of existing roads, the number of roads that are planned to construct and the required number of regions.</p><p>Next <span class="tex-span"><i>m</i></span> lines describe the roads that exist by the moment upgrading of the roads begun. Each of these lines contains three integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>: <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> — the numbers of the cities connected by this road (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub></span>), <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> — length of the road (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>. Note that one pair of cities can be connected with multiple roads.</p>

## Output

<p>If constructing the roads in the required way is impossible, print a single string "<span class="tex-font-style-tt">NO</span>" (without the quotes). Otherwise, in the first line print word "<span class="tex-font-style-tt">YES</span>" (without the quotes), and in the next <span class="tex-span"><i>p</i></span> lines print the road construction plan. Each line of the plan must consist of two distinct integers, giving the numbers of the cities connected by a road. The road must occur in the plan in the order they need to be constructed. If there are multiple optimal solutions, you can print any of them.</p>





```input1
9 6 2 2
1 2 2
3 2 1
4 6 20
1 3 8
7 8 3
5 7 2

```




```input2
2 0 1 2

```




```input3
2 0 0 2

```




```output1
YES
9 5
1 9

```




```output2
NO

```




```output3
YES

```



## Note

<p>Consider the first sample. Before the reform the Foolland consists of four regions. The first region includes cities <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">3</span>, the second region has cities <span class="tex-span">4</span> and <span class="tex-span">6</span>, the third region has cities <span class="tex-span">5</span>, <span class="tex-span">7</span>, <span class="tex-span">8</span>, the fourth region has city <span class="tex-span">9</span>. The total length of the roads in these cities is <span class="tex-span">11</span>, <span class="tex-span">20</span>, <span class="tex-span">5</span> and <span class="tex-span">0</span>, correspondingly. According to the plan, we first build the road of length <span class="tex-span">6</span> between cities <span class="tex-span">5</span> and <span class="tex-span">9</span>, then the road of length <span class="tex-span">23</span> between cities <span class="tex-span">1</span> and <span class="tex-span">9</span>. Thus, the total length of the built roads equals <span class="tex-span">29</span>.</p>
