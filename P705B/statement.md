## Description

<div><p>Peter Parker wants to play a game with Dr. Octopus. The game is about cycles. <span class="tex-font-style-it">Cycle</span> is a sequence of vertices, such that first one is connected with the second, second is connected with third and so on, while the last one is connected with the first one again. Cycle may consist of a single isolated vertex.</p><p>Initially there are <span class="tex-span"><i>k</i></span> cycles, <span class="tex-span"><i>i</i></span>-th of them consisting of exactly <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> vertices. Players play alternatively. Peter goes first. On each turn a player must choose a cycle with at least <span class="tex-span">2</span> vertices (for example, <span class="tex-span"><i>x</i></span> vertices) among all available cycles and replace it by two cycles with <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>x</i> - <i>p</i></span> vertices where <span class="tex-span">1 ≤ <i>p</i> &lt; <i>x</i></span> is chosen by the player. The player who cannot make a move loses the game (and his life!).</p><p>Peter wants to test some configurations of initial cycle sets before he actually plays with Dr. Octopus. Initially he has an empty set. In the <span class="tex-span"><i>i</i></span>-th test he adds a cycle with <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> vertices to the set (this is actually a multiset because it can contain two or more identical cycles). After each test, Peter wants to know that if the players begin the game with the current set of cycles, who wins? </p><p>Peter is pretty good at math, but now he asks you to help.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of tests Peter is about to make.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), <span class="tex-span"><i>i</i></span>-th of them stands for the number of vertices in the cycle added before the <span class="tex-span"><i>i</i></span>-th test.</p></div><div class="output-specification"><p>Print the result of all tests in order they are performed. Print <span class="tex-font-style-tt">1</span> if the player who moves first wins or <span class="tex-font-style-tt">2</span> otherwise.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of tests Peter is about to make.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), <span class="tex-span"><i>i</i></span>-th of them stands for the number of vertices in the cycle added before the <span class="tex-span"><i>i</i></span>-th test.</p>

## Output

<p>Print the result of all tests in order they are performed. Print <span class="tex-font-style-tt">1</span> if the player who moves first wins or <span class="tex-font-style-tt">2</span> otherwise.</p>





```input1
3
1 2 3

```




```input2
5
1 1 5 1 1

```




```output1
2
1
1

```




```output2
2
2
2
2
2

```



## Note

<p>In the first sample test:</p><p>In Peter's first test, there's only one cycle with <span class="tex-span">1</span> vertex. First player cannot make a move and loses.</p><p>In his second test, there's one cycle with <span class="tex-span">1</span> vertex and one with <span class="tex-span">2</span>. No one can make a move on the cycle with <span class="tex-span">1</span> vertex. First player can replace the second cycle with two cycles of <span class="tex-span">1</span> vertex and second player can't make any move and loses.</p><p>In his third test, cycles have <span class="tex-span">1</span>, <span class="tex-span">2</span> and <span class="tex-span">3</span> vertices. Like last test, no one can make a move on the first cycle. First player can replace the third cycle with one cycle with size <span class="tex-span">1</span> and one with size <span class="tex-span">2</span>. Now cycles have <span class="tex-span">1</span>, <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">2</span> vertices. Second player's only move is to replace a cycle of size <span class="tex-span">2</span> with <span class="tex-span">2</span> cycles of size <span class="tex-span">1</span>. And cycles are <span class="tex-span">1</span>, <span class="tex-span">1</span>, <span class="tex-span">1</span>, <span class="tex-span">1</span>, <span class="tex-span">2</span>. First player replaces the last cycle with <span class="tex-span">2</span> cycles with size <span class="tex-span">1</span> and wins.</p><p>In the second sample test:</p><p>Having cycles of size <span class="tex-span">1</span> is like not having them (because no one can make a move on them). </p><p>In Peter's third test: There a cycle of size <span class="tex-span">5</span> (others don't matter). First player has two options: replace it with cycles of sizes <span class="tex-span">1</span> and <span class="tex-span">4</span> or <span class="tex-span">2</span> and <span class="tex-span">3</span>.</p><ul> <li> If he replaces it with cycles of sizes <span class="tex-span">1</span> and <span class="tex-span">4</span>: Only second cycle matters. Second player will replace it with <span class="tex-span">2</span> cycles of sizes <span class="tex-span">2</span>. First player's only option to replace one of them with two cycles of size <span class="tex-span">1</span>. Second player does the same thing with the other cycle. First player can't make any move and loses. </li><li> If he replaces it with cycles of sizes <span class="tex-span">2</span> and <span class="tex-span">3</span>: Second player will replace the cycle of size <span class="tex-span">3</span> with two of sizes <span class="tex-span">1</span> and <span class="tex-span">2</span>. Now only cycles with more than one vertex are two cycles of size <span class="tex-span">2</span>. As shown in previous case, with <span class="tex-span">2</span> cycles of size <span class="tex-span">2</span> second player wins. </li></ul><p>So, either way first player loses.</p>
