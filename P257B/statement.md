## Description

<div><p>Petya and Vasya decided to play a little. They found <span class="tex-span"><i>n</i></span> red cubes and <span class="tex-span"><i>m</i></span> blue cubes. The game goes like that: the players take turns to choose a cube of some color (red or blue) and put it in a line from left to right (overall the line will have <span class="tex-span"><i>n</i> + <i>m</i></span> cubes). Petya moves first. Petya's task is to get as many pairs of neighbouring cubes of the same color as possible. Vasya's task is to get as many pairs of neighbouring cubes of different colors as possible. </p><p>The number of Petya's points in the game is the number of pairs of neighboring cubes of the same color in the line, the number of Vasya's points in the game is the number of neighbouring cubes of the different color in the line. Your task is to calculate the score at the end of the game (Petya's and Vasya's points, correspondingly), if both boys are playing optimally well. To "play optimally well" first of all means to maximize the number of one's points, and second — to minimize the number of the opponent's points.</p></div><div class="input-specification"><p>The only line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of red and blue cubes, correspondingly.</p></div><div class="output-specification"><p>On a single line print two space-separated integers — the number of Petya's and Vasya's points correspondingly provided that both players play optimally well.</p></div>

## Input

<p>The only line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of red and blue cubes, correspondingly.</p>

## Output

<p>On a single line print two space-separated integers — the number of Petya's and Vasya's points correspondingly provided that both players play optimally well.</p>





```input1
3 1

```




```input2
2 4

```




```output1
2 1

```




```output2
3 2

```



## Note

<p>In the first test sample the optimal strategy for Petya is to put the blue cube in the line. After that there will be only red cubes left, so by the end of the game the line of cubes from left to right will look as <span class="tex-font-style-tt">[blue, red, red, red]</span>. So, Petya gets 2 points and Vasya gets 1 point. </p><p>If Petya would choose the red cube during his first move, then, provided that both boys play optimally well, Petya would get 1 point and Vasya would get 2 points.</p>
