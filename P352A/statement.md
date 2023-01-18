## Description

<div><p>Jeff's got <span class="tex-span"><i>n</i></span> cards, each card contains either digit 0, or digit 5. Jeff can choose several cards and put them in a line so that he gets some number. What is the largest possible number divisible by 90 Jeff can make from the cards he's got?</p><p>Jeff must make the number without leading zero. At that, we assume that number 0 doesn't contain any leading zeroes. Jeff doesn't have to use all the cards.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup>)</span>. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 0</span> or <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 5</span>). Number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> represents the digit that is written on the <span class="tex-span"><i>i</i></span>-th card.</p></div><div class="output-specification"><p>In a single line print the answer to the problem — the maximum number, divisible by 90. If you can't make any divisible by 90 number from the cards, print -1.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup>)</span>. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 0</span> or <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 5</span>). Number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> represents the digit that is written on the <span class="tex-span"><i>i</i></span>-th card.</p>

## Output

<p>In a single line print the answer to the problem — the maximum number, divisible by 90. If you can't make any divisible by 90 number from the cards, print -1.</p>





```input1
4
5 0 5 0

```




```input2
11
5 5 5 5 5 5 5 5 0 5 5

```




```output1
0

```




```output2
5555555550

```



## Note

<p>In the first test you can make only one number that is a multiple of 90 — <span class="tex-span">0</span>.</p><p>In the second test you can make number <span class="tex-span">5555555550</span>, it is a multiple of <span class="tex-span">90</span>.</p>
