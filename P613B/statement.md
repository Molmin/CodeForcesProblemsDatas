## Description

<div><p>Lesha plays the recently published new version of the legendary game hacknet. In this version character skill mechanism was introduced. Now, each player character has exactly <span class="tex-span"><i>n</i></span> skills. Each skill is represented by a non-negative integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— the current skill level. All skills have the same maximum level <span class="tex-span"><i>A</i></span>.</p><p>Along with the skills, global ranking of all players was added. Players are ranked according to the so-called Force. The <span class="tex-font-style-it">Force</span> of a player is the sum of the following values:</p><ul> <li> The number of skills that a character has perfected (i.e., such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>A</i></span>), multiplied by coefficient <span class="tex-span"><i>c</i><sub class="lower-index"><i>f</i></sub></span>.</li><li> The minimum skill level among all skills (<span class="tex-span"><i>min</i> <i>a</i><sub class="lower-index"><i>i</i></sub></span>), multiplied by coefficient <span class="tex-span"><i>c</i><sub class="lower-index"><i>m</i></sub></span>. </li></ul><p>Now Lesha has <span class="tex-span"><i>m</i></span> hacknetian currency units, which he is willing to spend. Each currency unit can increase the current level of any skill by <span class="tex-span">1</span> (if it's not equal to <span class="tex-span"><i>A</i></span> yet). Help him spend his money in order to achieve the maximum possible value of the Force.</p></div><div class="input-specification"><p>The first line of the input contains five space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>A</i></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>f</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>m</i></sub></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>A</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>f</i></sub>, <i>c</i><sub class="lower-index"><i>m</i></sub> ≤ 1000</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 10<sup class="upper-index">15</sup></span>).</p><p>The second line contains exactly <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>A</i></span>), separated by spaces,&nbsp;— the current levels of skills.</p></div><div class="output-specification"><p>On the first line print the maximum value of the Force that the character can achieve using no more than <span class="tex-span"><i>m</i></span> currency units.</p><p>On the second line print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i>'<sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>a</i>'<sub class="lower-index"><i>i</i></sub> ≤ <i>A</i></span>), skill levels which one must achieve in order to reach the specified value of the Force, while using no more than <span class="tex-span"><i>m</i></span> currency units. Numbers should be separated by spaces.</p></div>

## Input

<p>The first line of the input contains five space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>A</i></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>f</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>m</i></sub></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>A</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>f</i></sub>, <i>c</i><sub class="lower-index"><i>m</i></sub> ≤ 1000</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 10<sup class="upper-index">15</sup></span>).</p><p>The second line contains exactly <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>A</i></span>), separated by spaces,&nbsp;— the current levels of skills.</p>

## Output

<p>On the first line print the maximum value of the Force that the character can achieve using no more than <span class="tex-span"><i>m</i></span> currency units.</p><p>On the second line print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i>'<sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>a</i>'<sub class="lower-index"><i>i</i></sub> ≤ <i>A</i></span>), skill levels which one must achieve in order to reach the specified value of the Force, while using no more than <span class="tex-span"><i>m</i></span> currency units. Numbers should be separated by spaces.</p>





```input1
3 5 10 1 5
1 3 1

```




```input2
3 5 10 1 339
1 3 1

```




```output1
12
2 5 2 

```




```output2
35
5 5 5 

```



## Note

<p>In the first test the optimal strategy is to increase the second skill to its maximum, and increase the two others by <span class="tex-font-style-bf">1</span>.</p><p>In the second test one should increase all skills to maximum.</p>
