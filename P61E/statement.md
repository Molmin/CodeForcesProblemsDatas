## Description

<div><p>The Romans have attacked again. This time they are much more than the Persians but Shapur is ready to defeat them. He says: "A lion is never afraid of a hundred sheep". </p><p>Nevertheless Shapur has to find weaknesses in the Roman army to defeat them. So he gives the army a weakness number.</p><p>In Shapur's opinion the weakness of an army is equal to the number of triplets <span class="tex-span"><i>i</i>, <i>j</i>, <i>k</i></span> such that <span class="tex-span"><i>i</i> &lt; <i>j</i> &lt; <i>k</i></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &gt; <i>a</i><sub class="lower-index"><i>j</i></sub> &gt; <i>a</i><sub class="lower-index"><i>k</i></sub></span> where <span class="tex-span"><i>a</i><sub class="lower-index"><i>x</i></sub></span> is the power of man standing at position <span class="tex-span"><i>x</i></span>. The Roman army has one special trait — powers of all the people in it are distinct.</p><p>Help Shapur find out how weak the Romans are.</p></div><div class="input-specification"><p>The first line of input contains a single number <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of men in Roman army. Next line contains <span class="tex-span"><i>n</i></span> different positive integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i>, 1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — powers of men in the Roman army. </p></div><div class="output-specification"><p>A single integer number, the weakness of the Roman army. </p><p>Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preffered to use <span class="tex-font-style-tt">cout</span> (also you may use <span class="tex-font-style-tt">%I64d</span>).</p></div>

## Input

<p>The first line of input contains a single number <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of men in Roman army. Next line contains <span class="tex-span"><i>n</i></span> different positive integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i>, 1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — powers of men in the Roman army. </p>

## Output

<p>A single integer number, the weakness of the Roman army. </p><p>Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preffered to use <span class="tex-font-style-tt">cout</span> (also you may use <span class="tex-font-style-tt">%I64d</span>).</p>





```input1
3
3 2 1

```




```input2
3
2 3 1

```




```input3
4
10 8 3 1

```




```input4
4
1 5 4 3

```




```output1
1

```




```output2
0

```




```output3
4

```




```output4
1

```


