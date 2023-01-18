## Description

<div><p>Famous Brazil city Rio de Janeiro holds a tennis tournament and Ostap Bender doesn't want to miss this event. There will be <span class="tex-span"><i>n</i></span> players participating, and the tournament will follow knockout rules from the very first game. That means, that if someone loses a game he leaves the tournament immediately.</p><p>Organizers are still arranging tournament grid (i.e. the order games will happen and who is going to play with whom) but they have already fixed one rule: two players can play against each other only if the number of games one of them has already played <span class="tex-font-style-bf">differs by no more than one</span> from the number of games the other one has already played. Of course, both players had to win all their games in order to continue participating in the tournament.</p><p>Tournament hasn't started yet so the audience is a bit bored. Ostap decided to find out what is the maximum number of games the winner of the tournament can take part in (assuming the rule above is used). However, it is unlikely he can deal with this problem without your help.</p></div><div class="input-specification"><p>The only line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup></span>)&nbsp;— the number of players to participate in the tournament.</p></div><div class="output-specification"><p>Print the maximum number of games in which the winner of the tournament can take part.</p></div>

## Input

<p>The only line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup></span>)&nbsp;— the number of players to participate in the tournament.</p>

## Output

<p>Print the maximum number of games in which the winner of the tournament can take part.</p>





```input1
2

```




```input2
3

```




```input3
4

```




```input4
10

```




```output1
1

```




```output2
2

```




```output3
2

```




```output4
4

```



## Note

<p>In all samples we consider that player number <span class="tex-span">1</span> is the winner.</p><p>In the first sample, there would be only one game so the answer is <span class="tex-span">1</span>.</p><p>In the second sample, player <span class="tex-span">1</span> can consequently beat players <span class="tex-span">2</span> and <span class="tex-span">3</span>. </p><p>In the third sample, player <span class="tex-span">1</span> can't play with each other player as after he plays with players <span class="tex-span">2</span> and <span class="tex-span">3</span> he can't play against player <span class="tex-span">4</span>, as he has <span class="tex-span">0</span> games played, while player <span class="tex-span">1</span> already played <span class="tex-span">2</span>. Thus, the answer is <span class="tex-span">2</span> and to achieve we make pairs <span class="tex-span">(1, 2)</span> and <span class="tex-span">(3, 4)</span> and then clash the winners.</p>
