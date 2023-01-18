## Description

<div><p>One fine morning, <span class="tex-span"><i>n</i></span> fools lined up in a row. After that, they numbered each other with numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, inclusive. Each fool got a unique number. The fools decided not to change their numbers before the end of the fun.</p><p>Every fool has exactly <span class="tex-span"><i>k</i></span> bullets and a pistol. In addition, the fool number <span class="tex-span"><i>i</i></span> has probability of <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (in percent) that he kills the fool he shoots at.</p><p>The fools decided to have several rounds of the fun. Each round of the fun looks like this: each currently living fool shoots at another living fool with the smallest number (a fool is not stupid enough to shoot at himself). All shots of the round are perfomed at one time (simultaneously). If there is exactly one living fool, he does not shoot.</p><p>Let's define a <span class="tex-font-style-it">situation</span> as the set of numbers of all the living fools at the some time. We say that a situation is <span class="tex-font-style-it">possible</span> if for some integer number <span class="tex-span"><i>j</i></span> (<span class="tex-span">0 ≤ <i>j</i> ≤ <i>k</i></span>) there is a nonzero probability that after <span class="tex-span"><i>j</i></span> rounds of the fun this situation will occur.</p><p>Valera knows numbers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> and <span class="tex-span"><i>k</i></span>. Help Valera determine the number of distinct <span class="tex-font-style-it">possible situations</span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 3000</span>) — the initial number of fools and the number of bullets for each fool.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the given probabilities (in percent).</p></div><div class="output-specification"><p>Print a single number — the answer to the problem.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 3000</span>) — the initial number of fools and the number of bullets for each fool.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the given probabilities (in percent).</p>

## Output

<p>Print a single number — the answer to the problem.</p>





```input1
3 3
50 50 50

```




```input2
1 1
100

```




```input3
2 1
100 100

```




```input4
3 3
0 0 0

```




```output1
7

```




```output2
1

```




```output3
2

```




```output4
1

```



## Note

<p>In the first sample, any situation is possible, except for situation <span class="tex-span">{1, 2}</span>.</p><p>In the second sample there is exactly one fool, so he does not make shots.</p><p>In the third sample the possible situations are <span class="tex-span">{1, 2}</span> (after zero rounds) and the "empty" situation <span class="tex-span">{}</span> (after one round).</p><p>In the fourth sample, the only possible situation is <span class="tex-span">{1, 2, 3}</span>.</p>
