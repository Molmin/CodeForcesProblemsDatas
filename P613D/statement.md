## Description

<div><p>Meanwhile, the kingdom of K is getting ready for the marriage of the King's daughter. However, in order not to lose face in front of the relatives, the King should first finish reforms in his kingdom. As the King can not wait for his daughter's marriage, reforms must be finished as soon as possible.</p><p>The kingdom currently consists of <span class="tex-span"><i>n</i></span> cities. Cities are connected by <span class="tex-span"><i>n</i> - 1</span> bidirectional road, such that one can get from any city to any other city. As the King had to save a lot, there is only one path between any two cities.</p><p>What is the point of the reform? The key ministries of the state should be relocated to distinct cities (we call such cities <span class="tex-font-style-it">important</span>). However, due to the fact that there is a high risk of an attack by barbarians it must be done carefully. The King has made several plans, each of which is described by a set of important cities, and now wonders what is the best plan.</p><p>Barbarians can capture some of the cities that are not important (the important ones will have enough protection for sure), after that the captured city becomes impassable. In particular, an interesting feature of the plan is the minimum number of cities that the barbarians need to capture in order to make all the important cities isolated, that is, from all important cities it would be impossible to reach any other important city.</p><p>Help the King to calculate this characteristic for each of his plan.</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of cities in the kingdom.</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two distinct integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the indices of the cities connected by the <span class="tex-span"><i>i</i></span>-th road. It is guaranteed that you can get from any city to any other one moving only along the existing roads.</p><p>The next line contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 100 000</span>)&nbsp;— the number of King's plans.</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines looks as follows: first goes number <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— the number of important cities in the King's plan, (<span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), then follow exactly <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> space-separated pairwise distinct numbers from 1 to <span class="tex-span"><i>n</i></span>&nbsp;— the numbers of important cities in this plan.</p><p>The sum of all <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>'s does't exceed <span class="tex-span">100 000</span>.</p></div><div class="output-specification"><p>For each plan print a single integer — the minimum number of cities that the barbarians need to capture, or print <span class="tex-span"> - 1</span> if all the barbarians' attempts to isolate important cities will not be effective.</p></div>

## Input

<p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of cities in the kingdom.</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two distinct integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the indices of the cities connected by the <span class="tex-span"><i>i</i></span>-th road. It is guaranteed that you can get from any city to any other one moving only along the existing roads.</p><p>The next line contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 100 000</span>)&nbsp;— the number of King's plans.</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines looks as follows: first goes number <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— the number of important cities in the King's plan, (<span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), then follow exactly <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> space-separated pairwise distinct numbers from 1 to <span class="tex-span"><i>n</i></span>&nbsp;— the numbers of important cities in this plan.</p><p>The sum of all <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>'s does't exceed <span class="tex-span">100 000</span>.</p>

## Output

<p>For each plan print a single integer — the minimum number of cities that the barbarians need to capture, or print <span class="tex-span"> - 1</span> if all the barbarians' attempts to isolate important cities will not be effective.</p>





```input1
4
1 3
2 3
4 3
4
2 1 2
3 2 3 4
3 1 2 4
4 1 2 3 4

```




```input2
7
1 2
2 3
3 4
1 5
5 6
5 7
1
4 2 4 6 7

```




```output1
1
-1
1
-1

```




```output2
2

```



## Note

<p>In the first sample, in the first and the third King's plan barbarians can capture the city <span class="tex-font-style-bf">3</span>, and that will be enough. In the second and the fourth plans all their attempts will not be effective.</p><p>In the second sample the cities to capture are <span class="tex-font-style-bf">3</span> and <span class="tex-font-style-bf">5</span>.</p>
