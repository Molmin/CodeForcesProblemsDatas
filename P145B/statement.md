## Description

<div><p><span class="tex-font-style-underline">Petya loves lucky numbers very much. Everybody knows that lucky numbers are positive integers whose decimal record contains only the lucky digits <span class="tex-font-style-bf">4</span> and <span class="tex-font-style-bf">7</span>. For example, numbers <span class="tex-font-style-bf">47</span>, <span class="tex-font-style-bf">744</span>, <span class="tex-font-style-bf">4</span> are lucky and <span class="tex-font-style-bf">5</span>, <span class="tex-font-style-bf">17</span>, <span class="tex-font-style-bf">467</span> are not.</span></p><p>Petya loves long lucky numbers very much. He is interested in the <span class="tex-font-style-bf">minimum</span> lucky number <span class="tex-span"><i>d</i></span> that meets some condition. Let <span class="tex-span"><i>cnt</i>(<i>x</i>)</span> be the number of occurrences of number <span class="tex-span"><i>x</i></span> in number <span class="tex-span"><i>d</i></span> as a substring. For example, if <span class="tex-span"><i>d</i> = 747747</span>, then <span class="tex-span"><i>cnt</i>(4) = 2</span>, <span class="tex-span"><i>cnt</i>(7) = 4</span>, <span class="tex-span"><i>cnt</i>(47) = 2</span>, <span class="tex-span"><i>cnt</i>(74) = 2</span>. Petya wants the following condition to fulfil simultaneously: <span class="tex-span"><i>cnt</i>(4) = <i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>cnt</i>(7) = <i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>cnt</i>(47) = <i>a</i><sub class="lower-index">3</sub></span>, <span class="tex-span"><i>cnt</i>(74) = <i>a</i><sub class="lower-index">4</sub></span>. Petya is not interested in the occurrences of other numbers. Help him cope with this task.</p></div><div class="input-specification"><p>The single line contains four integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">3</sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index">4</sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub>, <i>a</i><sub class="lower-index">4</sub> ≤ 10<sup class="upper-index">6</sup></span>).</p></div><div class="output-specification"><p>On the single line print without leading zeroes the answer to the problem — the minimum lucky number <span class="tex-span"><i>d</i></span> such, that <span class="tex-span"><i>cnt</i>(4) = <i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>cnt</i>(7) = <i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>cnt</i>(47) = <i>a</i><sub class="lower-index">3</sub></span>, <span class="tex-span"><i>cnt</i>(74) = <i>a</i><sub class="lower-index">4</sub></span>. If such number does not exist, print the single number "-1" (without the quotes).</p></div>

## Input

<p>The single line contains four integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">3</sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index">4</sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub>, <i>a</i><sub class="lower-index">4</sub> ≤ 10<sup class="upper-index">6</sup></span>).</p>

## Output

<p>On the single line print without leading zeroes the answer to the problem — the minimum lucky number <span class="tex-span"><i>d</i></span> such, that <span class="tex-span"><i>cnt</i>(4) = <i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>cnt</i>(7) = <i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>cnt</i>(47) = <i>a</i><sub class="lower-index">3</sub></span>, <span class="tex-span"><i>cnt</i>(74) = <i>a</i><sub class="lower-index">4</sub></span>. If such number does not exist, print the single number "-1" (without the quotes).</p>





```input1
2 2 1 1

```




```input2
4 7 3 1

```




```output1
4774

```




```output2
-1

```


