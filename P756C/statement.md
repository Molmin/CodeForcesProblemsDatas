## Description

<div><p>Nikita has a stack. A stack in this problem is a data structure that supports two operations. Operation <span class="tex-font-style-tt">push(x)</span> puts an integer <span class="tex-span"><i>x</i></span> on the top of the stack, and operation <span class="tex-font-style-tt">pop()</span> deletes the top integer from the stack, i.&nbsp;e. the last added. If the stack is empty, then the operation <span class="tex-font-style-tt">pop()</span> does nothing.</p><p>Nikita made <span class="tex-span"><i>m</i></span> operations with the stack but forgot them. Now Nikita wants to remember them. He remembers them one by one, on the <span class="tex-span"><i>i</i></span>-th step he remembers an operation he made <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>-th. In other words, he remembers the operations in order of some permutation <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>m</i></sub></span>. After each step Nikita wants to know what is the integer on the top of the stack after performing the operations he have already remembered, in the corresponding order. Help him!</p></div><div class="input-specification"><p>The first line contains the integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of operations Nikita made.</p><p>The next <span class="tex-span"><i>m</i></span> lines contain the operations Nikita remembers. The <span class="tex-span"><i>i</i></span>-th line starts with two integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 0</span> or <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 1</span>)&nbsp;— the index of operation he remembers on the step <span class="tex-span"><i>i</i></span>, and the type of the operation. <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> equals <span class="tex-span">0</span>, if the operation is <span class="tex-font-style-tt">pop()</span>, and <span class="tex-span">1</span>, is the operation is <span class="tex-font-style-tt">push(x)</span>. If the operation is <span class="tex-font-style-tt">push(x)</span>, the line also contains the integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the integer added to the stack.</p><p>It is guaranteed that each integer from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> is present exactly once among integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> integers. The integer <span class="tex-span"><i>i</i></span> should equal the number on the top of the stack after performing all the operations Nikita remembered on the steps from <span class="tex-span">1</span> to <span class="tex-span"><i>i</i></span>. If the stack is empty after performing all these operations, print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains the integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of operations Nikita made.</p><p>The next <span class="tex-span"><i>m</i></span> lines contain the operations Nikita remembers. The <span class="tex-span"><i>i</i></span>-th line starts with two integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 0</span> or <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 1</span>)&nbsp;— the index of operation he remembers on the step <span class="tex-span"><i>i</i></span>, and the type of the operation. <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> equals <span class="tex-span">0</span>, if the operation is <span class="tex-font-style-tt">pop()</span>, and <span class="tex-span">1</span>, is the operation is <span class="tex-font-style-tt">push(x)</span>. If the operation is <span class="tex-font-style-tt">push(x)</span>, the line also contains the integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the integer added to the stack.</p><p>It is guaranteed that each integer from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> is present exactly once among integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> integers. The integer <span class="tex-span"><i>i</i></span> should equal the number on the top of the stack after performing all the operations Nikita remembered on the steps from <span class="tex-span">1</span> to <span class="tex-span"><i>i</i></span>. If the stack is empty after performing all these operations, print <span class="tex-font-style-tt">-1</span>.</p>





```input1
2
2 1 2
1 0

```




```input2
3
1 1 2
2 1 3
3 0

```




```input3
5
5 0
4 0
3 1 1
2 1 1
1 1 2

```




```output1
2
2

```




```output2
2
3
2

```




```output3
-1
-1
-1
-1
2

```



## Note

<p>In the first example, after Nikita remembers the operation on the first step, the operation <span class="tex-font-style-tt">push(2)</span> is the only operation, so the answer is <span class="tex-span">2</span>. After he remembers the operation <span class="tex-font-style-tt">pop()</span> which was done before <span class="tex-font-style-tt">push(2)</span>, answer stays the same.</p><p>In the second example, the operations are <span class="tex-font-style-tt">push(2)</span>, <span class="tex-font-style-tt">push(3)</span> and <span class="tex-font-style-tt">pop()</span>. Nikita remembers them in the order they were performed.</p><p>In the third example Nikita remembers the operations in the reversed order.</p>
