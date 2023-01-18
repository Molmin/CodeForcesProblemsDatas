## Description

<div><p>One day Kefa found <span class="tex-span"><i>n</i></span> baloons. For convenience, we denote color of <span class="tex-span"><i>i</i></span>-th baloon as <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> — lowercase letter of the Latin alphabet. Also Kefa has <span class="tex-span"><i>k</i></span> friends. Friend will be upset, If he get two baloons of the same color. Kefa want to give out <span class="tex-font-style-bf">all</span> baloons to his friends. Help Kefa to find out, can he give out all his baloons, such that no one of his friens will be upset — print «<span class="tex-font-style-tt">YES</span>», if he can, and «<span class="tex-font-style-tt">NO</span>», otherwise. Note, that Kefa's friend will not upset, if he doesn't get baloons at all.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 100</span>) — the number of baloons and friends.</p><p>Next line contains string <span class="tex-span"><i>s</i></span> — colors of baloons.</p></div><div class="output-specification"><p>Answer to the task — «<span class="tex-font-style-tt">YES</span>» or «<span class="tex-font-style-tt">NO</span>» in a single line.</p><p>You can choose the case (lower or upper) for each letter arbitrary.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 100</span>) — the number of baloons and friends.</p><p>Next line contains string <span class="tex-span"><i>s</i></span> — colors of baloons.</p>

## Output

<p>Answer to the task — «<span class="tex-font-style-tt">YES</span>» or «<span class="tex-font-style-tt">NO</span>» in a single line.</p><p>You can choose the case (lower or upper) for each letter arbitrary.</p>





```input1
4 2
aabb

```




```input2
6 3
aacaab

```




```output1
YES

```




```output2
NO

```



## Note

<p>In the first sample Kefa can give <span class="tex-span">1</span>-st and <span class="tex-span">3</span>-rd baloon to the first friend, and <span class="tex-span">2</span>-nd and <span class="tex-span">4</span>-th to the second.</p><p>In the second sample Kefa needs to give to all his friends baloons of color <span class="tex-font-style-it">a</span>, but one baloon will stay, thats why answer is «<span class="tex-font-style-tt">NO</span>».</p>
