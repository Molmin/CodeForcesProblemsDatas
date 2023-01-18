## Description

<div><p>Nastya likes reading and even spends whole days in a library sometimes. Today she found a chronicle of Byteland in the library, and it stated that there lived shamans long time ago. It is known that at every moment there was exactly one shaman in Byteland, and there were <span class="tex-span"><i>n</i></span> shamans in total enumerated with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in the order they lived. Also, each shaman had a magic power which can now be expressed as an integer.</p><p>The chronicle includes a list of powers of the <span class="tex-span"><i>n</i></span> shamans. Also, some shamans can be king-shamans, if they gathered all the power of their predecessors, i.e. their power is exactly the sum of powers of all previous shamans. Nastya is interested in whether there was at least one king-shaman in Byteland.</p><p>Unfortunately many of the powers are unreadable in the list, so Nastya is doing the following:</p><ul> <li> Initially she supposes some power for each shaman. </li><li> After that she changes the power of some shaman <span class="tex-span"><i>q</i></span> times (the shamans can differ) and after that wants to check if there is at least one king-shaman in the list. If yes, she wants to know the index of any king-shaman. </li></ul><p>Unfortunately the list is too large and Nastya wants you to help her.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>q</i> ≤ 2·10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the magic power of the <span class="tex-span"><i>i</i></span>-th shaman.</p><p>After that <span class="tex-span"><i>q</i></span> lines follow, the <span class="tex-span"><i>i</i></span>-th of them contains two integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) that mean that the new power of the <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>-th shaman is <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>q</i></span> lines, the <span class="tex-span"><i>i</i></span>-th of them should contain <span class="tex-span"> - 1</span>, if after the <span class="tex-span"><i>i</i></span>-th change there are no shaman-kings, and otherwise a single integer <span class="tex-span"><i>j</i></span>, where <span class="tex-span"><i>j</i></span> is an index of some king-shaman after the <span class="tex-span"><i>i</i></span>-th change.</p><p>If there are multiple king-shamans after each change, print the index of any of them.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>q</i> ≤ 2·10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the magic power of the <span class="tex-span"><i>i</i></span>-th shaman.</p><p>After that <span class="tex-span"><i>q</i></span> lines follow, the <span class="tex-span"><i>i</i></span>-th of them contains two integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) that mean that the new power of the <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>-th shaman is <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>.</p>

## Output

<p>Print <span class="tex-span"><i>q</i></span> lines, the <span class="tex-span"><i>i</i></span>-th of them should contain <span class="tex-span"> - 1</span>, if after the <span class="tex-span"><i>i</i></span>-th change there are no shaman-kings, and otherwise a single integer <span class="tex-span"><i>j</i></span>, where <span class="tex-span"><i>j</i></span> is an index of some king-shaman after the <span class="tex-span"><i>i</i></span>-th change.</p><p>If there are multiple king-shamans after each change, print the index of any of them.</p>





```input1
2 1
1 3
1 2

```




```input2
3 4
2 2 3
1 1
1 2
2 4
3 6

```




```input3
10 7
0 3 1 4 6 2 7 8 10 1
2 5
1 3
9 36
4 10
4 9
1 2
1 0

```




```output1
-1

```




```output2
3
2
-1
3

```




```output3
1
-1
9
-1
4
-1
1

```



## Note

<p>In the first example powers of shamans after the first change are equal to <span class="tex-span">(2, 3)</span>. The answer equals <span class="tex-span"> - 1</span>, because the sum of powers of shamans before the first shaman is equal to <span class="tex-span">0</span>, and before the second is equal to <span class="tex-span">2</span>.</p><p>In the second example after the first change the powers are equal to <span class="tex-span">(1, 2, 3)</span>. The answer is equal to <span class="tex-span">3</span>, because the power of the third shaman is equal to <span class="tex-span">3</span>, and the sum of powers of the first and the second shaman is also <span class="tex-span">1 + 2 = 3</span>. After the second change the powers become equal to <span class="tex-span">(2, 2, 3)</span>, where the answer equals <span class="tex-span">2</span>. After the third change the powers become equal to <span class="tex-span">(2, 4, 3)</span>, where the answer equals <span class="tex-span"> - 1</span>. After the fourth change the powers become equal to <span class="tex-span">(2, 4, 6)</span>, where the answer equals <span class="tex-span">3</span>.</p>
