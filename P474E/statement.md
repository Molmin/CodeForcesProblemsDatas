## Description

<div><p>Marmot found a row with <span class="tex-span"><i>n</i></span> pillars. The <span class="tex-span"><i>i</i></span>-th pillar has the height of <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> meters. Starting from one pillar <span class="tex-span"><i>i</i><sub class="lower-index">1</sub></span>, Marmot wants to jump on the pillars <span class="tex-span"><i>i</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>i</i><sub class="lower-index"><i>k</i></sub></span>. (<span class="tex-span">1 ≤ <i>i</i><sub class="lower-index">1</sub> &lt; <i>i</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>i</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i></span>). From a pillar <span class="tex-span"><i>i</i></span> Marmot can jump on a pillar <span class="tex-span"><i>j</i></span> only if <span class="tex-span"><i>i</i> &lt; <i>j</i></span> and <span class="tex-span">|<i>h</i><sub class="lower-index"><i>i</i></sub> - <i>h</i><sub class="lower-index"><i>j</i></sub>| ≥ <i>d</i></span>, where <span class="tex-span">|<i>x</i>|</span> is the absolute value of the number <span class="tex-span"><i>x</i></span>.</p><p>Now Marmot is asking you find out a jump sequence with maximal length and print it.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>d</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>h</i><sub class="lower-index">1</sub>, <i>h</i><sub class="lower-index">2</sub>, ..., <i>h</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">15</sup></span>).</p></div><div class="output-specification"><p>The first line should contain one integer <span class="tex-span"><i>k</i></span>, the maximal length of a jump sequence.</p><p>The second line should contain <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>i</i><sub class="lower-index">1</sub>, <i>i</i><sub class="lower-index">2</sub>, ..., <i>i</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i><sub class="lower-index">1</sub> &lt; <i>i</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>i</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i></span>), representing the pillars' indices from the maximal length jump sequence.</p><p>If there is more than one maximal length jump sequence, print any.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>d</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>h</i><sub class="lower-index">1</sub>, <i>h</i><sub class="lower-index">2</sub>, ..., <i>h</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">15</sup></span>).</p>

## Output

<p>The first line should contain one integer <span class="tex-span"><i>k</i></span>, the maximal length of a jump sequence.</p><p>The second line should contain <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>i</i><sub class="lower-index">1</sub>, <i>i</i><sub class="lower-index">2</sub>, ..., <i>i</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i><sub class="lower-index">1</sub> &lt; <i>i</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>i</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i></span>), representing the pillars' indices from the maximal length jump sequence.</p><p>If there is more than one maximal length jump sequence, print any.</p>





```input1
5 2
1 3 6 7 4

```




```input2
10 3
2 1 3 6 9 11 7 3 20 18

```




```output1
4
1 2 3 5 

```




```output2
6
1 4 6 7 8 9 

```



## Note

<p>In the first example Marmot chooses the pillars <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">3</span>, <span class="tex-span">5</span> with the heights <span class="tex-span">1</span>, <span class="tex-span">3</span>, <span class="tex-span">6</span>, <span class="tex-span">4</span>. Another jump sequence of length <span class="tex-span">4</span> is <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">4</span>, <span class="tex-span">5</span>.</p>
