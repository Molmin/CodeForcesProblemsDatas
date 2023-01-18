## Description

<div><p>One day, little Vasya found himself in a maze consisting of <span class="tex-span">(<i>n</i> + 1)</span> rooms, numbered from <span class="tex-span">1</span> to <span class="tex-span">(<i>n</i> + 1)</span>. Initially, Vasya is at the first room and to get out of the maze, he needs to get to the <span class="tex-span">(<i>n</i> + 1)</span>-th one.</p><p>The maze is organized as follows. Each room of the maze has two one-way portals. Let's consider room number <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i>)</span>, someone can use the first portal to move from it to room number <span class="tex-span">(<i>i</i> + 1)</span>, also someone can use the second portal to move from it to room number <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, where <span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>i</i></span>.</p><p>In order not to get lost, Vasya decided to act as follows. </p><ul> <li> Each time Vasya enters some room, he paints a cross on its ceiling. Initially, Vasya paints a cross at the ceiling of room <span class="tex-span">1</span>. </li><li> Let's assume that Vasya is in room <span class="tex-span"><i>i</i></span> and has already painted a cross on its ceiling. Then, if the ceiling now contains an odd number of crosses, Vasya uses the second portal (it leads to room <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>), otherwise Vasya uses the first portal. </li></ul><p>Help Vasya determine the number of times he needs to use portals to get to room <span class="tex-span">(<i>n</i> + 1)</span> in the end.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup></span>)&nbsp;— the number of rooms. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>i</i></span>). Each <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> denotes the number of the room, that someone can reach, if he will use the second portal in the <span class="tex-span"><i>i</i></span>-th room.</p></div><div class="output-specification"><p>Print a single number — the number of portal moves the boy needs to go out of the maze. As the number can be rather large, print it modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup></span>)&nbsp;— the number of rooms. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>i</i></span>). Each <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> denotes the number of the room, that someone can reach, if he will use the second portal in the <span class="tex-span"><i>i</i></span>-th room.</p>

## Output

<p>Print a single number — the number of portal moves the boy needs to go out of the maze. As the number can be rather large, print it modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
2
1 2

```




```input2
4
1 1 2 3

```




```input3
5
1 1 1 1 1

```




```output1
4

```




```output2
20

```




```output3
62

```


