## Description

<div><p>Owl Sonya decided to become a partymaker. To train for this role she gather all her owl friends in the country house. There are <span class="tex-span"><i>m</i></span> chairs located in a circle and consequently numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>. Thus, chairs <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>i</i> + 1</span> are neighbouring for all <span class="tex-span"><i>i</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i> - 1</span>. Chairs <span class="tex-span">1</span> and <span class="tex-span"><i>m</i></span> are also neighbouring. Some chairs are occupied by her friends. There are <span class="tex-span"><i>n</i></span> friends in total. No two friends occupy the same chair. Rules are the following:</p><ol> <li> Each participant removes from the game the chair he is currently sitting on. </li><li> Each of the participants choose a direction that she will follow: clockwise (indices increase, from <span class="tex-span"><i>m</i></span> goes to <span class="tex-span">1</span>) and counter-clockwise (indices decrease, from <span class="tex-span">1</span> goes to <span class="tex-span"><i>m</i></span>). This direction may coincide or be different for any pair of owls. </li><li> Each turn all guests move one step in the chosen directions. If some guest move to the position with a chair there, he removes this chair from the game. </li><li> Game ends if there are no more chairs left in the game. </li></ol><p>Owls are very busy and want to get rid of the game as soon as possible. They cooperate to pick the direction. Your goal is to find the minimum number o moves required to finish the game.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the length of the circle.</p><p>The second line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of friends.</p><p>Last line contains an increasing sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>)&nbsp;— initial positions of all owls.</p></div><div class="output-specification"><p>Print the minimum number of move required to finish the game. Note, that <span class="tex-span">0</span> also may be an answer.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the length of the circle.</p><p>The second line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of friends.</p><p>Last line contains an increasing sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>)&nbsp;— initial positions of all owls.</p>

## Output

<p>Print the minimum number of move required to finish the game. Note, that <span class="tex-span">0</span> also may be an answer.</p>





```input1
6
3
1 3 5

```




```input2
6
2
1 6

```




```input3
406
6
1 2 3 204 205 206

```




```output1
1

```




```output2
2

```




```output3
100

```



## Note

<p>In the first sample, it's possible if all owls will move clockwise, i.e. in the direction of increasing indices.</p><p>In the sample, first owl has to move clockwise, while the second&nbsp;— counterclockwise.</p><p>In the third sample, the first and the fourth owls should move counterclockwise, while the third and the sixth&nbsp;— clockwise. The second and the firth may move in any direction.</p>
