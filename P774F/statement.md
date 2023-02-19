## Description

<div><p>Stepan has <span class="tex-span"><i>n</i></span> pens. Every day he uses them, and on the <span class="tex-span"><i>i</i></span>-th day he uses the pen number <span class="tex-span"><i>i</i></span>. On the <span class="tex-span">(<i>n</i> + 1)</span>-th day again he uses the pen number <span class="tex-span">1</span>, on the <span class="tex-span">(<i>n</i> + 2)</span>-th — he uses the pen number <span class="tex-span">2</span> and so on.</p><p>On every working day (from Monday to Saturday, inclusive) Stepan spends exactly <span class="tex-span">1</span> milliliter of ink of the pen he uses that day. On Sunday Stepan has a day of rest, he does not stend the ink of the pen he uses that day. </p><p>Stepan knows the current volume of ink in each of his pens. Now it's the <span class="tex-font-style-bf">Monday morning</span> and Stepan is going to use the pen <span class="tex-font-style-bf">number <span class="tex-span">1</span></span> today. Your task is to determine which pen will run out of ink before all the rest (that is, there will be no ink left in it), if Stepan will use the pens according to the conditions described above.</p></div><div class="input-specification"><p>The first line contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50 000</span>) — the number of pens Stepan has.</p><p>The second line contains the sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is equal to the number of milliliters of ink which the pen number <span class="tex-span"><i>i</i></span> currently has.</p></div><div class="output-specification"><p>Print the index of the pen which will run out of ink before all (it means that there will be no ink left in it), if Stepan will use pens according to the conditions described above. </p><p>Pens are numbered in the order they are given in input data. The numeration begins from one. </p><p>Note that the answer is always unambiguous, since several pens can not end at the same time.</p></div>

## Input

<p>The first line contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50 000</span>) — the number of pens Stepan has.</p><p>The second line contains the sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is equal to the number of milliliters of ink which the pen number <span class="tex-span"><i>i</i></span> currently has.</p>

## Output

<p>Print the index of the pen which will run out of ink before all (it means that there will be no ink left in it), if Stepan will use pens according to the conditions described above. </p><p>Pens are numbered in the order they are given in input data. The numeration begins from one. </p><p>Note that the answer is always unambiguous, since several pens can not end at the same time.</p>





```input1
3
3 3 3

```




```input2
5
5 4 5 4 4

```




```output1
2

```




```output2
5

```



## Note

<p>In the first test Stepan uses ink of pens as follows: </p><ol> <li> on the day number <span class="tex-span">1</span> (Monday) Stepan will use the pen number <span class="tex-span">1</span>, after that there will be <span class="tex-span">2</span> milliliters of ink in it; </li><li> on the day number <span class="tex-span">2</span> (Tuesday) Stepan will use the pen number <span class="tex-span">2</span>, after that there will be <span class="tex-span">2</span> milliliters of ink in it; </li><li> on the day number <span class="tex-span">3</span> (Wednesday) Stepan will use the pen number <span class="tex-span">3</span>, after that there will be <span class="tex-span">2</span> milliliters of ink in it; </li><li> on the day number <span class="tex-span">4</span> (Thursday) Stepan will use the pen number <span class="tex-span">1</span>, after that there will be <span class="tex-span">1</span> milliliters of ink in it; </li><li> on the day number <span class="tex-span">5</span> (Friday) Stepan will use the pen number <span class="tex-span">2</span>, after that there will be <span class="tex-span">1</span> milliliters of ink in it; </li><li> on the day number <span class="tex-span">6</span> (Saturday) Stepan will use the pen number <span class="tex-span">3</span>, after that there will be <span class="tex-span">1</span> milliliters of ink in it; </li><li> on the day number <span class="tex-span">7</span> (Sunday) Stepan will use the pen number <span class="tex-span">1</span>, but it is a day of rest so he will not waste ink of this pen in it; </li><li> on the day number <span class="tex-span">8</span> (Monday) Stepan will use the pen number <span class="tex-span">2</span>, after that this pen will run out of ink. </li></ol><p>So, the first pen which will not have ink is the pen number <span class="tex-span">2</span>.</p>
