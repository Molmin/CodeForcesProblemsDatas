## Description

<div><p>A MIPT student named Misha has a birthday today, and he decided to celebrate it in his country house in suburban Moscow. <span class="tex-span"><i>n</i></span> friends came by, and after a typical party they decided to play blind man's buff.</p><p>The birthday boy gets blindfolded and the other players scatter around the house. The game is played in several rounds. In each round, Misha catches exactly one of his friends and has to guess who it is. The probability of catching the <span class="tex-span"><i>i</i></span>-th friend does not change between rounds and is equal to <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> percent (as we know, it is directly proportional to the amount of alcohol consumed by the <span class="tex-span"><i>i</i></span>-th friend) and <span class="tex-span"><i>p</i><sub class="lower-index">1</sub> + <i>p</i><sub class="lower-index">2</sub> + ... + <i>p</i><sub class="lower-index"><i>n</i></sub> = 100</span> holds. Misha has no information about who he caught. After Misha makes an attempt to guess the caught person, the round ends. Even then, Misha isn't told whether he guessed correctly, and a new round begins.</p><p>The game ends when Misha guesses every friend at least once, that is, there exists such set of rounds <span class="tex-span"><i>k</i><sub class="lower-index">1</sub>, <i>k</i><sub class="lower-index">2</sub>, ..., <i>k</i><sub class="lower-index"><i>n</i></sub></span>, that during round number <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> Misha caught the <span class="tex-span"><i>i</i></span>-th friend and guessed him. Misha wants to minimize the expectation of the number of rounds of the game. Despite the fact that at any point in the game Misha has no information about who he has already guessed, his friends are honest, and if they see that the condition for the end of the game is fulfilled, the game ends immediately. Find the expectation of the number of rounds in the game if Misha plays optimally.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of Misha's friends.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<img align="middle" class="tex-formula" src="file://ZqNcHTfv.png" style="max-width: 100.0%;max-height: 100.0%;">), giving the probability to catch the <span class="tex-span"><i>i</i></span>-th friend in one particular round in percent.</p></div><div class="output-specification"><p>Print a single real value&nbsp;— the expectation of the number of rounds provided that Misha plays optimally. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://fZ2J5Z0w.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of Misha's friends.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<img align="middle" class="tex-formula" src="file://ZqNcHTfv.png" style="max-width: 100.0%;max-height: 100.0%;">), giving the probability to catch the <span class="tex-span"><i>i</i></span>-th friend in one particular round in percent.</p>

## Output

<p>Print a single real value&nbsp;— the expectation of the number of rounds provided that Misha plays optimally. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://fZ2J5Z0w.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
2
50 50

```




```input2
4
50 20 20 10

```




```output1
5.0000000000

```




```output2
39.2846263444

```



## Note

<p>The optimal strategy in the first sample is to guess friends alternately.</p>
