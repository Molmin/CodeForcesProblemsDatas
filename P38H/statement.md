## Description

<div><p>On the Berland Dependence Day it was decided to organize a great marathon. Berland consists of <span class="tex-span"><i>n</i></span> cities, some of which are linked by two-way roads. Each road has a certain length. The cities are numbered from 1 to <span class="tex-span"><i>n</i></span>. It is known that one can get from any city to any other one by the roads.</p><p><span class="tex-span"><i>n</i></span> runners take part in the competition, one from each city. But Berland runners are talkative by nature and that's why the juries took measures to avoid large crowds of marathon participants. The jury decided that every runner should start the marathon from their hometown. Before the start every sportsman will get a piece of paper containing the name of the city where the sportsman's finishing line is. The finish is chosen randomly for every sportsman but it can't coincide with the sportsman's starting point. Several sportsmen are allowed to finish in one and the same city. All the sportsmen start simultaneously and everyone runs the shortest route from the starting point to the finishing one. All the sportsmen run at one speed which equals to <span class="tex-span">1</span>.</p><p>After the competition a follow-up table of the results will be composed where the sportsmen will be sorted according to the nondecrease of time they spent to cover the distance. The first <span class="tex-span"><i>g</i></span> sportsmen in the table will get golden medals, the next <span class="tex-span"><i>s</i></span> sportsmen will get silver medals and the rest will get bronze medals. Besides, if two or more sportsmen spend the same amount of time to cover the distance, they are sorted according to the number of the city where a sportsman started to run in the ascending order. That means no two sportsmen share one and the same place.</p><p>According to the rules of the competition the number of gold medals <span class="tex-span"><i>g</i></span> must satisfy the inequation <span class="tex-span"><i>g</i><sub class="lower-index">1</sub> ≤ <i>g</i> ≤ <i>g</i><sub class="lower-index">2</sub></span>, where <span class="tex-span"><i>g</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>g</i><sub class="lower-index">2</sub></span> are values formed historically. In a similar way, the number of silver medals <span class="tex-span"><i>s</i></span> must satisfy the inequation <span class="tex-span"><i>s</i><sub class="lower-index">1</sub> ≤ <i>s</i> ≤ <i>s</i><sub class="lower-index">2</sub></span>, where <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> are also values formed historically.</p><p>At present, before the start of the competition, the destination points of every sportsman are unknown. However, the press demands details and that's why you are given the task of counting the number of the ways to distribute the medals. Two ways to distribute the medals are considered different if at least one sportsman could have received during those distributions different kinds of medals.</p></div><div class="input-specification"><p>The first input line contains given integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 50</span>, <span class="tex-span"><i>n</i> - 1 ≤ <i>m</i> ≤ 1000</span>), where <span class="tex-span"><i>n</i></span> is the number of Berland towns and <span class="tex-span"><i>m</i></span> is the number of roads.</p><p>Next in <span class="tex-span"><i>m</i></span> lines road descriptions are given as groups of three integers <span class="tex-span"><i>v</i></span>, <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>c</i></span>, which are the numbers of linked towns and its length (<span class="tex-span">1 ≤ <i>v</i>, <i>u</i> ≤ <i>n</i></span>, <span class="tex-span"><i>v</i> ≠ <i>u</i></span>, <span class="tex-span">1 ≤ <i>c</i> ≤ 1000</span>). Every pair of cities have no more than one road between them.</p><p>The last line contains integers <span class="tex-span"><i>g</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>g</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>g</i><sub class="lower-index">1</sub> ≤ <i>g</i><sub class="lower-index">2</sub></span>, <span class="tex-span">1 ≤ <i>s</i><sub class="lower-index">1</sub> ≤ <i>s</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>g</i><sub class="lower-index">2</sub> + <i>s</i><sub class="lower-index">2</sub> &lt; <i>n</i></span>). The input data numbers, located on one line, are space-separated.</p></div><div class="output-specification"><p>Print the single number — the number of ways to distribute the medals. It is guaranteed that the number fits in the standard 64-bit signed data type.</p></div>

## Input

<p>The first input line contains given integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 50</span>, <span class="tex-span"><i>n</i> - 1 ≤ <i>m</i> ≤ 1000</span>), where <span class="tex-span"><i>n</i></span> is the number of Berland towns and <span class="tex-span"><i>m</i></span> is the number of roads.</p><p>Next in <span class="tex-span"><i>m</i></span> lines road descriptions are given as groups of three integers <span class="tex-span"><i>v</i></span>, <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>c</i></span>, which are the numbers of linked towns and its length (<span class="tex-span">1 ≤ <i>v</i>, <i>u</i> ≤ <i>n</i></span>, <span class="tex-span"><i>v</i> ≠ <i>u</i></span>, <span class="tex-span">1 ≤ <i>c</i> ≤ 1000</span>). Every pair of cities have no more than one road between them.</p><p>The last line contains integers <span class="tex-span"><i>g</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>g</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>g</i><sub class="lower-index">1</sub> ≤ <i>g</i><sub class="lower-index">2</sub></span>, <span class="tex-span">1 ≤ <i>s</i><sub class="lower-index">1</sub> ≤ <i>s</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>g</i><sub class="lower-index">2</sub> + <i>s</i><sub class="lower-index">2</sub> &lt; <i>n</i></span>). The input data numbers, located on one line, are space-separated.</p>

## Output

<p>Print the single number — the number of ways to distribute the medals. It is guaranteed that the number fits in the standard 64-bit signed data type.</p>





```input1
3 2
1 2 1
2 3 1
1 1 1 1

```




```input2
4 5
1 2 2
2 3 1
3 4 2
4 1 2
1 3 3
1 2 1 1

```




```input3
3 3
1 2 2
2 3 1
3 1 2
1 1 1 1

```




```output1
3

```




```output2
19

```




```output3
4

```


