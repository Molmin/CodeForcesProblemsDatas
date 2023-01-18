## Description

<div><p>Ancient Egyptians are known to have used a large set of symbols <img align="middle" class="tex-formula" src="file://o9zGVGS7.png" style="max-width: 100.0%;max-height: 100.0%;"> to write on the walls of the temples. Fafa and Fifa went to one of the temples and found two non-empty words <span class="tex-span"><i>S</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>S</i><sub class="lower-index">2</sub></span> of equal lengths on the wall of temple written one below the other. Since this temple is very ancient, some symbols from the words were erased. The symbols in the set <img align="middle" class="tex-formula" src="file://L3tRP44m.png" style="max-width: 100.0%;max-height: 100.0%;"> have equal probability for being in the position of any erased symbol.</p><p>Fifa challenged Fafa to calculate the probability that <span class="tex-span"><i>S</i><sub class="lower-index">1</sub></span> is lexicographically greater than <span class="tex-span"><i>S</i><sub class="lower-index">2</sub></span>. Can you help Fafa with this task?</p><p>You know that <img align="middle" class="tex-formula" src="file://TGISeWh9.png" style="max-width: 100.0%;max-height: 100.0%;">, i.&nbsp;e. there were <span class="tex-span"><i>m</i></span> distinct characters in Egyptians' alphabet, in this problem these characters are denoted by integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> in alphabet order. A word <span class="tex-span"><i>x</i></span> is lexicographically greater than a word <span class="tex-span"><i>y</i></span> of the same length, if the words are same up to some position, and then the word <span class="tex-span"><i>x</i></span> has a larger character, than the word <span class="tex-span"><i>y</i></span>.</p><p>We can prove that the probability equals to some fraction <img align="middle" class="tex-formula" src="file://CA1cQpIA.png" style="max-width: 100.0%;max-height: 100.0%;">, where <span class="tex-span"><i>P</i></span> and <span class="tex-span"><i>Q</i></span> are coprime integers, and <img align="middle" class="tex-formula" src="file://WaoWHDrB.png" style="max-width: 100.0%;max-height: 100.0%;">. Print as the answer the value <img align="middle" class="tex-formula" src="file://qmkqVc6H.png" style="max-width: 100.0%;max-height: 100.0%;">, i.&nbsp;e. such a non-negative integer less than <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>, such that <img align="middle" class="tex-formula" src="file://Q7DwRLPY.png" style="max-width: 100.0%;max-height: 100.0%;">, where <img align="middle" class="tex-formula" src="file://Cca0aCxf.png" style="max-width: 100.0%;max-height: 100.0%;"> means that <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> give the same remainders when divided by <span class="tex-span"><i>m</i></span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>,  <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the length of each of the two words and the size of the alphabet <img align="middle" class="tex-formula" src="file://AZ5jUR5u.png" style="max-width: 100.0%;max-height: 100.0%;">, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>) — the symbols of <span class="tex-span"><i>S</i><sub class="lower-index">1</sub></span>. If <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 0</span>, then the symbol at position <span class="tex-span"><i>i</i></span> was erased.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers representing <span class="tex-span"><i>S</i><sub class="lower-index">2</sub></span> with the same format as <span class="tex-span"><i>S</i><sub class="lower-index">1</sub></span>.</p></div><div class="output-specification"><p>Print the value <img align="middle" class="tex-formula" src="file://85n8cLqB.png" style="max-width: 100.0%;max-height: 100.0%;">, where <span class="tex-span"><i>P</i></span> and <span class="tex-span"><i>Q</i></span> are coprime and <img align="middle" class="tex-formula" src="file://1vNvMFpm.png" style="max-width: 100.0%;max-height: 100.0%;"> is the answer to the problem.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>,  <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the length of each of the two words and the size of the alphabet <img align="middle" class="tex-formula" src="file://AZ5jUR5u.png" style="max-width: 100.0%;max-height: 100.0%;">, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>) — the symbols of <span class="tex-span"><i>S</i><sub class="lower-index">1</sub></span>. If <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 0</span>, then the symbol at position <span class="tex-span"><i>i</i></span> was erased.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers representing <span class="tex-span"><i>S</i><sub class="lower-index">2</sub></span> with the same format as <span class="tex-span"><i>S</i><sub class="lower-index">1</sub></span>.</p>

## Output

<p>Print the value <img align="middle" class="tex-formula" src="file://85n8cLqB.png" style="max-width: 100.0%;max-height: 100.0%;">, where <span class="tex-span"><i>P</i></span> and <span class="tex-span"><i>Q</i></span> are coprime and <img align="middle" class="tex-formula" src="file://1vNvMFpm.png" style="max-width: 100.0%;max-height: 100.0%;"> is the answer to the problem.</p>





```input1
1 2
0
1

```




```input2
1 2
1
0

```




```input3
7 26
0 15 12 9 13 0 14
11 1 0 13 15 12 0

```




```output1
500000004

```




```output2
0

```




```output3
230769233

```



## Note

<p>In the first sample, the first word can be converted into (<span class="tex-span">1</span>) or (<span class="tex-span">2</span>). The second option is the only one that will make it lexicographically larger than the second word. So, the answer to the problem will be <img align="middle" class="tex-formula" src="file://kStHnI48.png" style="max-width: 100.0%;max-height: 100.0%;">, that is <span class="tex-span">500000004</span>, because <img align="middle" class="tex-formula" src="file://C5urTx7t.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>In the second example, there is no replacement for the zero in the second word that will make the first one lexicographically larger. So, the answer to the problem is <img align="middle" class="tex-formula" src="file://ILhA7HNt.png" style="max-width: 100.0%;max-height: 100.0%;">, that is <span class="tex-span">0</span>.</p>
