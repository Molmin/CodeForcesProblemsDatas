## Description

<div><p>Vasya wants to turn on Christmas lights consisting of <span class="tex-span"><i>m</i></span> bulbs. Initially, all bulbs are turned off. There are <span class="tex-span"><i>n</i></span> buttons, each of them is connected to some set of bulbs. Vasya can press any of these buttons. When the button is pressed, it turns on all the bulbs it's connected to. Can Vasya light up all the bulbs?</p><p>If Vasya presses the button such that some bulbs connected to it are already turned on, they do not change their state, i.e. remain turned on.</p></div><div class="input-specification"><p>The first line of the input contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>)&nbsp;— the number of buttons and the number of bulbs respectively. </p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>)&nbsp;— the number of bulbs that are turned on by the <span class="tex-span"><i>i</i></span>-th button, and then <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> numbers <span class="tex-span"><i>y</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">1 ≤ <i>y</i><sub class="lower-index"><i>ij</i></sub> ≤ <i>m</i></span>)&nbsp;— the numbers of these bulbs.</p></div><div class="output-specification"><p>If it's possible to turn on all <span class="tex-span"><i>m</i></span> bulbs print "<span class="tex-font-style-tt">YES</span>", otherwise print "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>The first line of the input contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>)&nbsp;— the number of buttons and the number of bulbs respectively. </p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>)&nbsp;— the number of bulbs that are turned on by the <span class="tex-span"><i>i</i></span>-th button, and then <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> numbers <span class="tex-span"><i>y</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">1 ≤ <i>y</i><sub class="lower-index"><i>ij</i></sub> ≤ <i>m</i></span>)&nbsp;— the numbers of these bulbs.</p>

## Output

<p>If it's possible to turn on all <span class="tex-span"><i>m</i></span> bulbs print "<span class="tex-font-style-tt">YES</span>", otherwise print "<span class="tex-font-style-tt">NO</span>".</p>





```input1
3 4
2 1 4
3 1 3 1
1 2

```




```input2
3 3
1 1
1 2
1 1

```




```output1
YES

```




```output2
NO

```



## Note

<p>In the first sample you can press each button once and turn on all the bulbs. In the 2 sample it is impossible to turn on the 3-rd lamp.</p>
