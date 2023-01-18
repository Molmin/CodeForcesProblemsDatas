## Description

<div><p>When Kefa came to the restaurant and sat at a table, the waiter immediately brought him the menu. There were <span class="tex-span"><i>n</i></span> dishes. Kefa knows that he needs exactly <span class="tex-span"><i>m</i></span> dishes. But at that, he doesn't want to order the same dish twice to taste as many dishes as possible. </p><p>Kefa knows that the <span class="tex-span"><i>i</i></span>-th dish gives him <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> units of satisfaction. But some dishes do not go well together and some dishes go very well together. Kefa set to himself <span class="tex-span"><i>k</i></span> rules of eating food of the following type — if he eats dish <span class="tex-span"><i>x</i></span> exactly before dish <span class="tex-span"><i>y</i></span> (there should be no other dishes between <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>), then his satisfaction level raises by <span class="tex-span"><i>c</i></span>. </p><p>Of course, our parrot wants to get some maximal possible satisfaction from going to the restaurant. Help him in this hard task!</p></div><div class="input-specification"><p>The first line of the input contains three space-separated numbers, <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i> ≤ 18</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ <i>n</i> * (<i>n</i> - 1)</span>) — the number of dishes on the menu, the number of portions Kefa needs to eat to get full and the number of eating rules.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the satisfaction he gets from the <span class="tex-span"><i>i</i></span>-th dish.</p><p>Next <span class="tex-span"><i>k</i></span> lines contain the rules. The <span class="tex-span"><i>i</i></span>-th rule is described by the three numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). That means that if you eat dish <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> right before dish <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, then the Kefa's satisfaction increases by <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that there are no such pairs of indexes <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>i</i> &lt; <i>j</i> ≤ <i>k</i></span>), that <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> = <i>x</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub> = <i>y</i><sub class="lower-index"><i>j</i></sub></span>.</p></div><div class="output-specification"><p>In the single line of the output print the maximum satisfaction that Kefa can get from going to the restaurant.</p></div>

## Input

<p>The first line of the input contains three space-separated numbers, <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i> ≤ 18</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ <i>n</i> * (<i>n</i> - 1)</span>) — the number of dishes on the menu, the number of portions Kefa needs to eat to get full and the number of eating rules.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the satisfaction he gets from the <span class="tex-span"><i>i</i></span>-th dish.</p><p>Next <span class="tex-span"><i>k</i></span> lines contain the rules. The <span class="tex-span"><i>i</i></span>-th rule is described by the three numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). That means that if you eat dish <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> right before dish <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, then the Kefa's satisfaction increases by <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that there are no such pairs of indexes <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>i</i> &lt; <i>j</i> ≤ <i>k</i></span>), that <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> = <i>x</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub> = <i>y</i><sub class="lower-index"><i>j</i></sub></span>.</p>

## Output

<p>In the single line of the output print the maximum satisfaction that Kefa can get from going to the restaurant.</p>





```input1
2 2 1
1 1
2 1 1

```




```input2
4 3 2
1 2 3 4
2 1 5
3 4 2

```




```output1
3

```




```output2
12

```



## Note

<p>In the first sample it is best to first eat the second dish, then the first one. Then we get one unit of satisfaction for each dish and plus one more for the rule.</p><p>In the second test the fitting sequences of choice are 4 2 1 or 2 1 4. In both cases we get satisfaction 7 for dishes and also, if we fulfill rule 1, we get an additional satisfaction 5.</p>
