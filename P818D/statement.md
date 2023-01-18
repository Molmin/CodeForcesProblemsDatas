## Description

<div><p>Alice and Bob got very bored during a long car trip so they decided to play a game. From the window they can see cars of different colors running past them. Cars are going one after another.</p><p>The game rules are like this. Firstly Alice chooses some color <span class="tex-span"><i>A</i></span>, then Bob chooses some color <span class="tex-span"><i>B</i></span> (<span class="tex-span"><i>A</i> ≠ <i>B</i></span>). After each car they update the number of cars of their chosen color that have run past them. Let's define this numbers after <span class="tex-span"><i>i</i></span>-th car <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>A</i></sub>(<i>i</i>)</span> and <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>B</i></sub>(<i>i</i>)</span>.</p><ul> <li> If <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>A</i></sub>(<i>i</i>) &gt; <i>cnt</i><sub class="lower-index"><i>B</i></sub>(<i>i</i>)</span> for every <span class="tex-span"><i>i</i></span> then the winner is Alice. </li><li> If <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>B</i></sub>(<i>i</i>) ≥ <i>cnt</i><sub class="lower-index"><i>A</i></sub>(<i>i</i>)</span> for every <span class="tex-span"><i>i</i></span> then the winner is Bob. </li><li> Otherwise it's a draw. </li></ul><p>Bob knows all the colors of cars that they will encounter and order of their appearance. Alice have already chosen her color <span class="tex-span"><i>A</i></span> and Bob now wants to choose such color <span class="tex-span"><i>B</i></span> that he will win the game (draw is not a win). Help him find this color.</p><p>If there are multiple solutions, print any of them. If there is no such color then print <span class="tex-font-style-tt">-1</span>.</p></div><div class="input-specification"><p>The first line contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>A</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>A</i> ≤ 10<sup class="upper-index">6</sup></span>) – number of cars and the color chosen by Alice.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — colors of the cars that Alice and Bob will encounter in the order of their appearance.</p></div><div class="output-specification"><p>Output such color <span class="tex-span"><i>B</i></span> (<span class="tex-span">1 ≤ <i>B</i> ≤ 10<sup class="upper-index">6</sup></span>) that if Bob chooses it then he will win the game. If there are multiple solutions, print any of them. If there is no such color then print <span class="tex-font-style-tt">-1</span>.</p><p>It is guaranteed that if there exists any solution then there exists solution with (<span class="tex-span">1 ≤ <i>B</i> ≤ 10<sup class="upper-index">6</sup></span>).</p></div>

## Input

<p>The first line contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>A</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>A</i> ≤ 10<sup class="upper-index">6</sup></span>) – number of cars and the color chosen by Alice.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — colors of the cars that Alice and Bob will encounter in the order of their appearance.</p>

## Output

<p>Output such color <span class="tex-span"><i>B</i></span> (<span class="tex-span">1 ≤ <i>B</i> ≤ 10<sup class="upper-index">6</sup></span>) that if Bob chooses it then he will win the game. If there are multiple solutions, print any of them. If there is no such color then print <span class="tex-font-style-tt">-1</span>.</p><p>It is guaranteed that if there exists any solution then there exists solution with (<span class="tex-span">1 ≤ <i>B</i> ≤ 10<sup class="upper-index">6</sup></span>).</p>





```input1
4 1
2 1 4 2

```




```input2
5 2
2 2 4 5 3

```




```input3
3 10
1 2 3

```




```output1
2

```




```output2
-1

```




```output3
4

```



## Note

<p>Let's consider availability of colors in the first example: </p><ul> <li> <span class="tex-span"><i>cnt</i><sub class="lower-index">2</sub>(<i>i</i>) ≥ <i>cnt</i><sub class="lower-index">1</sub>(<i>i</i>)</span> for every <span class="tex-span"><i>i</i></span>, and color <span class="tex-span">2</span> can be the answer. </li><li> <span class="tex-span"><i>cnt</i><sub class="lower-index">4</sub>(2) &lt; <i>cnt</i><sub class="lower-index">1</sub>(2)</span>, so color <span class="tex-span">4</span> isn't the winning one for Bob. </li><li> All the other colors also have <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>j</i></sub>(2) &lt; <i>cnt</i><sub class="lower-index">1</sub>(2)</span>, thus they are not available. </li></ul><p>In the third example every color is acceptable except for <span class="tex-span">10</span>.</p>
