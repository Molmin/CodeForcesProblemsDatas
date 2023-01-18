## Description

<div><p>You took a peek on Thanos wearing Infinity Gauntlet. In the Gauntlet there is a place for six Infinity Gems:</p><ul> <li> the <span class="tex-font-style-tt">Power</span> Gem of <span class="tex-font-style-tt">purple</span> color, </li><li> the <span class="tex-font-style-tt">Time</span> Gem of <span class="tex-font-style-tt">green</span> color, </li><li> the <span class="tex-font-style-tt">Space</span> Gem of <span class="tex-font-style-tt">blue</span> color, </li><li> the <span class="tex-font-style-tt">Soul</span> Gem of <span class="tex-font-style-tt">orange</span> color, </li><li> the <span class="tex-font-style-tt">Reality</span> Gem of <span class="tex-font-style-tt">red</span> color, </li><li> the <span class="tex-font-style-tt">Mind</span> Gem of <span class="tex-font-style-tt">yellow</span> color. </li></ul><p>Using colors of Gems you saw in the Gauntlet determine the names of <span class="tex-font-style-bf">absent</span> Gems.</p></div><div class="input-specification"><p>In the first line of input there is one integer $n$ ($0 \le n \le 6$)&nbsp;— the number of Gems in Infinity Gauntlet.</p><p>In next $n$ lines there are colors of Gems you saw. Words used for colors are: <span class="tex-font-style-tt">purple</span>, <span class="tex-font-style-tt">green</span>, <span class="tex-font-style-tt">blue</span>, <span class="tex-font-style-tt">orange</span>, <span class="tex-font-style-tt">red</span>, <span class="tex-font-style-tt">yellow</span>. It is guaranteed that all the colors are <span class="tex-font-style-bf">distinct</span>. All colors are given in lowercase English letters.</p></div><div class="output-specification"><p>In the first line output one integer $m$ ($0 \le m \le 6$)&nbsp;— the number of absent Gems.</p><p>Then in $m$ lines print the names of absent Gems, each on its own line. Words used for names are: <span class="tex-font-style-tt">Power</span>, <span class="tex-font-style-tt">Time</span>, <span class="tex-font-style-tt">Space</span>, <span class="tex-font-style-tt">Soul</span>, <span class="tex-font-style-tt">Reality</span>, <span class="tex-font-style-tt">Mind</span>. Names can be printed in any order. Keep the first letter uppercase, others lowercase.</p></div>

## Input

<p>In the first line of input there is one integer $n$ ($0 \le n \le 6$)&nbsp;— the number of Gems in Infinity Gauntlet.</p><p>In next $n$ lines there are colors of Gems you saw. Words used for colors are: <span class="tex-font-style-tt">purple</span>, <span class="tex-font-style-tt">green</span>, <span class="tex-font-style-tt">blue</span>, <span class="tex-font-style-tt">orange</span>, <span class="tex-font-style-tt">red</span>, <span class="tex-font-style-tt">yellow</span>. It is guaranteed that all the colors are <span class="tex-font-style-bf">distinct</span>. All colors are given in lowercase English letters.</p>

## Output

<p>In the first line output one integer $m$ ($0 \le m \le 6$)&nbsp;— the number of absent Gems.</p><p>Then in $m$ lines print the names of absent Gems, each on its own line. Words used for names are: <span class="tex-font-style-tt">Power</span>, <span class="tex-font-style-tt">Time</span>, <span class="tex-font-style-tt">Space</span>, <span class="tex-font-style-tt">Soul</span>, <span class="tex-font-style-tt">Reality</span>, <span class="tex-font-style-tt">Mind</span>. Names can be printed in any order. Keep the first letter uppercase, others lowercase.</p>





```input1
4
red
purple
yellow
orange

```




```input2
0

```




```output1
2
Space
Time

```




```output2
6
Time
Mind
Soul
Power
Reality
Space

```



## Note

<p>In the first sample Thanos already has <span class="tex-font-style-tt">Reality</span>, <span class="tex-font-style-tt">Power</span>, <span class="tex-font-style-tt">Mind</span> and <span class="tex-font-style-tt">Soul</span> Gems, so he needs two more: <span class="tex-font-style-tt">Time</span> and <span class="tex-font-style-tt">Space</span>.</p><p>In the second sample Thanos doesn't have any Gems, so he needs all six.</p>
