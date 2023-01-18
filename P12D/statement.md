## Description

<div><p><span class="tex-span"><i>N</i></span> ladies attend the ball in the King's palace. Every lady can be described with three values: beauty, intellect and richness. King's Master of Ceremonies knows that ladies are very special creatures. If some lady understands that there is other lady at the ball which is more beautiful, smarter and more rich, she can jump out of the window. He knows values of all ladies and wants to find out how many probable self-murderers will be on the ball. Lets denote beauty of the <span class="tex-span"><i>i</i></span>-th lady by <span class="tex-span"><i>B</i><sub class="lower-index"><i>i</i></sub></span>, her intellect by <span class="tex-span"><i>I</i><sub class="lower-index"><i>i</i></sub></span> and her richness by <span class="tex-span"><i>R</i><sub class="lower-index"><i>i</i></sub></span>. Then <span class="tex-span"><i>i</i></span>-th lady is a probable self-murderer if there is some <span class="tex-span"><i>j</i></span>-th lady that <span class="tex-span"><i>B</i><sub class="lower-index"><i>i</i></sub> &lt; <i>B</i><sub class="lower-index"><i>j</i></sub>, <i>I</i><sub class="lower-index"><i>i</i></sub> &lt; <i>I</i><sub class="lower-index"><i>j</i></sub>, <i>R</i><sub class="lower-index"><i>i</i></sub> &lt; <i>R</i><sub class="lower-index"><i>j</i></sub></span>. Find the number of probable self-murderers.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 500000</span>). The second line contains <span class="tex-span"><i>N</i></span> integer numbers <span class="tex-span"><i>B</i><sub class="lower-index"><i>i</i></sub></span>, separated by single spaces. The third and the fourth lines contain sequences <span class="tex-span"><i>I</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>R</i><sub class="lower-index"><i>i</i></sub></span> in the same format. It is guaranteed that <span class="tex-span">0 ≤ <i>B</i><sub class="lower-index"><i>i</i></sub>, <i>I</i><sub class="lower-index"><i>i</i></sub>, <i>R</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>.</p></div><div class="output-specification"><p>Output the answer to the problem.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 500000</span>). The second line contains <span class="tex-span"><i>N</i></span> integer numbers <span class="tex-span"><i>B</i><sub class="lower-index"><i>i</i></sub></span>, separated by single spaces. The third and the fourth lines contain sequences <span class="tex-span"><i>I</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>R</i><sub class="lower-index"><i>i</i></sub></span> in the same format. It is guaranteed that <span class="tex-span">0 ≤ <i>B</i><sub class="lower-index"><i>i</i></sub>, <i>I</i><sub class="lower-index"><i>i</i></sub>, <i>R</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>.</p>

## Output

<p>Output the answer to the problem.</p>





```input1
3
1 4 2
4 3 2
2 5 3

```




```output1
1

```


