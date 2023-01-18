## Description

<div><p>Vasya became interested in bioinformatics. He's going to write an article about similar cyclic DNA sequences, so he invented a new method for determining the similarity of cyclic sequences.</p><p>Let's assume that strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> have the same length <span class="tex-span"><i>n</i></span>, then the function <span class="tex-span"><i>h</i>(<i>s</i>, <i>t</i>)</span> is defined as the number of positions in which the respective symbols of <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> are <span class="tex-font-style-it">the same</span>. Function <span class="tex-span"><i>h</i>(<i>s</i>, <i>t</i>)</span> can be used to define the function of Vasya distance <span class="tex-span">ρ(<i>s</i>, <i>t</i>)</span>: </p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://PCQenOld.png" style="max-width: 100.0%;max-height: 100.0%;"></center> where <img align="middle" class="tex-formula" src="file://dcq4M3pi.png" style="max-width: 100.0%;max-height: 100.0%;"> is obtained from string <span class="tex-span"><i>s</i></span>, by applying left circular shift <span class="tex-span"><i>i</i></span> times. For example, <center class="tex-equation"><span class="tex-span">ρ("<i>AGC</i>", "<i>CGT</i>") = </span></center> <center class="tex-equation"><span class="tex-span"><i>h</i>("<i>AGC</i>", "<i>CGT</i>") + <i>h</i>("<i>AGC</i>", "<i>GTC</i>") + <i>h</i>("<i>AGC</i>", "<i>TCG</i>") + </span></center> <center class="tex-equation"><span class="tex-span"><i>h</i>("<i>GCA</i>", "<i>CGT</i>") + <i>h</i>("<i>GCA</i>", "<i>GTC</i>") + <i>h</i>("<i>GCA</i>", "<i>TCG</i>") + </span></center> <center class="tex-equation"><span class="tex-span"><i>h</i>("<i>CAG</i>", "<i>CGT</i>") + <i>h</i>("<i>CAG</i>", "<i>GTC</i>") + <i>h</i>("<i>CAG</i>", "<i>TCG</i>") = </span></center> <center class="tex-equation"><span class="tex-span">1 + 1 + 0 + 0 + 1 + 1 + 1 + 0 + 1 = 6</span></center><p>Vasya found a string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span> on the Internet. Now he wants to count how many strings <span class="tex-span"><i>t</i></span> there are such that the Vasya distance from the string <span class="tex-span"><i>s</i></span> attains maximum possible value. Formally speaking, <span class="tex-span"><i>t</i></span> must satisfy the equation: <img align="middle" class="tex-formula" src="file://7jwcp5ZV.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Vasya could not try all possible strings to find an answer, so he needs your help. As the answer may be very large, count the number of such strings modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line of the input contains a single string of length <span class="tex-span"><i>n</i></span>, consisting of characters <span class="tex-font-style-tt">"ACGT"</span>.</p></div><div class="output-specification"><p>Print a single number&nbsp;— the answer modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line of the input contains a single string of length <span class="tex-span"><i>n</i></span>, consisting of characters <span class="tex-font-style-tt">"ACGT"</span>.</p>

## Output

<p>Print a single number&nbsp;— the answer modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
1
C

```




```input2
2
AG

```




```input3
3
TTT

```




```output1
1

```




```output2
4

```




```output3
1

```



## Note

<p>Please note that if for two distinct strings <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span> values <span class="tex-span">ρ(<i>s</i>, <i>t</i><sub class="lower-index">1</sub>)</span> и <span class="tex-span">ρ(<i>s</i>, <i>t</i><sub class="lower-index">2</sub>)</span> are maximum among all possible <span class="tex-span"><i>t</i></span>, then both strings must be taken into account in the answer even if one of them can be obtained by a circular shift of another one.</p><p>In the first sample, there is <span class="tex-span">ρ("<i>C</i>", "<i>C</i>") = 1</span>, for the remaining strings <span class="tex-span"><i>t</i></span> of length 1 the value of <span class="tex-span">ρ(<i>s</i>, <i>t</i>)</span> is 0.</p><p>In the second sample, <span class="tex-span">ρ("<i>AG</i>", "<i>AG</i>") = ρ("<i>AG</i>", "<i>GA</i>") = ρ("<i>AG</i>", "<i>AA</i>") = ρ("<i>AG</i>", "<i>GG</i>") = 4</span>.</p><p>In the third sample, <span class="tex-span">ρ("<i>TTT</i>", "<i>TTT</i>") = 27</span></p>
