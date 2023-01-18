## Description

<div><center> <img class="tex-graphics" src="file://hGWZ2HTV.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Senor Vorpal Kickass'o invented an innovative method to encrypt integer sequences of length <span class="tex-span"><i>n</i></span>. To encrypt a sequence, one has to choose a secret sequence <img align="middle" class="tex-formula" src="file://kz3E7U5i.png" style="max-width: 100.0%;max-height: 100.0%;">, that acts as a key.</p><p>Vorpal is very selective, so the key should be such a sequence <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, that its cyclic shifts are linearly independent, that is, there is no non-zero set of coefficients <span class="tex-span"><i>x</i><sub class="lower-index">0</sub>, <i>x</i><sub class="lower-index">1</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i> - 1</sub></span>, such that <img align="middle" class="tex-formula" src="file://RHwMb3s3.png" style="max-width: 100.0%;max-height: 100.0%;"> for all <span class="tex-span"><i>k</i></span> at the same time.</p><p>After that for a sequence <img align="middle" class="tex-formula" src="file://RcgT38TO.png" style="max-width: 100.0%;max-height: 100.0%;"> you should build the following cipher:</p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://6wd1IqNf.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>In other words, you are to compute the quadratic deviation between each cyclic shift of <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and the sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. The resulting sequence is the Kickass's cipher. The cipher is in development right now and Vorpal wants to decipher a sequence after it has been encrypted. You are to solve this problem for him. You are given sequences <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. You are to find all suitable sequences <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<img align="middle" class="tex-formula" src="file://OzdDuPzA.png" style="max-width: 100.0%;max-height: 100.0%;">).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">0</sub>, <i>b</i><sub class="lower-index">1</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i> - 1</sub></span> (<img align="middle" class="tex-formula" src="file://ks8ZaAm8.png" style="max-width: 100.0%;max-height: 100.0%;">).</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">0</sub>, <i>c</i><sub class="lower-index">1</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i> - 1</sub></span> (<img align="middle" class="tex-formula" src="file://SrHBJfCc.png" style="max-width: 100.0%;max-height: 100.0%;">).</p><p>It is guaranteed that all cyclic shifts of sequence <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are linearly independent.</p></div><div class="output-specification"><p>In the first line print a single integer <span class="tex-span"><i>k</i></span>&nbsp;— the number of sequences <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, such that after encrypting them with key <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> you get the sequence <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>After that in each of <span class="tex-span"><i>k</i></span> next lines print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span>. Print the sequences in lexicographical order.</p><p>Note that <span class="tex-span"><i>k</i></span> could be equal to <span class="tex-span">0</span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<img align="middle" class="tex-formula" src="file://OzdDuPzA.png" style="max-width: 100.0%;max-height: 100.0%;">).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">0</sub>, <i>b</i><sub class="lower-index">1</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i> - 1</sub></span> (<img align="middle" class="tex-formula" src="file://ks8ZaAm8.png" style="max-width: 100.0%;max-height: 100.0%;">).</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">0</sub>, <i>c</i><sub class="lower-index">1</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i> - 1</sub></span> (<img align="middle" class="tex-formula" src="file://SrHBJfCc.png" style="max-width: 100.0%;max-height: 100.0%;">).</p><p>It is guaranteed that all cyclic shifts of sequence <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are linearly independent.</p>

## Output

<p>In the first line print a single integer <span class="tex-span"><i>k</i></span>&nbsp;— the number of sequences <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, such that after encrypting them with key <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> you get the sequence <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>After that in each of <span class="tex-span"><i>k</i></span> next lines print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span>. Print the sequences in lexicographical order.</p><p>Note that <span class="tex-span"><i>k</i></span> could be equal to <span class="tex-span">0</span>.</p>





```input1
1
1
0

```




```input2
1
100
81

```




```input3
3
1 1 3
165 185 197

```




```output1
1
1

```




```output2
2
91
109

```




```output3
2
-6 -9 -1
8 5 13

```


