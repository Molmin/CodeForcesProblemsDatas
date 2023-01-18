## Description

<div><p>A robber has attempted to rob a bank but failed to complete his task. However, he had managed to open all the safes.</p><p>Oleg the bank client loves money (who doesn't), and decides to take advantage of this failed robbery and steal some money from the safes. There are many safes arranged in a line, where the <span class="tex-span"><i>i</i></span>-th safe from the left is called safe <span class="tex-span"><i>i</i></span>. There are <span class="tex-span"><i>n</i></span> banknotes left in all the safes in total. The <span class="tex-span"><i>i</i></span>-th banknote is in safe <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>. Oleg is now at safe <span class="tex-span"><i>a</i></span>. There are two security guards, one of which guards the safe <span class="tex-span"><i>b</i></span> such that <span class="tex-span"><i>b</i> &lt; <i>a</i></span>, i.e. the first guard is to the left of Oleg. The other guard guards the safe <span class="tex-span"><i>c</i></span> so that <span class="tex-span"><i>c</i> &gt; <i>a</i></span>, i.e. he is to the right of Oleg.</p><p>The two guards are very lazy, so they do not move. In every second, Oleg can either take all the banknotes from the current safe or move to any of the neighboring safes. However, he cannot visit any safe that is guarded by security guards at any time, becaues he might be charged for stealing. Determine the maximum amount of banknotes Oleg can gather.</p></div><div class="input-specification"><p>The first line of input contains three space-separated integers, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>b</i> &lt; <i>a</i> &lt; <i>c</i> ≤ 10<sup class="upper-index">9</sup></span>), denoting the positions of Oleg, the first security guard and the second security guard, respectively.</p><p>The next line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), denoting the number of banknotes.</p><p>The next line of input contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), denoting that the <span class="tex-span"><i>i</i></span>-th banknote is located in the <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>-th safe. Note that <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> are <span class="tex-font-style-bf">not</span> guaranteed to be distinct.</p></div><div class="output-specification"><p>Output a single integer: the maximum number of banknotes Oleg can take.</p></div>

## Input

<p>The first line of input contains three space-separated integers, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>b</i> &lt; <i>a</i> &lt; <i>c</i> ≤ 10<sup class="upper-index">9</sup></span>), denoting the positions of Oleg, the first security guard and the second security guard, respectively.</p><p>The next line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), denoting the number of banknotes.</p><p>The next line of input contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), denoting that the <span class="tex-span"><i>i</i></span>-th banknote is located in the <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>-th safe. Note that <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> are <span class="tex-font-style-bf">not</span> guaranteed to be distinct.</p>

## Output

<p>Output a single integer: the maximum number of banknotes Oleg can take.</p>





```input1
5 3 7
8
4 7 5 5 3 6 2 8

```




```input2
6 5 7
5
1 5 7 92 3

```




```output1
4

```




```output2
0

```



## Note

<p>In the first example Oleg can take the banknotes in positions <span class="tex-span">4</span>, <span class="tex-span">5</span>, <span class="tex-span">6</span> (note that there are <span class="tex-span">2</span> banknotes at position <span class="tex-span">5</span>). Oleg can't take the banknotes in safes <span class="tex-span">7</span> and <span class="tex-span">8</span> because he can't run into the second security guard. Similarly, Oleg cannot take the banknotes at positions <span class="tex-span">3</span> and <span class="tex-span">2</span> because he can't run into the first security guard. Thus, he can take a maximum of <span class="tex-span">4</span> banknotes.</p><p>For the second sample, Oleg can't take any banknotes without bumping into any of the security guards.</p>
