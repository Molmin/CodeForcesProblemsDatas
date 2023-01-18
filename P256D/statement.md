## Description

<div><p>There are <span class="tex-span"><i>n</i></span> people, sitting in a line at the table. For each person we know that he always tells either the truth or lies.</p><p>Little Serge asked them: how many of you always tell the truth? Each of the people at the table knows everything (who is an honest person and who is a liar) about all the people at the table. The honest people are going to say the correct answer, the liars are going to say any integer from 1 to <span class="tex-span"><i>n</i></span>, which is not the correct answer. Every liar chooses his answer, regardless of the other liars, so two distinct liars may give distinct answer.</p><p>Serge does not know any information about the people besides their answers to his question. He took a piece of paper and wrote <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the answer of the <span class="tex-span"><i>i</i></span>-th person in the row. Given this sequence, Serge determined that exactly <span class="tex-span"><i>k</i></span> people sitting at the table <span class="tex-font-style-bf">apparently lie</span>.</p><p>Serge wonders, how many variants of people's answers (sequences of answers <span class="tex-span"><i>a</i></span> of length <span class="tex-span"><i>n</i></span>) there are where one can say that exactly <span class="tex-span"><i>k</i></span> people sitting at the table apparently lie. As there can be rather many described variants of answers, count the remainder of dividing the number of the variants by <span class="tex-span">777777777</span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span">(1 ≤ <i>k</i> ≤ <i>n</i> ≤ 2<sup class="upper-index">8</sup>)</span>. It is guaranteed that <span class="tex-span"><i>n</i></span> — is the power of number 2.</p></div><div class="output-specification"><p>Print a single integer — the answer to the problem modulo <span class="tex-span">777777777</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span">(1 ≤ <i>k</i> ≤ <i>n</i> ≤ 2<sup class="upper-index">8</sup>)</span>. It is guaranteed that <span class="tex-span"><i>n</i></span> — is the power of number 2.</p>

## Output

<p>Print a single integer — the answer to the problem modulo <span class="tex-span">777777777</span>.</p>





```input1
1 1

```




```input2
2 1

```




```output1
0

```




```output2
2

```


