## Description

<div><p>Little Petya loves training spiders. Petya has a board <span class="tex-span"><i>n</i> × <i>m</i></span> in size. Each cell of the board initially has a spider sitting on it. After one second Petya chooses a certain action for each spider, and all of them humbly perform its commands. There are 5 possible commands: to stay idle or to move from current cell to some of the four side-neighboring cells (that is, one command for each of the four possible directions). Petya gives the commands so that no spider leaves the field. It is allowed for spiders to pass through each other when they crawl towards each other in opposite directions. All spiders crawl simultaneously and several spiders may end up in one cell. Petya wants to know the maximum possible number of spider-free cells after one second.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 40, <i>n</i>·<i>m</i> ≤ 40</span>) — the board sizes.</p></div><div class="output-specification"><p>In the first line print the maximum number of cells without spiders.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 40, <i>n</i>·<i>m</i> ≤ 40</span>) — the board sizes.</p>

## Output

<p>In the first line print the maximum number of cells without spiders.</p>





```input1
1 1

```




```input2
2 3

```




```output1
0

```




```output2
4

```



## Note

<p>In the first sample the only possible answer is:</p><p><span class="tex-font-style-tt">s</span></p><p>In the second sample one of the possible solutions is: </p><pre class="verbatim"><br>rdl<br>rul<br></pre><p><span class="tex-font-style-tt">s</span> denotes command "stay idle", <span class="tex-font-style-tt">l, r, d, u</span> denote commands "crawl left", "crawl right", "crawl down", "crawl up", correspondingly.</p>
