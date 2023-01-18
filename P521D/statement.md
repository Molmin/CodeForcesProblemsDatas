## Description

<div><p>Vasya plays one very well-known and extremely popular MMORPG game. His game character has <span class="tex-span"><i>k</i></span> skill; currently the <span class="tex-span"><i>i</i></span>-th of them equals to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. Also this game has a common rating table in which the participants are ranked according to the <span class="tex-font-style-bf">product</span> of all the skills of a hero in the descending order.</p><p>Vasya decided to 'upgrade' his character via the game store. This store offers <span class="tex-span"><i>n</i></span> possible ways to improve the hero's skills; Each of these ways belongs to one of three types:</p><ol> <li> assign the <span class="tex-span"><i>i</i></span>-th skill to <span class="tex-span"><i>b</i></span>; </li><li> add <span class="tex-span"><i>b</i></span> to the <span class="tex-span"><i>i</i></span>-th skill; </li><li> multiply the <span class="tex-span"><i>i</i></span>-th skill by <span class="tex-span"><i>b</i></span>. </li></ol><p>Unfortunately, a) every improvement can only be used once; b) the money on Vasya's card is enough only to purchase not more than <span class="tex-span"><i>m</i></span> of the <span class="tex-span"><i>n</i></span> improvements. Help Vasya to reach the highest ranking in the game. To do this tell Vasya which of improvements he has to purchase and in what order he should use them to make his rating become as high as possible. If there are several ways to achieve it, print any of them.</p></div><div class="input-specification"><p>The first line contains three numbers — <span class="tex-span"><i>k</i>, <i>n</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of skills, the number of improvements on sale and the number of them Vasya can afford.</p><p>The second line contains <span class="tex-span"><i>k</i></span> space-separated numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>), the initial values of skills.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span">3</span> space-separated numbers <span class="tex-span"><i>t</i><sub class="lower-index"><i>j</i></sub>, <i>i</i><sub class="lower-index"><i>j</i></sub>, <i>b</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>j</i></sub> ≤ 3, 1 ≤ <i>i</i><sub class="lower-index"><i>j</i></sub> ≤ <i>k</i>, 1 ≤ <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the type of the <span class="tex-span"><i>j</i></span>-th improvement (1 for assigning, 2 for adding, 3 for multiplying), the skill to which it can be applied and the value of <span class="tex-span"><i>b</i></span> for this improvement.</p></div><div class="output-specification"><p>The first line should contain a number <span class="tex-span"><i>l</i></span> (<span class="tex-span">0 ≤ <i>l</i> ≤ <i>m</i></span>) — the number of improvements you should use.</p><p>The second line should contain <span class="tex-span"><i>l</i></span> distinct space-separated numbers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the indices of improvements in the order in which they should be applied. The improvements are numbered starting from <span class="tex-span">1</span>, in the order in which they appear in the input. </p></div>

## Input

<p>The first line contains three numbers — <span class="tex-span"><i>k</i>, <i>n</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of skills, the number of improvements on sale and the number of them Vasya can afford.</p><p>The second line contains <span class="tex-span"><i>k</i></span> space-separated numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>), the initial values of skills.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span">3</span> space-separated numbers <span class="tex-span"><i>t</i><sub class="lower-index"><i>j</i></sub>, <i>i</i><sub class="lower-index"><i>j</i></sub>, <i>b</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>j</i></sub> ≤ 3, 1 ≤ <i>i</i><sub class="lower-index"><i>j</i></sub> ≤ <i>k</i>, 1 ≤ <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the type of the <span class="tex-span"><i>j</i></span>-th improvement (1 for assigning, 2 for adding, 3 for multiplying), the skill to which it can be applied and the value of <span class="tex-span"><i>b</i></span> for this improvement.</p>

## Output

<p>The first line should contain a number <span class="tex-span"><i>l</i></span> (<span class="tex-span">0 ≤ <i>l</i> ≤ <i>m</i></span>) — the number of improvements you should use.</p><p>The second line should contain <span class="tex-span"><i>l</i></span> distinct space-separated numbers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the indices of improvements in the order in which they should be applied. The improvements are numbered starting from <span class="tex-span">1</span>, in the order in which they appear in the input. </p>





```input1
2 4 3
13 20
1 1 14
1 2 30
2 1 6
3 2 2

```




```output1
3
2 3 4

```


