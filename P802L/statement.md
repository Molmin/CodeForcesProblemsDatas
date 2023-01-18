## Description

<div><p>Heidi is terrified by your estimate and she found it unrealistic that her friends would collaborate to drive her into debt. She expects that, actually, each person will just pick a random friend to send Heidi to. (This randomness assumption implies, however, that she can now visit the same friend an arbitrary number of times...) Moreover, if a person only has one friend in common with Heidi (i.e., if that person is in a leaf of the tree), then that person will not send Heidi back (so that Heidi's travel will end at some point).</p><p>Heidi also found unrealistic the assumption that she can make all the travels in one day. Therefore now she assumes that every time she travels a route between two friends, she needs to buy a new ticket. She wants to know: how much should she expect to spend on the trips?</p><p>For what it's worth, Heidi knows that Jenny has at least two friends.</p></div><div class="input-specification"><p>The first line contains the number of friends <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The next <span class="tex-span"><i>n</i> - 1</span> lines each contain three space-separated integers <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">0 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i> - 1</span>, <span class="tex-span">1 ≤ <i>c</i> ≤ 10<sup class="upper-index">4</sup></span>) meaning that <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> are friends and the cost for traveling between <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> is <span class="tex-span"><i>c</i></span> (paid every time!).</p><p>It is again guaranteed that the social network of the input forms a tree.</p></div><div class="output-specification"><p>Assume that the expected cost of the trips is written as an irreducible fraction <span class="tex-span"><i>a</i> / <i>b</i></span> (that is, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are coprime). Then Heidi, the weird cow that she is, asks you to output <img align="middle" class="tex-formula" src="file://AF3Lwgu9.png" style="max-width: 100.0%;max-height: 100.0%;">. (Output a single integer between <span class="tex-span">0</span> and <span class="tex-span">10<sup class="upper-index">9</sup> + 6</span>.)</p></div>

## Input

<p>The first line contains the number of friends <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The next <span class="tex-span"><i>n</i> - 1</span> lines each contain three space-separated integers <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">0 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i> - 1</span>, <span class="tex-span">1 ≤ <i>c</i> ≤ 10<sup class="upper-index">4</sup></span>) meaning that <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> are friends and the cost for traveling between <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> is <span class="tex-span"><i>c</i></span> (paid every time!).</p><p>It is again guaranteed that the social network of the input forms a tree.</p>

## Output

<p>Assume that the expected cost of the trips is written as an irreducible fraction <span class="tex-span"><i>a</i> / <i>b</i></span> (that is, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are coprime). Then Heidi, the weird cow that she is, asks you to output <img align="middle" class="tex-formula" src="file://AF3Lwgu9.png" style="max-width: 100.0%;max-height: 100.0%;">. (Output a single integer between <span class="tex-span">0</span> and <span class="tex-span">10<sup class="upper-index">9</sup> + 6</span>.)</p>





```input1
3
0 1 10
0 2 20

```




```input2
4
0 1 3
0 2 9
0 3 27

```




```input3
7
0 1 3
0 5 7
1 2 2
1 3 1
1 4 5
5 6 8

```




```input4
11
1 0 6646
2 0 8816
3 2 9375
4 2 5950
5 1 8702
6 2 2657
7 2 885
8 7 2660
9 2 5369
10 6 3798

```




```input5
6
0 1 8
0 2 24
1 3 40
1 4 16
4 5 8

```




```output1
15

```




```output2
13

```




```output3
400000019

```




```output4
153869806

```




```output5
39

```



## Note

<p>In the first example, with probability <span class="tex-span">1 / 2</span> Heidi will go to <span class="tex-span">1</span> from <span class="tex-span">0</span>, and with probability <span class="tex-span">1 / 2</span> she will go to <span class="tex-span">2</span>. In the first case the cost would be <span class="tex-span">10</span>, and in the second it would be <span class="tex-span">20</span>. After reaching <span class="tex-span">1</span> or <span class="tex-span">2</span> she will stop, as <span class="tex-span">1</span> and <span class="tex-span">2</span> are leaves of the social tree. Hence, the expected cost she has to pay is <span class="tex-span">10·1 / 2 + 20·1 / 2 = 15</span>.</p><p>In the third example, the expected cost is <span class="tex-span">81 / 5</span>. You should output <span class="tex-span">400000019</span>.</p><p>In her travels, Heidi has learned an intriguing fact about the structure of her social network. She tells you the following: <span class="tex-font-style-it">The mysterious determinant that you might be wondering about is such that it does not cause strange errors in your reasonable solution...</span> Did we mention that Heidi is a weird cow?</p>
