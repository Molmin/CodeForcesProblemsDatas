## Description

<div><p>Manao is taking part in a quiz. The quiz consists of <span class="tex-span"><i>n</i></span> consecutive questions. A correct answer gives one point to the player. The game also has a counter of consecutive correct answers. When the player answers a question correctly, the number on this counter increases by 1. If the player answers a question incorrectly, the counter is reset, that is, the number on it reduces to 0. If after an answer the counter reaches the number <span class="tex-span"><i>k</i></span>, then it is reset, and the player's score is doubled. Note that in this case, first 1 point is added to the player's score, and then the total score is doubled. At the beginning of the game, both the player's score and the counter of consecutive correct answers are set to zero.</p><p>Manao remembers that he has answered exactly <span class="tex-span"><i>m</i></span> questions correctly. But he does not remember the order in which the questions came. He's trying to figure out what his minimum score may be. Help him and compute the remainder of the corresponding number after division by <span class="tex-span">1000000009</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 9)</span>.</p></div><div class="input-specification"><p>The single line contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup>;&nbsp;0 ≤ <i>m</i> ≤ <i>n</i></span>).</p></div><div class="output-specification"><p>Print a single integer — the remainder from division of Manao's minimum possible score in the quiz by <span class="tex-span">1000000009</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 9)</span>.</p></div>

## Input

<p>The single line contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup>;&nbsp;0 ≤ <i>m</i> ≤ <i>n</i></span>).</p>

## Output

<p>Print a single integer — the remainder from division of Manao's minimum possible score in the quiz by <span class="tex-span">1000000009</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 9)</span>.</p>





```input1
5 3 2

```




```input2
5 4 2

```




```output1
3

```




```output2
6

```



## Note

<p>Sample 1. Manao answered 3 questions out of 5, and his score would double for each two consecutive correct answers. If Manao had answered the first, third and fifth questions, he would have scored as much as 3 points.</p><p>Sample 2. Now Manao answered 4 questions. The minimum possible score is obtained when the only wrong answer is to the question 4.</p><p>Also note that you are asked to minimize the score and not the remainder of the score modulo <span class="tex-span">1000000009</span>. For example, if Manao could obtain either <span class="tex-span">2000000000</span> or <span class="tex-span">2000000020</span> points, the answer is <span class="tex-span">2000000000&nbsp;<i>mod</i>&nbsp;1000000009</span>, even though <span class="tex-span">2000000020&nbsp;<i>mod</i>&nbsp;1000000009</span> is a smaller number.</p>
