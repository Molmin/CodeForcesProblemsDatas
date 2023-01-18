## Description

<div><p>Recently a serious bug has been found in the FOS code. The head of the F company wants to find the culprit and punish him. For that, he set up an organizational meeting, the issue is: who's bugged the code? Each of the <span class="tex-span"><i>n</i></span> coders on the meeting said: 'I know for sure that either <span class="tex-span"><i>x</i></span> or <span class="tex-span"><i>y</i></span> did it!'</p><p>The head of the company decided to choose two suspects and invite them to his office. Naturally, he should consider the coders' opinions. That's why the head wants to make such a choice that at least <span class="tex-span"><i>p</i></span> of <span class="tex-span"><i>n</i></span> coders agreed with it. A coder agrees with the choice of two suspects if at least one of the two people that he named at the meeting was chosen as a suspect. In how many ways can the head of F choose two suspects?</p><p>Note that even if some coder was chosen as a suspect, he can agree with the head's choice if he named the other chosen coder at the meeting.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>p</i></span> <span class="tex-span">(3 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup>;&nbsp;0 ≤ <i>p</i> ≤ <i>n</i>)</span> — the number of coders in the F company and the minimum number of agreed people.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the numbers of coders named by the <span class="tex-span"><i>i</i></span>-th coder. It is guaranteed that <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>i</i>, &nbsp;<i>y</i><sub class="lower-index"><i>i</i></sub> ≠ <i>i</i>, &nbsp;<i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="output-specification"><p>Print a single integer –– the number of possible two-suspect sets. Note that the order of the suspects doesn't matter, that is, sets <span class="tex-span">(1, 2)</span> и <span class="tex-span">(2, 1)</span> are considered identical.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>p</i></span> <span class="tex-span">(3 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup>;&nbsp;0 ≤ <i>p</i> ≤ <i>n</i>)</span> — the number of coders in the F company and the minimum number of agreed people.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the numbers of coders named by the <span class="tex-span"><i>i</i></span>-th coder. It is guaranteed that <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>i</i>, &nbsp;<i>y</i><sub class="lower-index"><i>i</i></sub> ≠ <i>i</i>, &nbsp;<i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub></span>.</p>

## Output

<p>Print a single integer –– the number of possible two-suspect sets. Note that the order of the suspects doesn't matter, that is, sets <span class="tex-span">(1, 2)</span> и <span class="tex-span">(2, 1)</span> are considered identical.</p>





```input1
4 2
2 3
1 4
1 4
2 1

```




```input2
8 6
5 6
5 7
5 8
6 2
2 1
7 3
1 3
1 4

```




```output1
6

```




```output2
1

```


