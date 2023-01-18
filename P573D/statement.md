## Description

<div><p>Would you want to fight against bears riding horses? Me neither.</p><p>Limak is a grizzly bear. He is general of the dreadful army of Bearland. The most important part of an army is cavalry of course.</p><p>Cavalry of Bearland consists of <span class="tex-span"><i>n</i></span> warriors and <span class="tex-span"><i>n</i></span> horses. <span class="tex-span"><i>i</i></span>-th warrior has strength <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>i</i></span>-th horse has strength <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>. Warrior together with his horse is called a unit. Strength of a unit is equal to multiplied strengths of warrior and horse. Total strength of cavalry is equal to sum of strengths of all <span class="tex-span"><i>n</i></span> units. Good assignment of warriors and horses makes cavalry truly powerful.</p><p>Initially, <span class="tex-span"><i>i</i></span>-th warrior has <span class="tex-span"><i>i</i></span>-th horse. You are given <span class="tex-span"><i>q</i></span> queries. In each query two warriors swap their horses with each other.</p><p>General Limak must be ready for every possible situation. What if warriors weren't allowed to ride their own horses? After each query find the maximum possible strength of cavalry if we consider assignments of all warriors to all horses that no warrior is assigned to his own horse (it can be proven that for <span class="tex-span"><i>n</i> ≥ 2</span> there is always at least one correct assignment).</p><p>Note that we can't leave a warrior without a horse.</p></div><div class="input-specification"><p>The first line contains two space-separated integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 30 000</span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 10 000</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers, <span class="tex-span"><i>w</i><sub class="lower-index">1</sub>, <i>w</i><sub class="lower-index">2</sub>, ..., <i>w</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — strengths of warriors.</p><p>The third line contains <span class="tex-span"><i>n</i></span> space-separated integers, <span class="tex-span"><i>h</i><sub class="lower-index">1</sub>, <i>h</i><sub class="lower-index">2</sub>, ..., <i>h</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — strengths of horses.</p><p>Next <span class="tex-span"><i>q</i></span> lines describe queries. <span class="tex-span"><i>i</i></span>-th of them contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>), indices of warriors who swap their horses with each other.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>q</i></span> lines with answers to queries. In <span class="tex-span"><i>i</i></span>-th line print the maximum possible strength of cavalry after first <span class="tex-span"><i>i</i></span> queries.</p></div>

## Input

<p>The first line contains two space-separated integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 30 000</span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 10 000</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers, <span class="tex-span"><i>w</i><sub class="lower-index">1</sub>, <i>w</i><sub class="lower-index">2</sub>, ..., <i>w</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — strengths of warriors.</p><p>The third line contains <span class="tex-span"><i>n</i></span> space-separated integers, <span class="tex-span"><i>h</i><sub class="lower-index">1</sub>, <i>h</i><sub class="lower-index">2</sub>, ..., <i>h</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — strengths of horses.</p><p>Next <span class="tex-span"><i>q</i></span> lines describe queries. <span class="tex-span"><i>i</i></span>-th of them contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>), indices of warriors who swap their horses with each other.</p>

## Output

<p>Print <span class="tex-span"><i>q</i></span> lines with answers to queries. In <span class="tex-span"><i>i</i></span>-th line print the maximum possible strength of cavalry after first <span class="tex-span"><i>i</i></span> queries.</p>





```input1
4 2
1 10 100 1000
3 7 2 5
2 4
2 4

```




```input2
3 3
7 11 5
3 2 1
1 2
1 3
2 3

```




```input3
7 4
1 2 4 8 16 32 64
87 40 77 29 50 11 18
1 5
2 7
6 2
5 6

```




```output1
5732
7532

```




```output2
44
48
52

```




```output3
9315
9308
9315
9315

```



## Note

<p>Clarification for the first sample:</p><center> <span class="tex-font-style-tt">Warriors:&nbsp;1&nbsp;10&nbsp;100&nbsp;1000</span><p><span class="tex-font-style-tt">Horses:&nbsp;&nbsp;&nbsp;3&nbsp;&nbsp;7&nbsp;&nbsp;2&nbsp;&nbsp;&nbsp;&nbsp;5&nbsp;</span> </p></center><p>After first query situation looks like the following:</p><center> <span class="tex-font-style-tt">Warriors:&nbsp;1&nbsp;10&nbsp;100&nbsp;1000</span><p><span class="tex-font-style-tt">Horses:&nbsp;&nbsp;&nbsp;3&nbsp;&nbsp;5&nbsp;&nbsp;2&nbsp;&nbsp;&nbsp;&nbsp;7&nbsp;</span> </p></center><p>We can get <span class="tex-span">1·2 + 10·3 + 100·7 + 1000·5 = 5732</span> (note that no hussar takes his own horse in this assignment).</p><p>After second query we get back to initial situation and optimal assignment is <span class="tex-span">1·2 + 10·3 + 100·5 + 1000·7 = 7532</span>.</p><p>Clarification for the second sample. After first query:</p><center> <span class="tex-font-style-tt">Warriors:&nbsp;&nbsp;7&nbsp;11&nbsp;5</span><p><span class="tex-font-style-tt">Horses:&nbsp;&nbsp;&nbsp;&nbsp;2&nbsp;&nbsp;3&nbsp;1</span> </p></center><p>Optimal assignment is <span class="tex-span">7·1 + 11·2 + 5·3 = 44</span>.</p><p>Then after second query <span class="tex-span">7·3 + 11·2 + 5·1 = 48</span>.</p><p>Finally <span class="tex-span">7·2 + 11·3 + 5·1 = 52</span>.</p>
