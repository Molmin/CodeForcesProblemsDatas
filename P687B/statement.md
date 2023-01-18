## Description

<div><p>Today Pari and Arya are playing a game called Remainders.</p><p>Pari chooses two positive integer <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>k</i></span>, and tells Arya <span class="tex-span"><i>k</i></span> but not <span class="tex-span"><i>x</i></span>. Arya have to find the value <img align="middle" class="tex-formula" src="file://b4DLkm0D.png" style="max-width: 100.0%;max-height: 100.0%;">. There are <span class="tex-span"><i>n</i></span> ancient numbers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> and Pari has to tell Arya <img align="middle" class="tex-formula" src="file://CXBExkhp.png" style="max-width: 100.0%;max-height: 100.0%;"> if Arya wants. Given <span class="tex-span"><i>k</i></span> and the ancient values, tell us if Arya has a winning strategy independent of value of <span class="tex-span"><i>x</i></span> or not. Formally, is it true that Arya can understand the value <img align="middle" class="tex-formula" src="file://jQ6u0rDp.png" style="max-width: 100.0%;max-height: 100.0%;"> for any positive integer <span class="tex-span"><i>x</i></span>?</p><p>Note, that <img align="middle" class="tex-formula" src="file://QtK96MGh.png" style="max-width: 100.0%;max-height: 100.0%;"> means the remainder of <span class="tex-span"><i>x</i></span> after dividing it by <span class="tex-span"><i>y</i></span>.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>,  <i>k</i> ≤ 1 000 000</span>)&nbsp;— the number of ancient integers and value <span class="tex-span"><i>k</i></span> that is chosen by Pari.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>).</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">Yes</span>" (without quotes) if Arya has a winning strategy independent of value of <span class="tex-span"><i>x</i></span>, or "<span class="tex-font-style-tt">No</span>" (without quotes) otherwise.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>,  <i>k</i> ≤ 1 000 000</span>)&nbsp;— the number of ancient integers and value <span class="tex-span"><i>k</i></span> that is chosen by Pari.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>).</p>

## Output

<p>Print "<span class="tex-font-style-tt">Yes</span>" (without quotes) if Arya has a winning strategy independent of value of <span class="tex-span"><i>x</i></span>, or "<span class="tex-font-style-tt">No</span>" (without quotes) otherwise.</p>





```input1
4 5
2 3 5 12

```




```input2
2 7
2 3

```




```output1
Yes

```




```output2
No

```



## Note

<p>In the first sample, Arya can understand <img align="middle" class="tex-formula" src="file://ALzp44rV.png" style="max-width: 100.0%;max-height: 100.0%;"> because <span class="tex-span">5</span> is one of the ancient numbers.</p><p>In the second sample, Arya can't be sure what <img align="middle" class="tex-formula" src="file://NH5JoWQI.png" style="max-width: 100.0%;max-height: 100.0%;"> is. For example <span class="tex-span">1</span> and <span class="tex-span">7</span> have the same remainders after dividing by <span class="tex-span">2</span> and <span class="tex-span">3</span>, but they differ in remainders after dividing by <span class="tex-span">7</span>.</p>
