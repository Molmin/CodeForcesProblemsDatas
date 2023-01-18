## Description

<div><p>Nikita and Sasha play a computer game where you have to breed some magical creatures. Initially, they have <span class="tex-span"><i>k</i></span> creatures numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i></span>. Creatures have <span class="tex-span"><i>n</i></span> different characteristics.</p><p>Sasha has a spell that allows to create a new creature from two given creatures. Each of its characteristics will be equal to the maximum of the corresponding characteristics of used creatures. Nikita has a similar spell, but in his spell, each characteristic of the new creature is equal to the minimum of the corresponding characteristics of used creatures. A new creature gets the smallest unused number.</p><p>They use their spells and are interested in some characteristics of their new creatures. Help them find out these characteristics.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 12</span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) — number of characteristics, creatures and queries.</p><p>Next <span class="tex-span"><i>k</i></span> lines describe original creatures. The line <span class="tex-span"><i>i</i></span> contains <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>1</sub>, <i>a</i><sub class="lower-index"><i>i</i>2</sub>, ..., <i>a</i><sub class="lower-index"><i>in</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— characteristics of the <span class="tex-span"><i>i</i></span>-th creature.</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contains a query. The <span class="tex-span"><i>i</i></span>-th of these lines contains numbers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 3</span>). They denote a query: </p><ul> <li> <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 1</span> means that Sasha used his spell to the creatures <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>. </li><li> <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 2</span> means that Nikita used his spell to the creatures <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>. </li><li> <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 3</span> means that they want to know the <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>-th characteristic of the <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>-th creature. In this case <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>. </li></ul><p>It's guaranteed that all creatures' numbers are valid, that means that they are created before any of the queries involving them.</p></div><div class="output-specification"><p>For each query with <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 3</span> output the corresponding characteristic.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 12</span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) — number of characteristics, creatures and queries.</p><p>Next <span class="tex-span"><i>k</i></span> lines describe original creatures. The line <span class="tex-span"><i>i</i></span> contains <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>1</sub>, <i>a</i><sub class="lower-index"><i>i</i>2</sub>, ..., <i>a</i><sub class="lower-index"><i>in</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— characteristics of the <span class="tex-span"><i>i</i></span>-th creature.</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contains a query. The <span class="tex-span"><i>i</i></span>-th of these lines contains numbers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 3</span>). They denote a query: </p><ul> <li> <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 1</span> means that Sasha used his spell to the creatures <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>. </li><li> <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 2</span> means that Nikita used his spell to the creatures <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>. </li><li> <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 3</span> means that they want to know the <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>-th characteristic of the <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>-th creature. In this case <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>. </li></ul><p>It's guaranteed that all creatures' numbers are valid, that means that they are created before any of the queries involving them.</p>

## Output

<p>For each query with <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 3</span> output the corresponding characteristic.</p>





```input1
2 2 4
1 2
2 1
1 1 2
2 1 2
3 3 1
3 4 2

```




```input2
5 3 8
1 2 3 4 5
5 1 2 3 4
4 5 1 2 3
1 1 2
1 2 3
2 4 5
3 6 1
3 6 2
3 6 3
3 6 4
3 6 5

```




```output1
2
1

```




```output2
5
2
2
3
4

```



## Note

<p>In the first sample, Sasha makes a creature with number <span class="tex-span">3</span> and characteristics <span class="tex-span">(2, 2)</span>. Nikita makes a creature with number <span class="tex-span">4</span> and characteristics <span class="tex-span">(1, 1)</span>. After that they find out the first characteristic for the creature <span class="tex-span">3</span> and the second characteristic for the creature <span class="tex-span">4</span>.</p>
