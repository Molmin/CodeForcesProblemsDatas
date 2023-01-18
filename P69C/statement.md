## Description

<div><p>In one school with Vasya there is a student Kostya. Kostya does not like physics, he likes different online games. Every day, having come home, Kostya throws his bag in the farthest corner and sits down at his beloved computer. Kostya even eats glued to the game. A few days ago Kostya bought a new RPG game "HaresButtle", which differs from all other games in this genre. It has a huge number of artifacts. As we know, artifacts are divided into basic and composite ones. Only the basic artifacts are available on sale. More powerful composite artifacts are collected from some number of basic artifacts.</p><p>After the composing composite artifact, all the components disappear.</p><p>Kostya is the head of the alliance, so he has to remember, what artifacts has not only himself, but also his allies. You must identify by sequence of artifacts purchased by Kostya and his allies, how many and which artifacts has been collected by each of them. It is believed that initially no one has any artifacts. </p></div><div class="input-specification"><p>The first line has 4 natural numbers: <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 100</span>) — the number of Kostya's allies, <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>) — the number of basic artifacts, <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>m</i> ≤ 50</span>) — the number of composite artifacts, <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 500</span>) — the number of his friends' purchases. The following <span class="tex-span"><i>n</i></span> lines contain the names of basic artifacts. After them <span class="tex-span"><i>m</i></span> lines contain the descriptions of composite artifacts in the following format:</p><p><span class="tex-font-style-tt">&lt;Art. Name&gt;: &lt;Art. №1&gt; &lt;Art. №1 Number&gt;, &lt;Art. №2&gt; &lt;Art. №2 Number&gt;, ... &lt;Art. №X&gt; &lt;Art. №Х Number&gt;</span></p><p>All the numbers are natural numbers not exceeding 100 (<span class="tex-span">1 ≤ <i>X</i> ≤ <i>n</i></span>).</p><p>The names of all artifacts are different, they are composed of lowercase Latin letters, and the length of each name is from 1 to 100 characters inclusive. All the words in the format of the description of a composite artifact are separated by exactly one space. It is guaranteed that all components of the new artifact are different and have already been met in the input data as the names of basic artifacts. </p><p>Next, each of the following <span class="tex-span"><i>q</i></span> lines is characterized by the number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, the number of a friend who has bought the artifact (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>k</i></span>), and the name of the purchased basic artifact. Let's assume that the backpacks of the heroes are infinitely large and any artifact bought later can fit in there.</p><p>It is guaranteed that after the <span class="tex-span"><i>i</i></span>-th purchase no more than one opportunity to collect the composite artifact appears. If such an opportunity arose, the hero must take advantage of it.</p></div><div class="output-specification"><p>The output file should consist of <span class="tex-span"><i>k</i></span> blocks. The first line should contain number <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> — the number of different artifacts the <span class="tex-span"><i>i</i></span>-th ally has. Then the block should contain <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> lines with the names of these artifacts and the number of these artifacts. At that the lines should be printed in accordance with the lexicographical order of the names of the artifacts. In each block all the artifacts must be different, and all the numbers except the <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> should be positive.</p></div>

## Input

<p>The first line has 4 natural numbers: <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 100</span>) — the number of Kostya's allies, <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>) — the number of basic artifacts, <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>m</i> ≤ 50</span>) — the number of composite artifacts, <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 500</span>) — the number of his friends' purchases. The following <span class="tex-span"><i>n</i></span> lines contain the names of basic artifacts. After them <span class="tex-span"><i>m</i></span> lines contain the descriptions of composite artifacts in the following format:</p><p><span class="tex-font-style-tt">&lt;Art. Name&gt;: &lt;Art. №1&gt; &lt;Art. №1 Number&gt;, &lt;Art. №2&gt; &lt;Art. №2 Number&gt;, ... &lt;Art. №X&gt; &lt;Art. №Х Number&gt;</span></p><p>All the numbers are natural numbers not exceeding 100 (<span class="tex-span">1 ≤ <i>X</i> ≤ <i>n</i></span>).</p><p>The names of all artifacts are different, they are composed of lowercase Latin letters, and the length of each name is from 1 to 100 characters inclusive. All the words in the format of the description of a composite artifact are separated by exactly one space. It is guaranteed that all components of the new artifact are different and have already been met in the input data as the names of basic artifacts. </p><p>Next, each of the following <span class="tex-span"><i>q</i></span> lines is characterized by the number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, the number of a friend who has bought the artifact (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>k</i></span>), and the name of the purchased basic artifact. Let's assume that the backpacks of the heroes are infinitely large and any artifact bought later can fit in there.</p><p>It is guaranteed that after the <span class="tex-span"><i>i</i></span>-th purchase no more than one opportunity to collect the composite artifact appears. If such an opportunity arose, the hero must take advantage of it.</p>

## Output

<p>The output file should consist of <span class="tex-span"><i>k</i></span> blocks. The first line should contain number <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> — the number of different artifacts the <span class="tex-span"><i>i</i></span>-th ally has. Then the block should contain <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> lines with the names of these artifacts and the number of these artifacts. At that the lines should be printed in accordance with the lexicographical order of the names of the artifacts. In each block all the artifacts must be different, and all the numbers except the <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> should be positive.</p>





```input1
2 3 2 5
desolator
refresher
perseverance
vanguard: desolator 1, refresher 1
maelstorm: perseverance 2
1 desolator
2 perseverance
1 refresher
2 desolator
2 perseverance

```




```output1
1
vanguard 1
2
desolator 1
maelstorm 1

```


