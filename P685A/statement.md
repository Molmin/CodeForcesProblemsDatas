## Description

<div><p>Robbers, who attacked the Gerda's cab, are very successful in covering from the kingdom police. To make the goal of catching them even harder, they use their own watches.</p><p>First, as they know that kingdom police is bad at math, robbers use the positional numeral system <span class="tex-font-style-bf">with base <span class="tex-span">7</span></span>. Second, they divide one day in <span class="tex-span"><i>n</i></span> hours, and each hour in <span class="tex-span"><i>m</i></span> minutes. Personal watches of each robber are divided in two parts: first of them has the smallest possible number of places that is necessary to display any integer from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i> - 1</span>, while the second has the smallest possible number of places that is necessary to display any integer from <span class="tex-span">0</span> to <span class="tex-span"><i>m</i> - 1</span>. Finally, if some value of hours or minutes can be displayed using less number of places in base <span class="tex-span">7</span> than this watches have, the required number of zeroes is added at the beginning of notation.</p><p>Note that to display number <span class="tex-span">0</span> section of the watches is required to have at least one place.</p><p>Little robber wants to know the number of moments of time (particular values of hours and minutes), such that all digits displayed on the watches are <span class="tex-font-style-bf">distinct</span>. Help her calculate this number.</p></div><div class="input-specification"><p>The first line of the input contains two integers, given in the decimal notation, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of hours in one day and the number of minutes in one hour, respectively.</p></div><div class="output-specification"><p>Print one integer in decimal notation&nbsp;— the number of different pairs of hour and minute, such that all digits displayed on the watches are distinct.</p></div>

## Input

<p>The first line of the input contains two integers, given in the decimal notation, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of hours in one day and the number of minutes in one hour, respectively.</p>

## Output

<p>Print one integer in decimal notation&nbsp;— the number of different pairs of hour and minute, such that all digits displayed on the watches are distinct.</p>





```input1
2 3

```




```input2
8 2

```




```output1
4

```




```output2
5

```



## Note

<p>In the first sample, possible pairs are: <span class="tex-span">(0: 1)</span>, <span class="tex-span">(0: 2)</span>, <span class="tex-span">(1: 0)</span>, <span class="tex-span">(1: 2)</span>.</p><p>In the second sample, possible pairs are: <span class="tex-span">(02: 1)</span>, <span class="tex-span">(03: 1)</span>, <span class="tex-span">(04: 1)</span>, <span class="tex-span">(05: 1)</span>, <span class="tex-span">(06: 1)</span>.</p>
