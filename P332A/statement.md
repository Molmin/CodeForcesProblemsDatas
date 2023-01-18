## Description

<div><p>Everybody knows that the Berland citizens are keen on health, especially students. Berland students are so tough that all they drink is orange juice!</p><p>Yesterday one student, Vasya and his mates made some barbecue and they drank this healthy drink only. After they ran out of the first barrel of juice, they decided to play a simple game. All <span class="tex-span"><i>n</i></span> people who came to the barbecue sat in a circle (thus each person received a unique index <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> from 0 to <span class="tex-span"><i>n</i> - 1</span>). The person number 0 started the game (this time it was Vasya). All turns in the game were numbered by integers starting from 1. If the <span class="tex-span"><i>j</i></span>-th turn was made by the person with index <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, then this person acted like that:</p><ol> <li> he pointed at the person with index <span class="tex-span">(<i>b</i><sub class="lower-index"><i>i</i></sub> + 1)&nbsp;<i>mod</i>&nbsp;<i>n</i></span> either with an elbow or with a nod (<span class="tex-span"><i>x</i>&nbsp;<i>mod</i>&nbsp;<i>y</i></span> is the remainder after dividing <span class="tex-span"><i>x</i></span> by <span class="tex-span"><i>y</i></span>); </li><li> if <span class="tex-span"><i>j</i> ≥ 4</span> and the players who had turns number <span class="tex-span"><i>j</i> - 1</span>, <span class="tex-span"><i>j</i> - 2</span>, <span class="tex-span"><i>j</i> - 3</span>, made during their turns the same moves as player <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> on the current turn, then he had drunk a glass of juice; </li><li> the turn went to person number <span class="tex-span">(<i>b</i><sub class="lower-index"><i>i</i></sub> + 1)&nbsp;<i>mod</i>&nbsp;<i>n</i></span>. </li></ol><p>The person who was pointed on the last turn did not make any actions.</p><p>The problem was, Vasya's drunk too much juice and can't remember the goal of the game. However, Vasya's got the recorded sequence of all the participants' actions (including himself). Now Vasya wants to find out the maximum amount of juice he could drink if he played optimally well (the other players' actions do not change). Help him.</p><p>You can assume that in any scenario, there is enough juice for everybody.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">4 ≤ <i>n</i> ≤ 2000</span>) — the number of participants in the game. The second line describes the actual game: the <span class="tex-span"><i>i</i></span>-th character of this line equals '<span class="tex-font-style-tt">a</span>', if the participant who moved <span class="tex-span"><i>i</i></span>-th pointed at the next person with his elbow, and '<span class="tex-font-style-tt">b</span>', if the participant pointed with a nod. The game continued for at least 1 and at most <span class="tex-span">2000</span> turns. </p></div><div class="output-specification"><p>Print a single integer — the number of glasses of juice Vasya could have drunk if he had played optimally well.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">4 ≤ <i>n</i> ≤ 2000</span>) — the number of participants in the game. The second line describes the actual game: the <span class="tex-span"><i>i</i></span>-th character of this line equals '<span class="tex-font-style-tt">a</span>', if the participant who moved <span class="tex-span"><i>i</i></span>-th pointed at the next person with his elbow, and '<span class="tex-font-style-tt">b</span>', if the participant pointed with a nod. The game continued for at least 1 and at most <span class="tex-span">2000</span> turns. </p>

## Output

<p>Print a single integer — the number of glasses of juice Vasya could have drunk if he had played optimally well.</p>





```input1
4
abbba

```




```input2
4
abbab

```




```output1
1

```




```output2
0

```



## Note

<p>In both samples Vasya has got two turns — 1 and 5. In the first sample, Vasya could have drunk a glass of juice during the fifth turn if he had pointed at the next person with a nod. In this case, the sequence of moves would look like "abbbb". In the second sample Vasya wouldn't drink a single glass of juice as the moves performed during turns 3 and 4 are different.</p>
