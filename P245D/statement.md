## Description

<div><p>Recently Polycarpus has learned the "bitwise AND" operation (which is also called "<span class="tex-font-style-tt">AND</span>") of non-negative integers. Now he wants to demonstrate the school IT teacher his superb manipulation with the learned operation.</p><p>For that Polycarpus came to school a little earlier and wrote on the board a sequence of non-negative integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. He also wrote a square matrix <span class="tex-span"><i>b</i></span> of size <span class="tex-span"><i>n</i> × <i>n</i></span>. The element of matrix <span class="tex-span"><i>b</i></span> that sits in the <span class="tex-span"><i>i</i></span>-th row in the <span class="tex-span"><i>j</i></span>-th column (we'll denote it as <span class="tex-span"><i>b</i><sub class="lower-index"><i>ij</i></sub></span>) equals:</p><ul> <li> the "bitwise AND" of numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> (that is, <span class="tex-span"><i>b</i><sub class="lower-index"><i>ij</i></sub> = <i>a</i><sub class="lower-index"><i>i</i></sub>&nbsp;&amp;&nbsp;<i>a</i><sub class="lower-index"><i>j</i></sub></span>), if <span class="tex-span"><i>i</i> ≠ <i>j</i></span>; </li><li> -1, if <span class="tex-span"><i>i</i> = <i>j</i></span>. </li></ul><p>Having written out matrix <span class="tex-span"><i>b</i></span>, Polycarpus got very happy and wiped <span class="tex-span"><i>a</i></span> off the blackboard. But the thing is, the teacher will want this sequence to check whether Polycarpus' calculations were correct. Polycarus urgently needs to restore the removed sequence of integers, or else he won't prove that he can count correctly.</p><p>Help Polycarpus, given matrix <span class="tex-span"><i>b</i></span>, restore the sequence of numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, that he has removed from the board. Polycarpus doesn't like large numbers, so any number in the restored sequence mustn't exceed <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span> — the size of square matrix <span class="tex-span"><i>b</i></span>. Next <span class="tex-span"><i>n</i></span> lines contain matrix <span class="tex-span"><i>b</i></span>. The <span class="tex-span"><i>i</i></span>-th of these lines contains <span class="tex-span"><i>n</i></span> space-separated integers: the <span class="tex-span"><i>j</i></span>-th number represents the element of matrix <span class="tex-span"><i>b</i><sub class="lower-index"><i>ij</i></sub></span>. It is guaranteed, that for all <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i>)</span> the following condition fulfills: <span class="tex-span"><i>b</i><sub class="lower-index"><i>ii</i></sub></span> = -1. It is guaranteed that for all <span class="tex-span"><i>i</i>, <i>j</i></span> <span class="tex-span">(1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i>;&nbsp;<i>i</i> ≠ <i>j</i>)</span> the following condition fulfills: <span class="tex-span">0 ≤ <i>b</i><sub class="lower-index"><i>ij</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>ij</i></sub> = <i>b</i><sub class="lower-index"><i>ji</i></sub></span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> non-negative integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — the sequence that Polycarpus wiped off the board. Separate the numbers by whitespaces. </p><p>It is guaranteed that there is sequence <span class="tex-span"><i>a</i></span> that satisfies the problem conditions. If there are multiple such sequences, you are allowed to print any of them.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span> — the size of square matrix <span class="tex-span"><i>b</i></span>. Next <span class="tex-span"><i>n</i></span> lines contain matrix <span class="tex-span"><i>b</i></span>. The <span class="tex-span"><i>i</i></span>-th of these lines contains <span class="tex-span"><i>n</i></span> space-separated integers: the <span class="tex-span"><i>j</i></span>-th number represents the element of matrix <span class="tex-span"><i>b</i><sub class="lower-index"><i>ij</i></sub></span>. It is guaranteed, that for all <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i>)</span> the following condition fulfills: <span class="tex-span"><i>b</i><sub class="lower-index"><i>ii</i></sub></span> = -1. It is guaranteed that for all <span class="tex-span"><i>i</i>, <i>j</i></span> <span class="tex-span">(1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i>;&nbsp;<i>i</i> ≠ <i>j</i>)</span> the following condition fulfills: <span class="tex-span">0 ≤ <i>b</i><sub class="lower-index"><i>ij</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>ij</i></sub> = <i>b</i><sub class="lower-index"><i>ji</i></sub></span>.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> non-negative integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — the sequence that Polycarpus wiped off the board. Separate the numbers by whitespaces. </p><p>It is guaranteed that there is sequence <span class="tex-span"><i>a</i></span> that satisfies the problem conditions. If there are multiple such sequences, you are allowed to print any of them.</p>





```input1
1
-1

```




```input2
3
-1 18 0
18 -1 0
0 0 -1

```




```input3
4
-1 128 128 128
128 -1 148 160
128 148 -1 128
128 160 128 -1

```




```output1
0
```




```output2
18 18 0
```




```output3
128 180 148 160
```



## Note

<p>If you do not know what is the "bitwise AND" operation please read: <span class="tex-font-style-tt">http://en.wikipedia.org/wiki/Bitwise_operation</span>.</p>
