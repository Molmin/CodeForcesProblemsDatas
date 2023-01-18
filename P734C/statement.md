## Description

<div><p>Anton is playing a very interesting computer game, but now he is stuck at one of the levels. To pass to the next level he has to prepare <span class="tex-span"><i>n</i></span> potions.</p><p>Anton has a special kettle, that can prepare one potions in <span class="tex-span"><i>x</i></span> seconds. Also, he knows spells of two types that can faster the process of preparing potions.</p><ol> <li> Spells of this type speed up the preparation time of one potion. There are <span class="tex-span"><i>m</i></span> spells of this type, the <span class="tex-span"><i>i</i></span>-th of them costs <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> manapoints and changes the preparation time of each potion to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> instead of <span class="tex-span"><i>x</i></span>. </li><li> Spells of this type immediately prepare some number of potions. There are <span class="tex-span"><i>k</i></span> such spells, the <span class="tex-span"><i>i</i></span>-th of them costs <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> manapoints and instantly create <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> potions. </li></ol><p>Anton can use <span class="tex-font-style-bf">no more than one</span> spell of the first type and <span class="tex-font-style-bf">no more than one</span> spell of the second type, and the total number of manapoints spent should not exceed <span class="tex-span"><i>s</i></span>. Consider that all spells are used instantly and right before Anton starts to prepare potions.</p><p>Anton wants to get to the next level as fast as possible, so he is interested in the minimum number of time he needs to spent in order to prepare at least <span class="tex-span"><i>n</i></span> potions.</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">9</sup>, 1 ≤ <i>m</i>, <i>k</i> ≤ 2·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of potions, Anton has to make, the number of spells of the first type and the number of spells of the second type.</p><p>The second line of the input contains two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">2 ≤ <i>x</i> ≤ 2·10<sup class="upper-index">9</sup>, 1 ≤ <i>s</i> ≤ 2·10<sup class="upper-index">9</sup></span>)&nbsp;— the initial number of seconds required to prepare one potion and the number of manapoints Anton can use.</p><p>The third line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>x</i></span>)&nbsp;— the number of seconds it will take to prepare one potion if the <span class="tex-span"><i>i</i></span>-th spell of the first type is used.</p><p>The fourth line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">9</sup></span>)&nbsp;— the number of manapoints to use the <span class="tex-span"><i>i</i></span>-th spell of the first type.</p><p>There are <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) in the fifth line&nbsp;— the number of potions that will be immediately created if the <span class="tex-span"><i>i</i></span>-th spell of the second type is used. It's guaranteed that <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> are <span class="tex-font-style-bf">not decreasing</span>, i.e. <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>c</i><sub class="lower-index"><i>j</i></sub></span> if <span class="tex-span"><i>i</i> &lt; <i>j</i></span>.</p><p>The sixth line contains <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">9</sup></span>)&nbsp;— the number of manapoints required to use the <span class="tex-span"><i>i</i></span>-th spell of the second type. It's guaranteed that <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> are <span class="tex-font-style-bf">not decreasing</span>, i.e. <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub> ≤ <i>d</i><sub class="lower-index"><i>j</i></sub></span> if <span class="tex-span"><i>i</i> &lt; <i>j</i></span>.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the minimum time one has to spent in order to prepare <span class="tex-span"><i>n</i></span> potions.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">9</sup>, 1 ≤ <i>m</i>, <i>k</i> ≤ 2·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of potions, Anton has to make, the number of spells of the first type and the number of spells of the second type.</p><p>The second line of the input contains two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">2 ≤ <i>x</i> ≤ 2·10<sup class="upper-index">9</sup>, 1 ≤ <i>s</i> ≤ 2·10<sup class="upper-index">9</sup></span>)&nbsp;— the initial number of seconds required to prepare one potion and the number of manapoints Anton can use.</p><p>The third line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>x</i></span>)&nbsp;— the number of seconds it will take to prepare one potion if the <span class="tex-span"><i>i</i></span>-th spell of the first type is used.</p><p>The fourth line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">9</sup></span>)&nbsp;— the number of manapoints to use the <span class="tex-span"><i>i</i></span>-th spell of the first type.</p><p>There are <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) in the fifth line&nbsp;— the number of potions that will be immediately created if the <span class="tex-span"><i>i</i></span>-th spell of the second type is used. It's guaranteed that <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> are <span class="tex-font-style-bf">not decreasing</span>, i.e. <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>c</i><sub class="lower-index"><i>j</i></sub></span> if <span class="tex-span"><i>i</i> &lt; <i>j</i></span>.</p><p>The sixth line contains <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">9</sup></span>)&nbsp;— the number of manapoints required to use the <span class="tex-span"><i>i</i></span>-th spell of the second type. It's guaranteed that <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> are <span class="tex-font-style-bf">not decreasing</span>, i.e. <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub> ≤ <i>d</i><sub class="lower-index"><i>j</i></sub></span> if <span class="tex-span"><i>i</i> &lt; <i>j</i></span>.</p>

## Output

<p>Print one integer&nbsp;— the minimum time one has to spent in order to prepare <span class="tex-span"><i>n</i></span> potions.</p>





```input1
20 3 2
10 99
2 4 3
20 10 40
4 15
10 80

```




```input2
20 3 2
10 99
2 4 3
200 100 400
4 15
100 800

```




```output1
20

```




```output2
200

```



## Note

<p>In the first sample, the optimum answer is to use the second spell of the first type that costs <span class="tex-span">10</span> manapoints. Thus, the preparation time of each potion changes to <span class="tex-span">4</span> seconds. Also, Anton should use the second spell of the second type to instantly prepare <span class="tex-span">15</span> potions spending <span class="tex-span">80</span> manapoints. The total number of manapoints used is <span class="tex-span">10 + 80 = 90</span>, and the preparation time is <span class="tex-span">4·5 = 20</span> seconds (<span class="tex-span">15</span> potions were prepared instantly, and the remaining <span class="tex-span">5</span> will take <span class="tex-span">4</span> seconds each).</p><p>In the second sample, Anton can't use any of the spells, so he just prepares <span class="tex-span">20</span> potions, spending <span class="tex-span">10</span> seconds on each of them and the answer is <span class="tex-span">20·10 = 200</span>.</p>
