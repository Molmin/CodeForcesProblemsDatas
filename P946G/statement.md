## Description

<div><p>We call an array <span class="tex-font-style-it">almost increasing</span> if we can erase not more than one element from it so that the array becomes strictly increasing (that is, every element is striclty greater than every element before it).</p><p>You are given an array <span class="tex-span"><i>a</i></span> consisting of <span class="tex-span"><i>n</i></span> elements. You are allowed to replace any element with any integer number (and you may do so any number of times you need). What is the minimum number of replacements you have to perform in order to make the array <span class="tex-font-style-it">almost increasing</span>?</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200000</span>) — the number of elements in <span class="tex-span"><i>a</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the array <span class="tex-span"><i>a</i></span>.</p></div><div class="output-specification"><p>Print the minimum number of replaces you have to perform so that <span class="tex-span"><i>a</i></span> is <span class="tex-font-style-it">almost increasing</span>.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200000</span>) — the number of elements in <span class="tex-span"><i>a</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the array <span class="tex-span"><i>a</i></span>.</p>

## Output

<p>Print the minimum number of replaces you have to perform so that <span class="tex-span"><i>a</i></span> is <span class="tex-font-style-it">almost increasing</span>.</p>





```input1
5
5 4 3 2 1

```




```input2
5
1 2 8 9 5

```




```output1
3

```




```output2
0

```


