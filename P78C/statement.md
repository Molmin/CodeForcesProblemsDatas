## Description

<div><p>Two beavers, Timur and Marsel, play the following game.</p><p>There are <span class="tex-span"><i>n</i></span> logs, each of exactly <span class="tex-span"><i>m</i></span> meters in length. The beavers move in turns. For each move a beaver chooses a log and gnaws it into some number (more than one) of <span class="tex-font-style-bf">equal</span> parts, the length of each one is expressed by an integer and is no less than <span class="tex-span"><i>k</i></span> meters. Each resulting part is also a log which can be gnawed in future by any beaver. The beaver that can't make a move loses. Thus, the other beaver wins.</p><p>Timur makes the first move. The players play in the optimal way. Determine the winner.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">Timur</span>", if Timur wins, or "<span class="tex-font-style-tt">Marsel</span>", if Marsel wins. You should print everything without the quotes. </p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print "<span class="tex-font-style-tt">Timur</span>", if Timur wins, or "<span class="tex-font-style-tt">Marsel</span>", if Marsel wins. You should print everything without the quotes. </p>





```input1
1 15 4

```




```input2
4 9 5

```




```output1
Timur
```




```output2
Marsel
```



## Note

<p>In the first sample the beavers only have one log, of <span class="tex-span">15</span> meters in length. Timur moves first. The only move he can do is to split the log into <span class="tex-span">3</span> parts each <span class="tex-span">5</span> meters in length. Then Marsel moves but he can't split any of the resulting logs, as <span class="tex-span"><i>k</i> = 4</span>. Thus, the winner is Timur.</p><p>In the second example the beavers have <span class="tex-span">4</span> logs <span class="tex-span">9</span> meters in length. Timur can't split any of them, so that the resulting parts possessed the length of not less than <span class="tex-span">5</span> meters, that's why he loses instantly.</p>
