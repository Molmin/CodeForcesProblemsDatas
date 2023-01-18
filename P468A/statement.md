## Description

<div><p>Little X used to play a card game called "24 Game", but recently he has found it too easy. So he invented a new game.</p><p>Initially you have a sequence of <span class="tex-span"><i>n</i></span> integers: <span class="tex-span">1, 2, ..., <i>n</i></span>. In a single step, you can pick two of them, let's denote them <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, erase them from the sequence, and append to the sequence either <span class="tex-span"><i>a</i> + <i>b</i></span>, or <span class="tex-span"><i>a</i> - <i>b</i></span>, or <span class="tex-span"><i>a</i> × <i>b</i></span>.</p><p>After <span class="tex-span"><i>n</i> - 1</span> steps there is only one number left. Can you make this number equal to <span class="tex-span">24</span>?</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p></div><div class="output-specification"><p>If it's possible, print "<span class="tex-font-style-tt">YES</span>" in the first line. Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p><p>If there is a way to obtain <span class="tex-span">24</span> as the result number, in the following <span class="tex-span"><i>n</i> - 1</span> lines print the required operations an operation per line. Each operation should be in form: "<span class="tex-span"><i>a</i></span> <span class="tex-span"><i>op</i></span> <span class="tex-span"><i>b</i></span> = <span class="tex-span"><i>c</i></span>". Where <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are the numbers you've picked at this operation; <span class="tex-span"><i>op</i></span> is either "<span class="tex-font-style-tt">+</span>", or "<span class="tex-font-style-tt">-</span>", or "<span class="tex-font-style-tt">*</span>"; <span class="tex-span"><i>c</i></span> is the result of corresponding operation. Note, that the absolute value of <span class="tex-span"><i>c</i></span> mustn't be greater than <span class="tex-span">10<sup class="upper-index">18</sup></span>. The result of the last operation must be equal to <span class="tex-span">24</span>. Separate operator sign and equality sign from numbers with spaces.</p><p>If there are multiple valid answers, you may print any of them.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p>

## Output

<p>If it's possible, print "<span class="tex-font-style-tt">YES</span>" in the first line. Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p><p>If there is a way to obtain <span class="tex-span">24</span> as the result number, in the following <span class="tex-span"><i>n</i> - 1</span> lines print the required operations an operation per line. Each operation should be in form: "<span class="tex-span"><i>a</i></span> <span class="tex-span"><i>op</i></span> <span class="tex-span"><i>b</i></span> = <span class="tex-span"><i>c</i></span>". Where <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are the numbers you've picked at this operation; <span class="tex-span"><i>op</i></span> is either "<span class="tex-font-style-tt">+</span>", or "<span class="tex-font-style-tt">-</span>", or "<span class="tex-font-style-tt">*</span>"; <span class="tex-span"><i>c</i></span> is the result of corresponding operation. Note, that the absolute value of <span class="tex-span"><i>c</i></span> mustn't be greater than <span class="tex-span">10<sup class="upper-index">18</sup></span>. The result of the last operation must be equal to <span class="tex-span">24</span>. Separate operator sign and equality sign from numbers with spaces.</p><p>If there are multiple valid answers, you may print any of them.</p>





```input1
1

```




```input2
8

```




```output1
NO

```




```output2
YES
8 * 7 = 56
6 * 5 = 30
3 - 4 = -1
1 - 2 = -1
30 - -1 = 31
56 - 31 = 25
25 + -1 = 24

```


