## Description

<div><p>Heidi got one brain, thumbs up! But the evening isn't over yet and one more challenge awaits our dauntless agent: after dinner, at precisely midnight, the <span class="tex-span"><i>N</i></span> attendees love to play a very risky game...</p><p>Every zombie gets a number <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>n</i><sub class="lower-index"><i>i</i></sub> ≤ <i>N</i></span>) written on his forehead. Although no zombie can see his own number, he can see the numbers written on the foreheads of all <span class="tex-span"><i>N</i> - 1</span> fellows. Note that not all numbers have to be unique (they can even all be the same). From this point on, no more communication between zombies is allowed. Observation is the only key to success. When the cuckoo clock strikes midnight, all attendees have to simultaneously guess the number on their own forehead. If at least one of them guesses his number correctly, all zombies survive and go home happily. On the other hand, if not a single attendee manages to guess his number correctly, all of them are doomed to die!</p><p>Zombies aren't very bright creatures though, and Heidi has to act fast if she does not want to jeopardize her life. She has one single option: by performing some quick surgery on the brain she managed to get from the chest, she has the ability to remotely reprogram the decision-making strategy of all attendees for their upcoming midnight game! Can you suggest a sound strategy to Heidi which, given the rules of the game, ensures that at least one attendee will guess his own number correctly, for any possible sequence of numbers on the foreheads?</p><p>Given a zombie's rank <span class="tex-span"><i>R</i></span> and the <span class="tex-span"><i>N</i> - 1</span> numbers <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> on the other attendees' foreheads, your program will have to return the number that the zombie of rank <span class="tex-span"><i>R</i></span> shall guess. Those answers define your strategy, and we will check if it is flawless or not.</p></div><div class="input-specification"><p>The first line of input contains a single integer <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ <i>T</i> ≤ 50000</span>): the number of scenarios for which you have to make a guess.</p><p>The <span class="tex-span"><i>T</i></span> scenarios follow, described on two lines each: </p><ul> <li> The first line holds two integers, <span class="tex-span"><i>N</i></span> (<span class="tex-span">2 ≤ <i>N</i> ≤ 6</span>), the number of attendees, and <span class="tex-span"><i>R</i></span> (<span class="tex-span">1 ≤ <i>R</i> ≤ <i>N</i></span>), the rank of the zombie who has to make the guess. </li><li> The second line lists <span class="tex-span"><i>N</i> - 1</span> integers: the numbers on the foreheads of all other attendees, listed in increasing order of the attendees' rank. (Every zombie knows the rank of every other zombie.) </li></ul></div><div class="output-specification"><p>For every scenario, output a single integer: the number that the zombie of rank <span class="tex-span"><i>R</i></span> shall guess, based on the numbers <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> on his <span class="tex-span"><i>N</i> - 1</span> fellows' foreheads.</p></div>

## Input

<p>The first line of input contains a single integer <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ <i>T</i> ≤ 50000</span>): the number of scenarios for which you have to make a guess.</p><p>The <span class="tex-span"><i>T</i></span> scenarios follow, described on two lines each: </p><ul> <li> The first line holds two integers, <span class="tex-span"><i>N</i></span> (<span class="tex-span">2 ≤ <i>N</i> ≤ 6</span>), the number of attendees, and <span class="tex-span"><i>R</i></span> (<span class="tex-span">1 ≤ <i>R</i> ≤ <i>N</i></span>), the rank of the zombie who has to make the guess. </li><li> The second line lists <span class="tex-span"><i>N</i> - 1</span> integers: the numbers on the foreheads of all other attendees, listed in increasing order of the attendees' rank. (Every zombie knows the rank of every other zombie.) </li></ul>

## Output

<p>For every scenario, output a single integer: the number that the zombie of rank <span class="tex-span"><i>R</i></span> shall guess, based on the numbers <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> on his <span class="tex-span"><i>N</i> - 1</span> fellows' foreheads.</p>





```input1
4
2 1
1
2 2
1
2 1
2
2 2
2

```




```input2
2
5 2
2 2 2 2
6 4
3 2 6 1 2

```




```output1
1
2
2
1

```




```output2
5
2

```



## Note

<p>For instance, if there were <span class="tex-span"><i>N</i> = 2</span> two attendees, a successful strategy could be: </p><ul> <li> The zombie of rank 1 always guesses the number he sees on the forehead of the zombie of rank 2. </li><li> The zombie of rank 2 always guesses the opposite of the number he sees on the forehead of the zombie of rank 1. </li></ul>
