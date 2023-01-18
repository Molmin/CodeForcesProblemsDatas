## Description

<div><p><span class="tex-font-style-it">Nian is a monster which lives deep in the oceans. Once a year, it shows up on the land, devouring livestock and even people. In order to keep the monster away, people fill their villages with red colour, light, and cracking noise, all of which frighten the monster out of coming.</span></p><p>Little Tommy has <span class="tex-span"><i>n</i></span> lanterns and Big Banban has <span class="tex-span"><i>m</i></span> lanterns. Tommy's lanterns have brightness <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, and Banban's have brightness <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span> respectively.</p><p>Tommy intends to hide one of his lanterns, then Banban picks one of Tommy's non-hidden lanterns and one of his own lanterns to form a pair. The pair's brightness will be the product of the brightness of two lanterns.</p><p>Tommy wants to make the product as small as possible, while Banban tries to make it as large as possible.</p><p>You are asked to find the brightness of the chosen pair if both of them choose optimally.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 50</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>.</p><p>The third line contains <span class="tex-span"><i>m</i></span> space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span>.</p><p>All the integers range from <span class="tex-span"> - 10<sup class="upper-index">9</sup></span> to <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the brightness of the chosen pair.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 50</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>.</p><p>The third line contains <span class="tex-span"><i>m</i></span> space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span>.</p><p>All the integers range from <span class="tex-span"> - 10<sup class="upper-index">9</sup></span> to <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p>

## Output

<p>Print a single integer&nbsp;— the brightness of the chosen pair.</p>





```input1
2 2
20 18
2 14

```




```input2
5 3
-1 0 1 2 3
-1 0 1

```




```output1
252

```




```output2
2

```



## Note

<p>In the first example, Tommy will hide <span class="tex-span">20</span> and Banban will choose <span class="tex-span">18</span> from Tommy and <span class="tex-span">14</span> from himself.</p><p>In the second example, Tommy will hide <span class="tex-span">3</span> and Banban will choose <span class="tex-span">2</span> from Tommy and <span class="tex-span">1</span> from himself.</p>
