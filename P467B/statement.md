## Description

<div><p>After you had helped George and Alex to move in the dorm, they went to help their friend Fedor play a new computer game «Call of Soldiers 3».</p><p>The game has <span class="tex-span">(<i>m</i> + 1)</span> players and <span class="tex-span"><i>n</i></span> types of soldiers in total. Players «Call of Soldiers 3» are numbered form <span class="tex-span">1</span> to <span class="tex-span">(<i>m</i> + 1)</span>. Types of soldiers are numbered from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i> - 1</span>. Each player has an army. Army of the <span class="tex-span"><i>i</i></span>-th player can be described by non-negative integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>. Consider binary representation of <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>: if the <span class="tex-span"><i>j</i></span>-th bit of number <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> equal to one, then the army of the <span class="tex-span"><i>i</i></span>-th player has soldiers of the <span class="tex-span"><i>j</i></span>-th type. </p><p>Fedor is the <span class="tex-span">(<i>m</i> + 1)</span>-th player of the game. He assume that two players can become friends if their armies differ in at most <span class="tex-span"><i>k</i></span> types of soldiers (in other words, binary representations of the corresponding numbers differ in at most <span class="tex-span"><i>k</i></span> bits). Help Fedor and count how many players can become his friends.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ <i>n</i> ≤ 20;&nbsp;1 ≤ <i>m</i> ≤ 1000)</span>.</p><p>The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span">(<i>m</i> + 1)</span> lines contains a single integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 2<sup class="upper-index"><i>n</i></sup> - 1)</span>, that describes the <span class="tex-span"><i>i</i></span>-th player's army. We remind you that Fedor is the <span class="tex-span">(<i>m</i> + 1)</span>-th player.</p></div><div class="output-specification"><p>Print a single integer — the number of Fedor's potential friends.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ <i>n</i> ≤ 20;&nbsp;1 ≤ <i>m</i> ≤ 1000)</span>.</p><p>The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span">(<i>m</i> + 1)</span> lines contains a single integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 2<sup class="upper-index"><i>n</i></sup> - 1)</span>, that describes the <span class="tex-span"><i>i</i></span>-th player's army. We remind you that Fedor is the <span class="tex-span">(<i>m</i> + 1)</span>-th player.</p>

## Output

<p>Print a single integer — the number of Fedor's potential friends.</p>





```input1
7 3 1
8
5
111
17

```




```input2
3 3 3
1
2
3
4

```




```output1
0

```




```output2
3

```


