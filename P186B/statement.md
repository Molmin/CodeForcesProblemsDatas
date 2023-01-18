## Description

<div><p>Each year in the castle of Dwarven King there is a competition in growing mushrooms among the dwarves. The competition is one of the most prestigious ones, and the winner gets a wooden salad bowl. This year's event brought together the best mushroom growers from around the world, so we had to slightly change the rules so that the event gets more interesting to watch.</p><p>Each mushroom grower has a mushroom that he will grow on the competition. Under the new rules, the competition consists of two parts. The first part lasts <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span> seconds and the second part lasts <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span> seconds. The first and the second part are separated by a little break.</p><p>After the starting whistle the first part of the contest starts, and all mushroom growers start growing mushrooms at once, each at his individual speed of <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> meters per second. After <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span> seconds, the mushroom growers stop growing mushrooms and go to have a break. During the break, for unexplained reasons, the growth of all mushrooms is reduced by <span class="tex-span"><i>k</i></span> percent. After the break the second part of the contest starts and all mushrooms growers at the same time continue to grow mushrooms, each at his individual speed of <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> meters per second. After a <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span> seconds after the end of the break, the competition ends. Note that the speeds before and after the break may vary.</p><p>Before the match dwarf Pasha learned from all participants, what two speeds they have chosen. However, the participants did not want to disclose to him all their strategy and therefore, did not say in what order they will be using these speeds. That is, if a participant chose speeds <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, then there are two strategies: he either uses speed <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> before the break and speed <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> after it, or vice versa.</p><p>Dwarf Pasha really wants to win the totalizer. He knows that each participant chooses the strategy that maximizes the height of the mushroom. Help Dwarf Pasha make the final table of competition results.</p><p>The participants are sorted in the result table by the mushroom height (the participants with higher mushrooms follow earlier in the table). In case of equal mushroom heights, the participants are sorted by their numbers (the participants with a smaller number follow earlier).</p></div><div class="input-specification"><p>The first input line contains four integer numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub> ≤ 1000;&nbsp;1 ≤ <i>k</i> ≤ 100)</span> — the number of participants, the time before the break, the time after the break and the percentage, by which the mushroom growth drops during the break, correspondingly.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains two integers. The <span class="tex-span"><i>i</i></span>-th <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i>)</span> line contains space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 1000)</span> — the speeds which the participant number <span class="tex-span"><i>i</i></span> chose.</p></div><div class="output-specification"><p>Print the final results' table: <span class="tex-span"><i>n</i></span> lines, each line should contain the number of the corresponding dwarf and the final maximum height of his mushroom with <span class="tex-font-style-bf">exactly two digits</span> after the decimal point. The answer will be considered correct if it is <span class="tex-font-style-bf">absolutely accurate</span>.</p></div>

## Input

<p>The first input line contains four integer numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub> ≤ 1000;&nbsp;1 ≤ <i>k</i> ≤ 100)</span> — the number of participants, the time before the break, the time after the break and the percentage, by which the mushroom growth drops during the break, correspondingly.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains two integers. The <span class="tex-span"><i>i</i></span>-th <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i>)</span> line contains space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 1000)</span> — the speeds which the participant number <span class="tex-span"><i>i</i></span> chose.</p>

## Output

<p>Print the final results' table: <span class="tex-span"><i>n</i></span> lines, each line should contain the number of the corresponding dwarf and the final maximum height of his mushroom with <span class="tex-font-style-bf">exactly two digits</span> after the decimal point. The answer will be considered correct if it is <span class="tex-font-style-bf">absolutely accurate</span>.</p>





```input1
2 3 3 50
2 4
4 2

```




```input2
4 1 1 1
544 397
280 101
280 101
693 970

```




```output1
1 15.00
2 15.00

```




```output2
4 1656.07
1 937.03
2 379.99
3 379.99

```



## Note

<ul> <li> First example: for each contestant it is optimal to use firstly speed 2 and afterwards speed 4, because <span class="tex-span">2·3·0.5 + 4·3 &gt; 4·3·0.5 + 2·3</span>. </li></ul>
