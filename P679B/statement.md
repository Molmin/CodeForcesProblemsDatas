## Description

<div><p>Limak is a little polar bear. He plays by building towers from blocks. Every block is a cube with positive integer length of side. Limak has infinitely many blocks of each side length.</p><p>A block with side <span class="tex-span"><i>a</i></span> has volume <span class="tex-span"><i>a</i><sup class="upper-index">3</sup></span>. A tower consisting of blocks with sides <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span> has the total volume <span class="tex-span"><i>a</i><sub class="lower-index">1</sub><sup class="upper-index">3</sup> + <i>a</i><sub class="lower-index">2</sub><sup class="upper-index">3</sup> + ... + <i>a</i><sub class="lower-index"><i>k</i></sub><sup class="upper-index">3</sup></span>.</p><p>Limak is going to build a tower. First, he asks you to tell him a positive integer <span class="tex-span"><i>X</i></span>&nbsp;— the required total volume of the tower. Then, Limak adds new blocks greedily, one by one. Each time he adds the biggest block such that the total volume doesn't exceed <span class="tex-span"><i>X</i></span>.</p><p>Limak asks you to choose <span class="tex-span"><i>X</i></span> not greater than <span class="tex-span"><i>m</i></span>. Also, he wants to maximize the number of blocks in the tower at the end (however, he still behaves greedily). Secondarily, he wants to maximize <span class="tex-span"><i>X</i></span>.</p><p>Can you help Limak? Find the maximum number of blocks his tower can have and the maximum <span class="tex-span"><i>X</i> ≤ <i>m</i></span> that results this number of blocks.</p></div><div class="input-specification"><p>The only line of the input contains one integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">15</sup></span>), meaning that Limak wants you to choose <span class="tex-span"><i>X</i></span> between <span class="tex-span">1</span> and <span class="tex-span"><i>m</i></span>, inclusive.</p></div><div class="output-specification"><p>Print two integers&nbsp;— the maximum number of blocks in the tower and the maximum required total volume <span class="tex-span"><i>X</i></span>, resulting in the maximum number of blocks.</p></div>

## Input

<p>The only line of the input contains one integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">15</sup></span>), meaning that Limak wants you to choose <span class="tex-span"><i>X</i></span> between <span class="tex-span">1</span> and <span class="tex-span"><i>m</i></span>, inclusive.</p>

## Output

<p>Print two integers&nbsp;— the maximum number of blocks in the tower and the maximum required total volume <span class="tex-span"><i>X</i></span>, resulting in the maximum number of blocks.</p>





```input1
48

```




```input2
6

```




```output1
9 42

```




```output2
6 6

```



## Note

<p>In the first sample test, there will be <span class="tex-span">9</span> blocks if you choose <span class="tex-span"><i>X</i> = 23</span> or <span class="tex-span"><i>X</i> = 42</span>. Limak wants to maximize <span class="tex-span"><i>X</i></span> secondarily so you should choose <span class="tex-span">42</span>.</p><p>In more detail, after choosing <span class="tex-span"><i>X</i> = 42</span> the process of building a tower is:</p><ul> <li> Limak takes a block with side <span class="tex-span">3</span> because it's the biggest block with volume not greater than <span class="tex-span">42</span>. The remaining volume is <span class="tex-span">42 - 27 = 15</span>. </li><li> The second added block has side <span class="tex-span">2</span>, so the remaining volume is <span class="tex-span">15 - 8 = 7</span>. </li><li> Finally, Limak adds <span class="tex-span">7</span> blocks with side <span class="tex-span">1</span>, one by one. </li></ul><p>So, there are <span class="tex-span">9</span> blocks in the tower. The total volume is is <span class="tex-span">3<sup class="upper-index">3</sup> + 2<sup class="upper-index">3</sup> + 7·1<sup class="upper-index">3</sup> = 27 + 8 + 7 = 42</span>.</p>
