## Description

<div><p>The capital of Berland has <span class="tex-span"><i>n</i></span> multifloor buildings. The architect who built up the capital was very creative, so all the houses were built in one row.</p><p>Let's enumerate all the houses from left to right, starting with one. A house is considered to be <span class="tex-font-style-it">luxurious</span> if the number of floors in it is strictly greater than in all the houses with larger numbers. In other words, a house is luxurious if the number of floors in it is strictly greater than in all the houses, which are located to the right from it. In this task it is assumed that the heights of floors in the houses are the same.</p><p>The new architect is interested in <span class="tex-span"><i>n</i></span> questions, <span class="tex-span"><i>i</i></span>-th of them is about the following: "how many floors should be added to the <span class="tex-span"><i>i</i></span>-th house to make it luxurious?" (for all <span class="tex-span"><i>i</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, inclusive). You need to help him cope with this task.</p><p>Note that all these questions are independent from each other — the answer to the question for house <span class="tex-span"><i>i</i></span> does not affect other answers (i.e., the floors to the houses are not actually added).</p></div><div class="input-specification"><p>The first line of the input contains a single number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of houses in the capital of Berland.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated positive integers <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> equals the number of floors in the <span class="tex-span"><i>i</i></span>-th house. </p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, where number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of floors that need to be added to the house number <span class="tex-span"><i>i</i></span> to make it luxurious. If the house is already luxurious and nothing needs to be added to it, then <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> should be equal to zero.</p><p>All houses are numbered from left to right, starting from one.</p></div>

## Input

<p>The first line of the input contains a single number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of houses in the capital of Berland.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated positive integers <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> equals the number of floors in the <span class="tex-span"><i>i</i></span>-th house. </p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, where number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of floors that need to be added to the house number <span class="tex-span"><i>i</i></span> to make it luxurious. If the house is already luxurious and nothing needs to be added to it, then <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> should be equal to zero.</p><p>All houses are numbered from left to right, starting from one.</p>





```input1
5
1 2 3 1 2

```




```input2
4
3 2 1 4

```




```output1
3 2 0 2 0
```




```output2
2 3 4 0
```


