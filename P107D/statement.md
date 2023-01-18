## Description

<div><p>Zeyad wants to commit <span class="tex-span"><i>n</i></span> crimes in Egypt and not be punished at the end. There are several types of crimes. For example, bribery is a crime but is not considered such when repeated twice. Therefore, bribery is not considered a crime when repeated an even number of times. Speeding is a crime, but is not considered such when repeated a number of times which is a multiple of five.</p><p>More specifically, <span class="tex-span"><i>c</i></span> conditions on crime repetitions are known. Each condition describes the crime type <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and its multiplicity <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span>. If the number of times Zeyad committed the crime <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is a multiple of <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span>, Zeyad will not be punished for crime <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>. Some crimes may be listed more than once. In this case fulfilling at least one condition for this crime is enough to not be punished for it. Of course, if for certain crime the number of times Zeyad committed it is zero, he is innocent with respect to this crime.</p><p>Now Zeyad is interested in a number of ways he can commit exactly <span class="tex-span"><i>n</i></span> crimes without any punishment.</p><p>The order of commiting the crimes matters. More formally, two ways, sequences <span class="tex-span"><i>w</i>1</span> and <span class="tex-span"><i>w</i>2</span>, of committing <span class="tex-span"><i>n</i></span> crimes are equal if <span class="tex-span"><i>w</i>1<sub class="lower-index"><i>i</i></sub> = <i>w</i>2<sub class="lower-index"><i>i</i></sub></span>, for all <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup>, 0 ≤ <i>c</i> ≤ 1000</span>) — the number of crimes Zeyad would like to commit and the number of conditions he is aware of.</p><p>Then the definitions for <span class="tex-span"><i>c</i></span> conditions follow. There are <span class="tex-span">26</span> types of crimes. Each crime definition consists of crime type — a capital Latin letter — and its multiplicity. </p><p>The multiplicity of each crime is a positive integer number and the product of all multiplicities does not exceed <span class="tex-span">123</span>. Some conditions may be repeated in the input more than once.</p><p>Crime of multiplicity <span class="tex-span">1</span> is not yielding any punishment regardless of the number of times it was committed. The strictness of the law is compensated by the fact that it's non-mandatory.</p><p>Obviously, if some crime is not listed in the set of conditions, then Zeyad will not consider it, as committing it would unavoidably lead to the punishment.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span> stream (you may also use the <span class="tex-font-style-tt">%I64d</span> specificator).</p></div><div class="output-specification"><p>Output the number of different ways Zeyad can commit exactly <span class="tex-span"><i>n</i></span> crimes with no punishment modulo <span class="tex-span">12345</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup>, 0 ≤ <i>c</i> ≤ 1000</span>) — the number of crimes Zeyad would like to commit and the number of conditions he is aware of.</p><p>Then the definitions for <span class="tex-span"><i>c</i></span> conditions follow. There are <span class="tex-span">26</span> types of crimes. Each crime definition consists of crime type — a capital Latin letter — and its multiplicity. </p><p>The multiplicity of each crime is a positive integer number and the product of all multiplicities does not exceed <span class="tex-span">123</span>. Some conditions may be repeated in the input more than once.</p><p>Crime of multiplicity <span class="tex-span">1</span> is not yielding any punishment regardless of the number of times it was committed. The strictness of the law is compensated by the fact that it's non-mandatory.</p><p>Obviously, if some crime is not listed in the set of conditions, then Zeyad will not consider it, as committing it would unavoidably lead to the punishment.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span> stream (you may also use the <span class="tex-font-style-tt">%I64d</span> specificator).</p>

## Output

<p>Output the number of different ways Zeyad can commit exactly <span class="tex-span"><i>n</i></span> crimes with no punishment modulo <span class="tex-span">12345</span>.</p>





```input1
5 2
A 1
B 2

```




```input2
6 3
A 1
B 2
C 3

```




```input3
8 3
A 2
A 3
B 2

```




```output1
16

```




```output2
113

```




```output3
128

```



## Note

<p>In the first test case, the 16 ways are: AAAAA, AAABB, AABAB, AABBA, ABAAB, ABABA, ABBAA, BAAAB, BAABA, BABAA, BBAAA, ABBBB, BABBB, BBABB, BBBAB, BBBBA.</p>
