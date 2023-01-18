## Description

<div><p>Kalila and Dimna are two jackals living in a huge jungle. One day they decided to join a logging factory in order to make money. </p><p>The manager of logging factory wants them to go to the jungle and cut <span class="tex-span"><i>n</i></span> trees with heights <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. They bought a chain saw from a shop. Each time they use the chain saw on the tree number <span class="tex-span"><i>i</i></span>, they can decrease the height of this tree by one unit. Each time that Kalila and Dimna use the chain saw, they need to recharge it. Cost of charging depends on the id of the trees which have been cut completely (a tree is cut completely if its height equal to 0). If the maximum id of a tree which has been cut completely is <span class="tex-span"><i>i</i></span> (the tree that have height <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> in the beginning), then the cost of charging the chain saw would be <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. If no tree is cut completely, Kalila and Dimna cannot charge the chain saw. The chainsaw is charged in the beginning. We know that for each <span class="tex-span"><i>i</i></span> &lt; <span class="tex-span"><i>j</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>a</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> &gt; <i>b</i><sub class="lower-index"><i>j</i></sub></span> and also <span class="tex-span"><i>b</i><sub class="lower-index"><i>n</i></sub> = 0</span> and <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> = 1</span>. Kalila and Dimna want to cut all the trees completely, with minimum cost. </p><p>They want you to help them! Will you?</p></div><div class="input-specification"><p>The first line of input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The second line of input contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). The third line of input contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>It's guaranteed that <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> = 1</span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>n</i></sub> = 0</span>, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> &lt; <i>a</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>a</i><sub class="lower-index"><i>n</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index">1</sub> &gt; <i>b</i><sub class="lower-index">2</sub> &gt; ... &gt; <i>b</i><sub class="lower-index"><i>n</i></sub></span>.</p></div><div class="output-specification"><p>The only line of output must contain the minimum cost of cutting all the trees completely.</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line of input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The second line of input contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). The third line of input contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>It's guaranteed that <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> = 1</span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>n</i></sub> = 0</span>, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> &lt; <i>a</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>a</i><sub class="lower-index"><i>n</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index">1</sub> &gt; <i>b</i><sub class="lower-index">2</sub> &gt; ... &gt; <i>b</i><sub class="lower-index"><i>n</i></sub></span>.</p>

## Output

<p>The only line of output must contain the minimum cost of cutting all the trees completely.</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
5
1 2 3 4 5
5 4 3 2 0

```




```input2
6
1 2 3 10 20 30
6 5 4 3 2 0

```




```output1
25

```




```output2
138

```


