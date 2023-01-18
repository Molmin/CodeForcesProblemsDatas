## Description

<div><p>Goshtasp was known to be a good programmer in his school. One day Vishtasp, Goshtasp's friend, asked him to solve this task:</p><p><span class="tex-font-style-underline">Given a positive integer <span class="tex-span"><i>n</i></span>, you should determine whether <span class="tex-span"><i>n</i></span> is rich.</span></p><p>The positive integer <span class="tex-span"><i>x</i></span> is rich, if there exists some set of distinct numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span> such that <img align="middle" class="tex-formula" src="file://mN3crfG6.png" style="max-width: 100.0%;max-height: 100.0%;">. In addition: every <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> should be either a prime number, or equal to <span class="tex-span">1</span>.</p><p>Vishtasp said that he would share his Eidi <span class="tex-span">50 / 50</span> with Goshtasp, if he could solve the task. Eidi is money given to children for Noruz by their parents and/or relatives.</p><p>Goshtasp needs to solve this problem to get money, you need to solve it to get score!</p></div><div class="input-specification"><p>Input contains a single positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10000</span>).</p></div><div class="output-specification"><p>If the number is not rich print <span class="tex-span">0</span>. Otherwise print the numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span>. If several solutions exist print the lexicographically <span class="tex-font-style-underline">latest</span> solution. Answers are compared as sequences of numbers, not as strings.</p><p>For comparing two sequences <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> we first find the first index <span class="tex-span"><i>i</i></span> such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>, if <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub></span> then <span class="tex-span"><i>a</i></span> is lexicographically earlier and if <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> &lt; <i>a</i><sub class="lower-index"><i>i</i></sub></span> then <span class="tex-span"><i>b</i></span> is lexicographically earlier. If <span class="tex-span"><i>m</i> ≠ <i>n</i></span> we add zeroes at the end of the smaller sequence (only for the moment of comparison) and then perform the comparison.</p><p>You do not need to minimize the number of elements in sequence (i.e. <span class="tex-span"><i>m</i></span>). You just need to print the lexicographically <span class="tex-font-style-underline">latest</span> solution.</p><p>See samples to find out how to print the sequence.</p></div>

## Input

<p>Input contains a single positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10000</span>).</p>

## Output

<p>If the number is not rich print <span class="tex-span">0</span>. Otherwise print the numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span>. If several solutions exist print the lexicographically <span class="tex-font-style-underline">latest</span> solution. Answers are compared as sequences of numbers, not as strings.</p><p>For comparing two sequences <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> we first find the first index <span class="tex-span"><i>i</i></span> such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>, if <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub></span> then <span class="tex-span"><i>a</i></span> is lexicographically earlier and if <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> &lt; <i>a</i><sub class="lower-index"><i>i</i></sub></span> then <span class="tex-span"><i>b</i></span> is lexicographically earlier. If <span class="tex-span"><i>m</i> ≠ <i>n</i></span> we add zeroes at the end of the smaller sequence (only for the moment of comparison) and then perform the comparison.</p><p>You do not need to minimize the number of elements in sequence (i.e. <span class="tex-span"><i>m</i></span>). You just need to print the lexicographically <span class="tex-font-style-underline">latest</span> solution.</p><p>See samples to find out how to print the sequence.</p>





```input1
11

```




```input2
545

```




```output1
11=11

```




```output2
541+3+1=545

```


