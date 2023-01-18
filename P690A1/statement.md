## Description

<div><p>Tonight is brain dinner night and all zombies will gather together to scarf down some delicious brains. The artful Heidi plans to crash the party, incognito, disguised as one of them. Her objective is to get away with at least one brain, so she can analyze the zombies' mindset back home and gain a strategic advantage.</p><p>They will be <span class="tex-span"><i>N</i></span> guests tonight: <span class="tex-span"><i>N</i> - 1</span> real zombies and a fake one, our Heidi. The living-dead love hierarchies as much as they love brains: each one has a unique rank in the range <span class="tex-span">1</span> to <span class="tex-span"><i>N</i> - 1</span>, and Heidi, who still appears slightly different from the others, is attributed the highest rank, <span class="tex-span"><i>N</i></span>. Tonight there will be a chest with brains on display and every attendee sees how many there are. These will then be split among the attendees according to the following procedure:</p><p>The zombie of the highest rank makes a suggestion on who gets how many brains (every brain is an indivisible entity). A vote follows. If at least half of the attendees accept the offer, the brains are shared in the suggested way and the feast begins. But if majority is not reached, then the highest-ranked zombie is killed, and the next zombie in hierarchy has to make a suggestion. If he is killed too, then the third highest-ranked makes one, etc. (It's enough to have exactly half of the votes – in case of a tie, the vote of the highest-ranked alive zombie counts twice, and he will of course vote in favor of his own suggestion in order to stay alive.)</p><p>You should know that zombies are very greedy and sly, and they know this too – basically all zombie brains are alike. Consequently, a zombie will never accept an offer which is suboptimal for him. That is, if an offer is not <span class="tex-font-style-it">strictly</span> better than a potential later offer, he will vote against it. And make no mistake: while zombies may normally seem rather dull, tonight their intellects are perfect. Each zombie's priorities for tonight are, in descending order: </p><ol> <li> survive the event (they experienced death already once and know it is no fun), </li><li> get as many brains as possible. </li></ol><p>Heidi goes first and must make an offer which at least half of the attendees will accept, and which allocates at least one brain for Heidi herself.</p><p>What is the smallest number of brains that have to be in the chest for this to be possible?</p></div><div class="input-specification"><p>The only line of input contains one integer: <span class="tex-span"><i>N</i></span>, the number of attendees (<span class="tex-span">1 ≤ <i>N</i> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Output one integer: the smallest number of brains in the chest which allows Heidi to take one brain home.</p></div>

## Input

<p>The only line of input contains one integer: <span class="tex-span"><i>N</i></span>, the number of attendees (<span class="tex-span">1 ≤ <i>N</i> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Output one integer: the smallest number of brains in the chest which allows Heidi to take one brain home.</p>





```input1
1

```




```input2
4

```




```output1
1

```




```output2
2

```


