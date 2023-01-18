## Description

<div><p>Bob came to a cash &amp; carry store, put <span class="tex-span"><i>n</i></span> items into his trolley, and went to the checkout counter to pay. Each item is described by its price <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and time <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> in seconds that a checkout assistant spends on this item. While the checkout assistant is occupied with some item, Bob can steal some other items from his trolley. To steal one item Bob needs exactly 1 second. What is the minimum amount of money that Bob will have to pay to the checkout assistant? Remember, please, that it is Bob, who determines the order of items for the checkout assistant.</p></div><div class="input-specification"><p>The first input line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>). In each of the following <span class="tex-span"><i>n</i></span> lines each item is described by a pair of numbers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2000, 1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is 0, Bob won't be able to steal anything, while the checkout assistant is occupied with item <span class="tex-span"><i>i</i></span>.</p></div><div class="output-specification"><p>Output one number — answer to the problem: what is the minimum amount of money that Bob will have to pay.</p></div>

## Input

<p>The first input line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>). In each of the following <span class="tex-span"><i>n</i></span> lines each item is described by a pair of numbers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2000, 1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is 0, Bob won't be able to steal anything, while the checkout assistant is occupied with item <span class="tex-span"><i>i</i></span>.</p>

## Output

<p>Output one number — answer to the problem: what is the minimum amount of money that Bob will have to pay.</p>





```input1
4
2 10
0 20
1 5
1 3

```




```input2
3
0 1
0 10
0 100

```




```output1
8

```




```output2
111

```


