## Description

<div><p>Amr has got a large array of size <span class="tex-span"><i>n</i></span>. Amr doesn't like large arrays so he intends to make it smaller.</p><p>Amr doesn't care about anything in the array except the beauty of it. The beauty of the array is defined to be the maximum number of times that some number occurs in this array. He wants to choose the smallest subsegment of this array such that the beauty of it will be the same as the original array.</p><p>Help Amr by choosing the smallest subsegment possible.</p></div><div class="input-specification"><p>The first line contains one number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), the size of the array.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>), representing elements of the array.</p></div><div class="output-specification"><p>Output two integers <span class="tex-span"><i>l</i>, <i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>), the beginning and the end of the subsegment chosen respectively.</p><p>If there are several possible answers you may output any of them. </p></div>

## Input

<p>The first line contains one number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), the size of the array.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>), representing elements of the array.</p>

## Output

<p>Output two integers <span class="tex-span"><i>l</i>, <i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>), the beginning and the end of the subsegment chosen respectively.</p><p>If there are several possible answers you may output any of them. </p>





```input1
5
1 1 2 2 1

```




```input2
5
1 2 2 3 1

```




```input3
6
1 2 2 1 1 2

```




```output1
1 5
```




```output2
2 3
```




```output3
1 5
```



## Note

<p>A subsegment <span class="tex-span"><i>B</i></span> of an array <span class="tex-span"><i>A</i></span> from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> is an array of size <span class="tex-span"><i>r</i> - <i>l</i> + 1</span> where <span class="tex-span"><i>B</i><sub class="lower-index"><i>i</i></sub> = <i>A</i><sub class="lower-index"><i>l</i> + <i>i</i> - 1</sub></span> for all <span class="tex-span">1 ≤ <i>i</i> ≤ <i>r</i> - <i>l</i> + 1</span></p>
