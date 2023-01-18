## Description

<div><p>Pasha has two hamsters: Arthur and Alexander. Pasha put <span class="tex-span"><i>n</i></span> apples in front of them. Pasha knows which apples Arthur likes. Similarly, Pasha knows which apples Alexander likes. Pasha doesn't want any conflict between the hamsters (as they may like the same apple), so he decided to distribute the apples between the hamsters on his own. He is going to give some apples to Arthur and some apples to Alexander. It doesn't matter how many apples each hamster gets but it is important that each hamster gets only the apples he likes. It is possible that somebody doesn't get any apples.</p><p>Help Pasha distribute all the apples between the hamsters. Note that Pasha wants to distribute all the apples, not just some of them.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100;&nbsp;1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i>)</span> — the number of apples Pasha has, the number of apples Arthur likes and the number of apples Alexander likes, correspondingly.</p><p>The next line contains <span class="tex-span"><i>a</i></span> distinct integers — the numbers of the apples Arthur likes. The next line contains <span class="tex-span"><i>b</i></span> distinct integers — the numbers of the apples Alexander likes.</p><p>Assume that the apples are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The input is such that the answer exists.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> characters, each of them equals either 1 or 2. If the <span class="tex-span"><i>i</i></span>-h character equals 1, then the <span class="tex-span"><i>i</i></span>-th apple should be given to Arthur, otherwise it should be given to Alexander. If there are multiple correct answers, you are allowed to print any of them.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100;&nbsp;1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i>)</span> — the number of apples Pasha has, the number of apples Arthur likes and the number of apples Alexander likes, correspondingly.</p><p>The next line contains <span class="tex-span"><i>a</i></span> distinct integers — the numbers of the apples Arthur likes. The next line contains <span class="tex-span"><i>b</i></span> distinct integers — the numbers of the apples Alexander likes.</p><p>Assume that the apples are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The input is such that the answer exists.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> characters, each of them equals either 1 or 2. If the <span class="tex-span"><i>i</i></span>-h character equals 1, then the <span class="tex-span"><i>i</i></span>-th apple should be given to Arthur, otherwise it should be given to Alexander. If there are multiple correct answers, you are allowed to print any of them.</p>





```input1
4 2 3
1 2
2 3 4

```




```input2
5 5 2
3 4 1 2 5
2 3

```




```output1
1 1 2 2

```




```output2
1 1 1 1 1

```


