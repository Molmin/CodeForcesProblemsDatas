## Description

<div><p>Your friend recently gave you some slimes for your birthday. You have a very large amount of slimes with value <span class="tex-span">1</span> and <span class="tex-span">2</span>, and you decide to invent a game using these slimes.</p><p>You initialize a row with <span class="tex-span"><i>n</i></span> empty spaces. You also choose a number <span class="tex-span"><i>p</i></span> to be used in the game. Then, you will perform the following steps while the last space is empty. </p><ol> <li> With probability <img align="middle" class="tex-formula" src="file://8B3rbgB1.png" style="max-width: 100.0%;max-height: 100.0%;">, you will choose a slime with value <span class="tex-span">1</span>, and with probability <img align="middle" class="tex-formula" src="file://DXgUMeEJ.png" style="max-width: 100.0%;max-height: 100.0%;">, you will choose a slime with value <span class="tex-span">2</span>. You place the chosen slime on the last space of the board. </li><li> You will push the slime to the left as far as possible. If it encounters another slime, and they have the same value <span class="tex-span"><i>v</i></span>, you will merge the slimes together to create a single slime with value <span class="tex-span"><i>v</i> + 1</span>. This continues on until the slime reaches the end of the board, or encounters a slime with a different value than itself. </li></ol><p>You have played the game a few times, but have gotten bored of it. You are now wondering, what is the expected sum of all values of the slimes on the board after you finish the game.</p></div><div class="input-specification"><p>The first line of the input will contain two integers <span class="tex-span"><i>n</i>, <i>p</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>p</i> &lt; 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print the expected sum of all slimes on the board after the game finishes. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p><p>Namely, let's assume that your answer is <span class="tex-span"><i>a</i></span> and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://GDAaxC5G.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line of the input will contain two integers <span class="tex-span"><i>n</i>, <i>p</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>p</i> &lt; 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print the expected sum of all slimes on the board after the game finishes. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p><p>Namely, let's assume that your answer is <span class="tex-span"><i>a</i></span> and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://GDAaxC5G.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
2 500000000

```




```input2
10 1

```




```input3
100 123456789

```




```output1
3.562500000000000

```




```output2
64.999983360007620

```




```output3
269.825611298854770

```



## Note

<p>In the first sample, we have a board with two squares, and there is a <span class="tex-span">0.5</span> probability of a <span class="tex-font-style-tt">1</span> appearing and a <span class="tex-span">0.5</span> probability of a <span class="tex-font-style-tt">2</span> appearing.</p><p>Our final board states can be <span class="tex-font-style-tt">1 2</span> with probability <span class="tex-span">0.25</span>, <span class="tex-font-style-tt">2 1</span> with probability <span class="tex-span">0.375</span>, <span class="tex-font-style-tt">3 2</span> with probability <span class="tex-span">0.1875</span>, <span class="tex-font-style-tt">3 1</span> with probability <span class="tex-span">0.1875</span>. The expected value is thus <span class="tex-span">(1 + 2)·0.25 + (2 + 1)·0.375 + (3 + 2)·0.1875 + (3 + 1)·0.1875 = 3.5625</span>.</p>
