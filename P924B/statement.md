## Description

<div><p>An atom of element X can exist in <span class="tex-span"><i>n</i></span> distinct states with energies <span class="tex-span"><i>E</i><sub class="lower-index">1</sub> &lt; <i>E</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>E</i><sub class="lower-index"><i>n</i></sub></span>. Arkady wants to build a laser on this element, using a three-level scheme. Here is a simplified description of the scheme. </p><p>Three distinct states <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>j</i></span> and <span class="tex-span"><i>k</i></span> are selected, where <span class="tex-span"><i>i</i> &lt; <i>j</i> &lt; <i>k</i></span>. After that the following process happens: </p><ol> <li> initially the atom is in the state <span class="tex-span"><i>i</i></span>,</li><li> we spend <span class="tex-span"><i>E</i><sub class="lower-index"><i>k</i></sub> - <i>E</i><sub class="lower-index"><i>i</i></sub></span> energy to put the atom in the state <span class="tex-span"><i>k</i></span>,</li><li> the atom emits a photon with useful energy <span class="tex-span"><i>E</i><sub class="lower-index"><i>k</i></sub> - <i>E</i><sub class="lower-index"><i>j</i></sub></span> and changes its state to the state <span class="tex-span"><i>j</i></span>,</li><li> the atom spontaneously changes its state to the state <span class="tex-span"><i>i</i></span>, losing energy <span class="tex-span"><i>E</i><sub class="lower-index"><i>j</i></sub> - <i>E</i><sub class="lower-index"><i>i</i></sub></span>,</li><li> the process repeats from step 1. </li></ol><p>Let's define the energy conversion efficiency as <img align="middle" class="tex-formula" src="file://F3tTJlWI.png" style="max-width: 100.0%;max-height: 100.0%;">, i.&nbsp;e. the ration between the useful energy of the photon and spent energy.</p><p>Due to some limitations, Arkady can only choose such three states that <span class="tex-span"><i>E</i><sub class="lower-index"><i>k</i></sub> - <i>E</i><sub class="lower-index"><i>i</i></sub> ≤ <i>U</i></span>.</p><p>Help Arkady to find such the maximum possible energy conversion efficiency within the above constraints.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>U</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>U</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of states and the maximum possible difference between <span class="tex-span"><i>E</i><sub class="lower-index"><i>k</i></sub></span> and <span class="tex-span"><i>E</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>The second line contains a sequence of integers <span class="tex-span"><i>E</i><sub class="lower-index">1</sub>, <i>E</i><sub class="lower-index">2</sub>, ..., <i>E</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>E</i><sub class="lower-index">1</sub> &lt; <i>E</i><sub class="lower-index">2</sub>... &lt; <i>E</i><sub class="lower-index"><i>n</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). It is guaranteed that all <span class="tex-span"><i>E</i><sub class="lower-index"><i>i</i></sub></span> are given in increasing order.</p></div><div class="output-specification"><p>If it is not possible to choose three states that satisfy all constraints, print <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise, print one real number <span class="tex-span">η</span>&nbsp;— the maximum possible energy conversion efficiency. Your answer is considered correct its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p><p>Formally, let your answer be <span class="tex-span"><i>a</i></span>, and the jury's answer be <span class="tex-span"><i>b</i></span>. Your answer is considered correct if <img align="middle" class="tex-formula" src="file://eIHBYVBa.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>U</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>U</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of states and the maximum possible difference between <span class="tex-span"><i>E</i><sub class="lower-index"><i>k</i></sub></span> and <span class="tex-span"><i>E</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>The second line contains a sequence of integers <span class="tex-span"><i>E</i><sub class="lower-index">1</sub>, <i>E</i><sub class="lower-index">2</sub>, ..., <i>E</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>E</i><sub class="lower-index">1</sub> &lt; <i>E</i><sub class="lower-index">2</sub>... &lt; <i>E</i><sub class="lower-index"><i>n</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). It is guaranteed that all <span class="tex-span"><i>E</i><sub class="lower-index"><i>i</i></sub></span> are given in increasing order.</p>

## Output

<p>If it is not possible to choose three states that satisfy all constraints, print <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise, print one real number <span class="tex-span">η</span>&nbsp;— the maximum possible energy conversion efficiency. Your answer is considered correct its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p><p>Formally, let your answer be <span class="tex-span"><i>a</i></span>, and the jury's answer be <span class="tex-span"><i>b</i></span>. Your answer is considered correct if <img align="middle" class="tex-formula" src="file://eIHBYVBa.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
4 4
1 3 5 7

```




```input2
10 8
10 13 15 16 17 19 20 22 24 25

```




```input3
3 1
2 5 10

```




```output1
0.5

```




```output2
0.875

```




```output3
-1

```



## Note

<p>In the first example choose states <span class="tex-span">1</span>, <span class="tex-span">2</span> and <span class="tex-span">3</span>, so that the energy conversion efficiency becomes equal to <img align="middle" class="tex-formula" src="file://3qa14E16.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>In the second example choose states <span class="tex-span">4</span>, <span class="tex-span">5</span> and <span class="tex-span">9</span>, so that the energy conversion efficiency becomes equal to <img align="middle" class="tex-formula" src="file://SATsCkPN.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
