## Description

<div><p>Recently, Dima met with Sasha in a philatelic store, and since then they are collecting coins together. Their favorite occupation is to sort collections of coins. Sasha likes having things in order, that is why he wants his coins to be arranged in a row in such a way that firstly come coins out of circulation, and then come coins still in circulation. </p><p>For arranging coins Dima uses the following algorithm. One step of his algorithm looks like the following:</p><ol> <li> He looks through all the coins from left to right; </li><li> If he sees that the <span class="tex-span"><i>i</i></span>-th coin is still in circulation, and <span class="tex-span">(<i>i</i> + 1)</span>-th coin is already out of circulation, he exchanges these two coins and continues watching coins from <span class="tex-span">(<i>i</i> + 1)</span>-th. </li></ol> <p>Dima repeats the procedure above until it happens that no two coins were exchanged during this procedure. Dima calls <span class="tex-font-style-it">hardness of ordering</span> the number of steps required for him according to the algorithm above to sort the sequence, e.g. the number of times he looks through the coins from the very beginning. For example, for the ordered sequence hardness of ordering equals one.</p><p>Today Sasha invited Dima and proposed him a game. First he puts <span class="tex-span"><i>n</i></span> coins in a row, all of them are out of circulation. Then Sasha chooses one of the coins out of circulation and replaces it with a coin in circulation for <span class="tex-span"><i>n</i></span> times. During this process Sasha constantly asks Dima what is the hardness of ordering of the sequence. </p><p>The task is more complicated because Dima should not touch the coins and he should determine hardness of ordering in his mind. Help Dima with this task. </p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300 000</span>)&nbsp;— number of coins that Sasha puts behind Dima.</p><p>Second line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— positions that Sasha puts coins in circulation to. At first Sasha replaces coin located at position <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span>, then coin located at position <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span> and so on. Coins are numbered from left to right.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i> + 1</span> numbers <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index">0</sub></span> is a hardness of ordering at the beginning, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> is a hardness of ordering after the first replacement and so on. </p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300 000</span>)&nbsp;— number of coins that Sasha puts behind Dima.</p><p>Second line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— positions that Sasha puts coins in circulation to. At first Sasha replaces coin located at position <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span>, then coin located at position <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span> and so on. Coins are numbered from left to right.</p>

## Output

<p>Print <span class="tex-span"><i>n</i> + 1</span> numbers <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index">0</sub></span> is a hardness of ordering at the beginning, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> is a hardness of ordering after the first replacement and so on. </p>





```input1
4
1 3 4 2

```




```input2
8
6 8 3 4 7 2 1 5

```




```output1
1 2 3 2 1

```




```output2
1 2 2 3 4 3 4 5 1

```



## Note

<p>Let's denote as <span class="tex-font-style-tt">O</span> coin out of circulation, and as <span class="tex-font-style-tt">X</span> — coin is circulation.</p><p>At the first sample, initially in row there are coins that are not in circulation, so Dima will look through them from left to right and won't make any exchanges.</p><p>After replacement of the first coin with a coin in circulation, Dima will exchange this coin with next three times and after that he will finally look through the coins and finish the process.</p><p><span class="tex-font-style-tt">XOOO</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt">OOOX</span></p><p>After replacement of the third coin, Dima's actions look this way:</p><p><span class="tex-font-style-tt">XOXO</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt">OXOX</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt">OOXX</span></p><p>After replacement of the fourth coin, Dima's actions look this way:</p><p><span class="tex-font-style-tt">XOXX</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt">OXXX</span></p><p>Finally, after replacement of the second coin, row becomes consisting of coins that are in circulation and Dima will look through coins from left to right without any exchanges.</p>
