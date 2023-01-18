## Description

<div><p>Recently Max has got himself into popular CCG "BrainStone". As "BrainStone" is a pretty intellectual game, Max has to solve numerous hard problems during the gameplay. Here is one of them:</p><p>Max owns <span class="tex-span"><i>n</i></span> creatures, <span class="tex-span"><i>i</i></span>-th of them can be described with two numbers — its health <span class="tex-span"><i>hp</i><sub class="lower-index"><i>i</i></sub></span> and its damage <span class="tex-span"><i>dmg</i><sub class="lower-index"><i>i</i></sub></span>. Max also has two types of spells in stock:</p><ol> <li> Doubles health of the creature (<span class="tex-span"><i>hp</i><sub class="lower-index"><i>i</i></sub></span> := <span class="tex-span"><i>hp</i><sub class="lower-index"><i>i</i></sub>·2</span>); </li><li> Assigns value of <span class="tex-font-style-bf">health</span> of the creature to its <span class="tex-font-style-bf">damage</span> (<span class="tex-span"><i>dmg</i><sub class="lower-index"><i>i</i></sub></span> := <span class="tex-span"><i>hp</i><sub class="lower-index"><i>i</i></sub></span>). </li></ol><p>Spell of first type can be used no more than <span class="tex-span"><i>a</i></span> times in total, of the second type — no more than <span class="tex-span"><i>b</i></span> times in total. Spell can be used on a certain creature multiple times. Spells can be used in arbitrary order. It isn't necessary to use all the spells.</p><p>Max is really busy preparing for his final exams, so he asks you to determine what is the maximal total damage of all creatures he can achieve if he uses spells in most optimal way.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>a</i> ≤ 20</span>, <span class="tex-span">0 ≤ <i>b</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of creatures, spells of the first type and spells of the second type, respectively.</p><p>The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>n</i></span> lines contain two number <span class="tex-span"><i>hp</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>dmg</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>hp</i><sub class="lower-index"><i>i</i></sub>, <i>dmg</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — description of the <span class="tex-span"><i>i</i></span>-th creature.</p></div><div class="output-specification"><p>Print single integer — maximum total damage creatures can deal.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>a</i> ≤ 20</span>, <span class="tex-span">0 ≤ <i>b</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of creatures, spells of the first type and spells of the second type, respectively.</p><p>The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>n</i></span> lines contain two number <span class="tex-span"><i>hp</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>dmg</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>hp</i><sub class="lower-index"><i>i</i></sub>, <i>dmg</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — description of the <span class="tex-span"><i>i</i></span>-th creature.</p>

## Output

<p>Print single integer — maximum total damage creatures can deal.</p>





```input1
2 1 1
10 15
6 1

```




```input2
3 0 3
10 8
7 11
5 2

```




```output1
27

```




```output2
26

```



## Note

<p>In the first example Max should use the spell of the first type on the second creature, then the spell of the second type on the same creature. Then total damage will be equal to <span class="tex-span">15 + 6·2 = 27</span>.</p><p>In the second example Max should use the spell of the second type on the first creature, then the spell of the second type on the third creature. Total damage will be equal to <span class="tex-span">10 + 11 + 5 = 26</span>.</p>
