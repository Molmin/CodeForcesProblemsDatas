## Description

<div><p>A boy named Gena really wants to get to the "Russian Code Cup" finals, or at least get a t-shirt. But the offered problems are too complex, so he made an arrangement with his <span class="tex-span"><i>n</i></span> friends that they will solve the problems for him.</p><p>The participants are offered <span class="tex-span"><i>m</i></span> problems on the contest. For each friend, Gena knows what problems he can solve. But Gena's friends won't agree to help Gena for nothing: the <span class="tex-span"><i>i</i></span>-th friend asks Gena <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> rubles for his help <span class="tex-font-style-bf">in solving all the problems</span> he can. Also, the friend agreed to write a code for Gena only if Gena's computer is connected to at least <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> monitors, each monitor costs <span class="tex-span"><i>b</i></span> rubles.</p><p>Gena is careful with money, so he wants to spend as little money as possible to solve all the problems. Help Gena, tell him how to spend the smallest possible amount of money. Initially, there's no monitors connected to Gena's computer.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>; <span class="tex-span">1 ≤ <i>m</i> ≤ 20</span>; <span class="tex-span">1 ≤ <i>b</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of Gena's friends, the number of problems and the cost of a single monitor.</p><p>The following <span class="tex-span">2<i>n</i></span> lines describe the friends. Lines number <span class="tex-span">2<i>i</i></span> and <span class="tex-span">(2<i>i</i> + 1)</span> contain the information about the <span class="tex-span"><i>i</i></span>-th friend. The <span class="tex-span">2<i>i</i></span>-th line contains three integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>; <span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>; <span class="tex-span">1 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>)&nbsp;— the desired amount of money, monitors and the number of problems the friend can solve. The <span class="tex-span">(2<i>i</i> + 1)</span>-th line contains <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> distinct positive integers&nbsp;— the numbers of problems that the <span class="tex-span"><i>i</i></span>-th friend can solve. The problems are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>.</p></div><div class="output-specification"><p>Print the minimum amount of money Gena needs to spend to solve all the problems. Or print -1, if this cannot be achieved.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>; <span class="tex-span">1 ≤ <i>m</i> ≤ 20</span>; <span class="tex-span">1 ≤ <i>b</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of Gena's friends, the number of problems and the cost of a single monitor.</p><p>The following <span class="tex-span">2<i>n</i></span> lines describe the friends. Lines number <span class="tex-span">2<i>i</i></span> and <span class="tex-span">(2<i>i</i> + 1)</span> contain the information about the <span class="tex-span"><i>i</i></span>-th friend. The <span class="tex-span">2<i>i</i></span>-th line contains three integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>; <span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>; <span class="tex-span">1 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>)&nbsp;— the desired amount of money, monitors and the number of problems the friend can solve. The <span class="tex-span">(2<i>i</i> + 1)</span>-th line contains <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> distinct positive integers&nbsp;— the numbers of problems that the <span class="tex-span"><i>i</i></span>-th friend can solve. The problems are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>.</p>

## Output

<p>Print the minimum amount of money Gena needs to spend to solve all the problems. Or print -1, if this cannot be achieved.</p>





```input1
2 2 1
100 1 1
2
100 2 1
1

```




```input2
3 2 5
100 1 1
1
100 1 1
2
200 1 2
1 2

```




```input3
1 2 1
1 1 1
1

```




```output1
202

```




```output2
205

```




```output3
-1

```


