## Description

<div><p>You have <span class="tex-span"><i>r</i></span> red, <span class="tex-span"><i>g</i></span> green and <span class="tex-span"><i>b</i></span> blue balloons. To decorate a single table for the banquet you need exactly three balloons. Three balloons attached to some table shouldn't have the same color. What maximum number <span class="tex-span"><i>t</i></span> of tables can be decorated if we know number of balloons of each color?</p><p>Your task is to write a program that for given values <span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>g</i></span> and <span class="tex-span"><i>b</i></span> will find the maximum number <span class="tex-span"><i>t</i></span> of tables, that can be decorated in the required manner.</p></div><div class="input-specification"><p>The single line contains three integers <span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>g</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">0 ≤ <i>r</i>, <i>g</i>, <i>b</i> ≤ 2·10<sup class="upper-index">9</sup></span>) — the number of red, green and blue baloons respectively. The numbers are separated by exactly one space.</p></div><div class="output-specification"><p>Print a single integer <span class="tex-span"><i>t</i></span> — the maximum number of tables that can be decorated in the required manner.</p></div>

## Input

<p>The single line contains three integers <span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>g</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">0 ≤ <i>r</i>, <i>g</i>, <i>b</i> ≤ 2·10<sup class="upper-index">9</sup></span>) — the number of red, green and blue baloons respectively. The numbers are separated by exactly one space.</p>

## Output

<p>Print a single integer <span class="tex-span"><i>t</i></span> — the maximum number of tables that can be decorated in the required manner.</p>





```input1
5 4 3

```




```input2
1 1 1

```




```input3
2 3 3

```




```output1
4

```




```output2
1

```




```output3
2

```



## Note

<p>In the first sample you can decorate the tables with the following balloon sets: "<span class="tex-font-style-tt">rgg</span>", "<span class="tex-font-style-tt">gbb</span>", "<span class="tex-font-style-tt">brr</span>", "<span class="tex-font-style-tt">rrg</span>", where "<span class="tex-font-style-tt">r</span>", "<span class="tex-font-style-tt">g</span>" and "<span class="tex-font-style-tt">b</span>" represent the red, green and blue balls, respectively.</p>
