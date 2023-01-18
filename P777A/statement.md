## Description

<div><p>Bomboslav likes to look out of the window in his room and watch lads outside playing famous shell game. The game is played by two persons: operator and player. Operator takes three similar opaque shells and places a ball beneath one of them. Then he shuffles the shells by swapping some pairs and the player has to guess the current position of the ball.</p><p>Bomboslav noticed that guys are not very inventive, so the operator always swaps the left shell with the middle one during odd moves (first, third, fifth, etc.) and always swaps the middle shell with the right one during even moves (second, fourth, etc.).</p><p>Let's number shells from <span class="tex-span">0</span> to <span class="tex-span">2</span> from left to right. Thus the left shell is assigned number <span class="tex-span">0</span>, the middle shell is <span class="tex-span">1</span> and the right shell is <span class="tex-span">2</span>. Bomboslav has missed the moment when the ball was placed beneath the shell, but he knows that exactly <span class="tex-span"><i>n</i></span> movements were made by the operator and the ball was under shell <span class="tex-span"><i>x</i></span> at the end. Now he wonders, what was the initial position of the ball?</p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">9</sup></span>)&nbsp;— the number of movements made by the operator.</p><p>The second line contains a single integer <span class="tex-span"><i>x</i></span> (<span class="tex-span">0 ≤ <i>x</i> ≤ 2</span>)&nbsp;— the index of the shell where the ball was found after <span class="tex-span"><i>n</i></span> movements.</p></div><div class="output-specification"><p>Print one integer from <span class="tex-span">0</span> to <span class="tex-span">2</span>&nbsp;— the index of the shell where the ball was initially placed.</p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">9</sup></span>)&nbsp;— the number of movements made by the operator.</p><p>The second line contains a single integer <span class="tex-span"><i>x</i></span> (<span class="tex-span">0 ≤ <i>x</i> ≤ 2</span>)&nbsp;— the index of the shell where the ball was found after <span class="tex-span"><i>n</i></span> movements.</p>

## Output

<p>Print one integer from <span class="tex-span">0</span> to <span class="tex-span">2</span>&nbsp;— the index of the shell where the ball was initially placed.</p>





```input1
4
2

```




```input2
1
1

```




```output1
1

```




```output2
0

```



## Note

<p>In the first sample, the ball was initially placed beneath the middle shell and the operator completed four movements.</p><ol> <li> During the first move operator swapped the left shell and the middle shell. The ball is now under the left shell. </li><li> During the second move operator swapped the middle shell and the right one. The ball is still under the left shell. </li><li> During the third move operator swapped the left shell and the middle shell again. The ball is again in the middle. </li><li> Finally, the operators swapped the middle shell and the right shell. The ball is now beneath the right shell. </li></ol>
