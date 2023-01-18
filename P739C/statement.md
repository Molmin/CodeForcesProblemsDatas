## Description

<div><p>Alyona has built <span class="tex-span"><i>n</i></span> towers by putting small cubes some on the top of others. Each cube has size <span class="tex-span">1 × 1 × 1</span>. A tower is a non-zero amount of cubes standing on the top of each other. The towers are next to each other, forming a row.</p><p>Sometimes Alyona chooses some segment towers, and put on the top of each tower several cubes. Formally, Alyouna chooses some segment of towers from <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and adds <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> cubes on the top of them.</p><p>Let the sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> be the heights of the towers from left to right. Let's call as a segment of towers <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i></sub>, <i>a</i><sub class="lower-index"><i>l</i> + 1</sub>, ..., <i>a</i><sub class="lower-index"><i>r</i></sub></span> a hill if the following condition holds: there is integer <span class="tex-span"><i>k</i></span> (<span class="tex-span"><i>l</i> ≤ <i>k</i> ≤ <i>r</i></span>) such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i></sub> &lt; <i>a</i><sub class="lower-index"><i>l</i> + 1</sub> &lt; <i>a</i><sub class="lower-index"><i>l</i> + 2</sub> &lt; ... &lt; <i>a</i><sub class="lower-index"><i>k</i></sub> &gt; <i>a</i><sub class="lower-index"><i>k</i> + 1</sub> &gt; <i>a</i><sub class="lower-index"><i>k</i> + 2</sub> &gt; ... &gt; <i>a</i><sub class="lower-index"><i>r</i></sub></span>.</p><p>After each addition of <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> cubes on the top of the towers from <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, Alyona wants to know the maximum width among all hills. The width of a hill is the number of towers in it.</p></div><div class="input-specification"><p>The first line contain single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of towers.</p><p>The second line contain <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of cubes in each tower. </p><p>The third line contain single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of additions.</p><p>The next <span class="tex-span"><i>m</i></span> lines contain <span class="tex-span">3</span> integers each. The <span class="tex-span"><i>i</i></span>-th of these lines contains integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), that mean that Alyona puts <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> cubes on the tio of each of the towers from <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> lines. In <span class="tex-span"><i>i</i></span>-th line print the maximum width of the hills after the <span class="tex-span"><i>i</i></span>-th addition.</p></div>

## Input

<p>The first line contain single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of towers.</p><p>The second line contain <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of cubes in each tower. </p><p>The third line contain single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of additions.</p><p>The next <span class="tex-span"><i>m</i></span> lines contain <span class="tex-span">3</span> integers each. The <span class="tex-span"><i>i</i></span>-th of these lines contains integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), that mean that Alyona puts <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> cubes on the tio of each of the towers from <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> lines. In <span class="tex-span"><i>i</i></span>-th line print the maximum width of the hills after the <span class="tex-span"><i>i</i></span>-th addition.</p>





```input1
5
5 5 5 5 5
3
1 3 2
2 2 1
4 4 1

```




```output1
2
4
5

```



## Note

<p>The first sample is as follows:</p><p>After addition of <span class="tex-span">2</span> cubes on the top of each towers from the first to the third, the number of cubes in the towers become equal to <span class="tex-span">[7, 7, 7, 5, 5]</span>. The hill with maximum width is <span class="tex-span">[7, 5]</span>, thus the maximum width is <span class="tex-span">2</span>.</p><p>After addition of <span class="tex-span">1</span> cube on the second tower, the number of cubes in the towers become equal to <span class="tex-span">[7, 8, 7, 5, 5]</span>. The hill with maximum width is now <span class="tex-span">[7, 8, 7, 5]</span>, thus the maximum width is <span class="tex-span">4</span>.</p><p>After addition of <span class="tex-span">1</span> cube on the fourth tower, the number of cubes in the towers become equal to <span class="tex-span">[7, 8, 7, 6, 5]</span>. The hill with maximum width is now <span class="tex-span">[7, 8, 7, 6, 5]</span>, thus the maximum width is <span class="tex-span">5</span>.</p>
