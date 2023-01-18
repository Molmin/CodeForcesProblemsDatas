## Description

<div><p>The rules of Sith Tournament are well known to everyone. <span class="tex-span"><i>n</i></span> Sith take part in the Tournament. The Tournament starts with the random choice of two Sith who will fight in the first battle. As one of them loses, his place is taken by the next randomly chosen Sith who didn't fight before. Does it need to be said that each battle in the Sith Tournament ends with a death of one of opponents? The Tournament ends when the only Sith remains alive.</p><p>Jedi Ivan accidentally appeared in the list of the participants in the Sith Tournament. However, his skills in the Light Side of the Force are so strong so he can influence the choice of participants either who start the Tournament or who take the loser's place after each battle. Of course, he won't miss his chance to take advantage of it. Help him to calculate the probability of his victory.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 18</span>)&nbsp;— the number of participants of the Sith Tournament.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>n</i></span> real numbers, which form a matrix <span class="tex-span"><i>p</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>ij</i></sub> ≤ 1</span>). Each its element <span class="tex-span"><i>p</i><sub class="lower-index"><i>ij</i></sub></span> is the probability that the <span class="tex-span"><i>i</i></span>-th participant defeats the <span class="tex-span"><i>j</i></span>-th in a duel.</p><p>The elements on the main diagonal <span class="tex-span"><i>p</i><sub class="lower-index"><i>ii</i></sub></span> are equal to zero. For all different <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>j</i></span> the equality <span class="tex-span"><i>p</i><sub class="lower-index"><i>ij</i></sub> + <i>p</i><sub class="lower-index"><i>ji</i></sub> = 1</span> holds. All probabilities are given with no more than six decimal places.</p><p>Jedi Ivan is the number <span class="tex-span">1</span> in the list of the participants.</p></div><div class="output-specification"><p>Output a real number&nbsp;— the probability that Jedi Ivan will stay alive after the Tournament. Absolute or relative error of the answer must not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 18</span>)&nbsp;— the number of participants of the Sith Tournament.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>n</i></span> real numbers, which form a matrix <span class="tex-span"><i>p</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>ij</i></sub> ≤ 1</span>). Each its element <span class="tex-span"><i>p</i><sub class="lower-index"><i>ij</i></sub></span> is the probability that the <span class="tex-span"><i>i</i></span>-th participant defeats the <span class="tex-span"><i>j</i></span>-th in a duel.</p><p>The elements on the main diagonal <span class="tex-span"><i>p</i><sub class="lower-index"><i>ii</i></sub></span> are equal to zero. For all different <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>j</i></span> the equality <span class="tex-span"><i>p</i><sub class="lower-index"><i>ij</i></sub> + <i>p</i><sub class="lower-index"><i>ji</i></sub> = 1</span> holds. All probabilities are given with no more than six decimal places.</p><p>Jedi Ivan is the number <span class="tex-span">1</span> in the list of the participants.</p>

## Output

<p>Output a real number&nbsp;— the probability that Jedi Ivan will stay alive after the Tournament. Absolute or relative error of the answer must not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
3
0.0 0.5 0.8
0.5 0.0 0.4
0.2 0.6 0.0

```




```output1
0.680000000000000

```


