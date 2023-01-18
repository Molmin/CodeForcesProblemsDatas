## Description

<div><p>Hamed has recently found a string <span class="tex-span"><i>t</i></span> and suddenly became quite fond of it. He spent several days trying to find all occurrences of <span class="tex-span"><i>t</i></span> in other strings he had. Finally he became tired and started thinking about the following problem. Given a string <span class="tex-span"><i>s</i></span> how many ways are there to extract <span class="tex-span"><i>k</i> ≥ 1</span> non-overlapping substrings from it such that each of them contains string <span class="tex-span"><i>t</i></span> as a substring? More formally, you need to calculate the number of ways to choose two sequences <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>k</i></sub></span> satisfying the following requirements:</p><ul> <li> <span class="tex-span"><i>k</i> ≥ 1</span> </li><li> <img align="middle" class="tex-formula" src="file://usfTV1sk.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> <img align="middle" class="tex-formula" src="file://e5MbX5eM.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> <img align="middle" class="tex-formula" src="file://9SqR2RYb.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> <img align="middle" class="tex-formula" src="file://Q7QLU0tZ.png" style="max-width: 100.0%;max-height: 100.0%;">&nbsp;&nbsp;<span class="tex-span"><i>t</i></span> is a substring of string <span class="tex-span"><i>s</i><sub class="lower-index"><i>a</i><sub class="lower-index"><i>i</i></sub></sub><i>s</i><sub class="lower-index"><i>a</i><sub class="lower-index"><i>i</i></sub> + 1</sub>... <i>s</i><sub class="lower-index"><i>b</i><sub class="lower-index"><i>i</i></sub></sub></span> (string <span class="tex-span"><i>s</i></span> is considered as <span class="tex-span">1</span>-indexed). </li></ul><p>As the number of ways can be rather large print it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>Input consists of two lines containing strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ |<i>s</i>|, |<i>t</i>| ≤ 10<sup class="upper-index">5</sup></span>). Each string consists of lowercase Latin letters.</p></div><div class="output-specification"><p>Print the answer in a single line.</p></div>

## Input

<p>Input consists of two lines containing strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ |<i>s</i>|, |<i>t</i>| ≤ 10<sup class="upper-index">5</sup></span>). Each string consists of lowercase Latin letters.</p>

## Output

<p>Print the answer in a single line.</p>





```input1
ababa
aba

```




```input2
welcometoroundtwohundredandeightytwo
d

```




```input3
ddd
d

```




```output1
5

```




```output2
274201

```




```output3
12

```


