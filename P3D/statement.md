## Description

<div><p>This is yet another problem on regular bracket sequences.</p><p>A bracket sequence is called regular, if by inserting "<span class="tex-font-style-tt">+</span>" and "<span class="tex-font-style-tt">1</span>" into it we get a correct mathematical expression. For example, sequences "<span class="tex-font-style-tt">(())()</span>", "<span class="tex-font-style-tt">()</span>" and "<span class="tex-font-style-tt">(()(()))</span>" are regular, while "<span class="tex-font-style-tt">)(</span>", "<span class="tex-font-style-tt">(()</span>" and "<span class="tex-font-style-tt">(()))(</span>" are not. You have a pattern of a bracket sequence that consists of characters "<span class="tex-font-style-tt">(</span>", "<span class="tex-font-style-tt">)</span>" and "<span class="tex-font-style-tt">?</span>". You have to replace each character "<span class="tex-font-style-tt">?</span>" with a bracket so, that you get a regular bracket sequence.</p><p>For each character "<span class="tex-font-style-tt">?</span>" the cost of its replacement with "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>" is given. Among all the possible variants your should choose the cheapest.</p></div><div class="input-specification"><p>The first line contains a non-empty pattern of even length, consisting of characters "<span class="tex-font-style-tt">(</span>", "<span class="tex-font-style-tt">)</span>" and "<span class="tex-font-style-tt">?</span>". Its length doesn't exceed <span class="tex-span">5·10<sup class="upper-index">4</sup></span>. Then there follow <span class="tex-span"><i>m</i></span> lines, where <span class="tex-span"><i>m</i></span> is the number of characters "<span class="tex-font-style-tt">?</span>" in the pattern. Each line contains two integer numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>,  <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the cost of replacing the <span class="tex-span"><i>i</i></span>-th character "<span class="tex-font-style-tt">?</span>" with an opening bracket, and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> — with a closing one.</p></div><div class="output-specification"><p>Print the cost of the optimal regular bracket sequence in the first line, and the required sequence in the second.</p><p>Print <span class="tex-font-style-tt">-1</span>, if there is no answer. If the answer is not unique, print any of them. </p></div>

## Input

<p>The first line contains a non-empty pattern of even length, consisting of characters "<span class="tex-font-style-tt">(</span>", "<span class="tex-font-style-tt">)</span>" and "<span class="tex-font-style-tt">?</span>". Its length doesn't exceed <span class="tex-span">5·10<sup class="upper-index">4</sup></span>. Then there follow <span class="tex-span"><i>m</i></span> lines, where <span class="tex-span"><i>m</i></span> is the number of characters "<span class="tex-font-style-tt">?</span>" in the pattern. Each line contains two integer numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>,  <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the cost of replacing the <span class="tex-span"><i>i</i></span>-th character "<span class="tex-font-style-tt">?</span>" with an opening bracket, and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> — with a closing one.</p>

## Output

<p>Print the cost of the optimal regular bracket sequence in the first line, and the required sequence in the second.</p><p>Print <span class="tex-font-style-tt">-1</span>, if there is no answer. If the answer is not unique, print any of them. </p>





```input1
(??)
1 2
2 8

```




```output1
4
()()

```


