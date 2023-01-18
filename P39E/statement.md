## Description

<div><p>You all know the Dirichlet principle, the point of which is that if <span class="tex-span"><i>n</i></span> boxes have no less than <span class="tex-span"><i>n</i> + 1</span> items, that leads to the existence of a box in which there are at least two items.</p><p>Having heard of that principle, but having not mastered the technique of logical thinking, 8 year olds Stas and Masha invented a game. There are <span class="tex-span"><i>a</i></span> different boxes and <span class="tex-span"><i>b</i></span> different items, and each turn a player can either add a new box or a new item. The player, after whose turn the number of ways of putting <span class="tex-span"><i>b</i></span> items into <span class="tex-span"><i>a</i></span> boxes becomes no less then a certain given number <span class="tex-span"><i>n</i></span>, loses. All the boxes and items are considered to be different. Boxes may remain empty.</p><p>Who loses if both players play optimally and Stas's turn is first?</p></div><div class="input-specification"><p>The only input line has three integers <span class="tex-span"><i>a</i>, <i>b</i>, <i>n</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ 10000</span>, <span class="tex-span">1 ≤ <i>b</i> ≤ 30</span>, <span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>) — the initial number of the boxes, the number of the items and the number which constrains the number of ways, respectively. Guaranteed that the initial number of ways is strictly less than <span class="tex-span"><i>n</i></span>.</p></div><div class="output-specification"><p>Output "Stas" if Masha wins. Output "Masha" if Stas wins. In case of a draw, output "Missing".</p></div>

## Input

<p>The only input line has three integers <span class="tex-span"><i>a</i>, <i>b</i>, <i>n</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ 10000</span>, <span class="tex-span">1 ≤ <i>b</i> ≤ 30</span>, <span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>) — the initial number of the boxes, the number of the items and the number which constrains the number of ways, respectively. Guaranteed that the initial number of ways is strictly less than <span class="tex-span"><i>n</i></span>.</p>

## Output

<p>Output "Stas" if Masha wins. Output "Masha" if Stas wins. In case of a draw, output "Missing".</p>





```input1
2 2 10

```




```input2
5 5 16808

```




```input3
3 1 4

```




```input4
1 4 10

```




```output1
Masha

```




```output2
Masha

```




```output3
Stas

```




```output4
Missing

```



## Note

<p>In the second example the initial number of ways is equal to <span class="tex-span">3125</span>. </p><ul> <li> If Stas increases the number of boxes, he will lose, as Masha may increase the number of boxes once more during her turn. After that any Stas's move will lead to defeat. </li><li> But if Stas increases the number of items, then any Masha's move will be losing. </li></ul>
