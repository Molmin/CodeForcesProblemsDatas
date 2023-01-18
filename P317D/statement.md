## Description

<div><p>Vasya and Petya wrote down all integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> to play the "powers" game (<span class="tex-span"><i>n</i></span> can be quite large; however, Vasya and Petya are not confused by this fact).</p><p>Players choose numbers in turn (Vasya chooses first). If some number <span class="tex-span"><i>x</i></span> is chosen at the current turn, it is forbidden to choose <span class="tex-span"><i>x</i></span> or all of its other positive integer powers (that is, <span class="tex-span"><i>x</i><sup class="upper-index">2</sup></span>, <span class="tex-span"><i>x</i><sup class="upper-index">3</sup></span>, <span class="tex-span">...</span>) at the next turns. For instance, if the number <span class="tex-span">9</span> is chosen at the first turn, one cannot choose <span class="tex-span">9</span> or <span class="tex-span">81</span> later, while it is still allowed to choose <span class="tex-span">3</span> or <span class="tex-span">27</span>. The one who cannot make a move loses.</p><p>Who wins if both Vasya and Petya play optimally?</p></div><div class="input-specification"><p>Input contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print the name of the winner — "<span class="tex-font-style-tt">Vasya</span>" or "<span class="tex-font-style-tt">Petya</span>" (without quotes).</p></div>

## Input

<p>Input contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print the name of the winner — "<span class="tex-font-style-tt">Vasya</span>" or "<span class="tex-font-style-tt">Petya</span>" (without quotes).</p>





```input1
1

```




```input2
2

```




```input3
8

```




```output1
Vasya

```




```output2
Petya

```




```output3
Petya

```



## Note

<p>In the first sample Vasya will choose 1 and win immediately.</p><p>In the second sample no matter which number Vasya chooses during his first turn, Petya can choose the remaining number and win.</p>
